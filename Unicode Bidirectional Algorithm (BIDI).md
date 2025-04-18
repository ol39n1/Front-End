# Unicode Bidirectional Algorithm (BIDI): A Comprehensive Guide

## Introduction to Bidirectional Text

The Unicode Bidirectional Algorithm (BIDI) addresses one of the complex challenges in text rendering: displaying text that contains both left-to-right (LTR) and right-to-left (RTL) scripts. This is common in many situations, such as:

- Arabic or Hebrew text that includes English words or numbers
- Technical documentation in RTL languages that contains code samples
- Multilingual content in user interfaces
- Documents containing mixed scripts in various contexts

## How the BIDI Algorithm Works

The Unicode BIDI algorithm determines how to display text with mixed directionality. It operates in several steps:

### 1. Character Types

The algorithm first assigns a directional type to each character:

- **Strong LTR**: Most Latin, Greek, Cyrillic characters (L)
- **Strong RTL**: Hebrew, Arabic, Syriac characters (R)
- **European Number**: European digits (EN)
- **Arabic Number**: Arabic-Indic digits (AN)
- **Neutral**: Spaces, punctuation, etc. (WS, ON)
- **Directional Control Characters**: Explicit formatting codes (LRE, RLE, etc.)

### 2. Resolving Neutral Characters

Neutral characters (spaces, punctuation) take on the direction of surrounding strong characters.

### 3. Implicit Level Resolution

The algorithm creates a hierarchy of directional levels:
- Even levels represent LTR text
- Odd levels represent RTL text

### 4. Reordering

The text is finally reordered based on these levels for display.

## BIDI Control Characters

Unicode provides special characters to explicitly control text direction:

### Embedding Controls

| Character | Unicode | Description |
|-----------|---------|-------------|
| LRE | U+202A | Left-to-Right Embedding |
| RLE | U+202B | Right-to-Left Embedding |
| PDF | U+202C | Pop Directional Formatting (end embedding) |

### Override Controls

| Character | Unicode | Description |
|-----------|---------|-------------|
| LRO | U+202D | Left-to-Right Override |
| RLO | U+202E | Right-to-Left Override |

### Isolate Controls (Newer and Preferred)

| Character | Unicode | Description |
|-----------|---------|-------------|
| LRI | U+2066 | Left-to-Right Isolate |
| RLI | U+2067 | Right-to-Left Isolate |
| FSI | U+2068 | First Strong Isolate |
| PDI | U+2069 | Pop Directional Isolate |

### Directional Marks

| Character | Unicode | Description |
|-----------|---------|-------------|
| LRM | U+200E | Left-to-Right Mark |
| RLM | U+200F | Right-to-Left Mark |
| ALM | U+061C | Arabic Letter Mark |

## Example of BIDI Algorithm Application

Consider this text: "The book title is مرحبا بالعالم (Hello World) in Arabic."

1. The Latin text "The book title is" is assigned LTR direction
2. The Arabic text "مرحبا بالعالم" is assigned RTL direction
3. The parenthesized English text "(Hello World)" is assigned LTR direction
4. The final text "in Arabic." is assigned LTR direction
5. The algorithm creates embedding levels and reorders for display

The result displays with the Arabic text flowing RTL, while the surrounding English flows LTR.

## Using CSS for Bidirectional Text

CSS provides several properties to control bidirectional text:

### The `direction` Property

```css
/* Set base direction to RTL */
.rtl-container {
  direction: rtl;
}

/* Set base direction to LTR */
.ltr-container {
  direction: ltr;
}
```

### The `unicode-bidi` Property

```css
/* Override the bidirectional algorithm */
.bidi-override {
  unicode-bidi: bidi-override;
  direction: rtl;
}

/* Isolate and embed */
.bidi-isolate {
  unicode-bidi: isolate;
}

.bidi-embed {
  unicode-bidi: embed;
}

/* Plain text in opposite direction */
.bidi-plaintext {
  unicode-bidi: plaintext;
}
```

### HTML `dir` Attribute

```html
<!-- Base document direction -->
<html dir="rtl">
  <!-- Content here will have RTL as base direction -->
  
  <!-- Override for specific element -->
  <p dir="ltr">This paragraph has LTR direction.</p>
  
  <!-- Auto-detect direction based on first strong character -->
  <p dir="auto">This paragraph's direction depends on its content.</p>
</html>
```

## Common Challenges and Solutions

### 1. Numbering in RTL Text

Arabic numerals still flow LTR even in RTL text:

```html
<p dir="rtl">الصفحة 123 من الكتاب</p>
```

This displays with "123" still in LTR order, not "321".

### 2. Punctuation at Boundaries

Punctuation can appear on unexpected sides of text:

```html
<p dir="rtl">هذا هو "مثال" للنص.</p>
```

The quotation marks positioning is handled by the BIDI algorithm.

### 3. Mixed Content with HTML

When mixing HTML with bidirectional content:

```html
<p dir="rtl">
  النص بالعربية <span dir="ltr">English text</span> ثم نص عربي مرة أخرى.
</p>
```

### 4. Mirrored Characters

Some symbols are automatically mirrored in RTL context:
- Parentheses: ( ) becomes ) (
- Greater/less than: < > becomes > <
- Square brackets: [ ] becomes ] [

## Best Practices for Bidirectional Text

### 1. Set Base Direction

Always establish the base direction for your document:

```html
<html dir="rtl" lang="ar">
  <!-- Arabic website with RTL base direction -->
</html>
```

### 2. Use Isolates Instead of Embeddings

Newer isolate controls (LRI, RLI, FSI) are preferred over older embeddings:

```html
<!-- Better approach -->
<span dir="rtl">Arabic text with <span dir="ltr">isolated English</span> content</span>

<!-- Rather than using control characters -->
```

### 3. Use Logical CSS Properties

Use logical properties instead of physical ones:

```css
/* Using logical properties */
.container {
  margin-inline-end: 20px;  /* instead of margin-right or margin-left */
  padding-inline-start: 10px; /* instead of padding-left or padding-right */
  border-inline-start: 1px solid gray; /* instead of border-left or border-right */
}
```

### 4. Consider Text Alignment

Text alignment should respect the script direction:

```css
/* Let alignment follow direction */
.container {
  text-align: start;  /* aligns left in LTR, right in RTL */
}
```

### 5. Handle User-Generated Content

For user content with unpredictable script:

```html
<div dir="auto">
  <!-- User-generated content here will determine its own direction -->
</div>
```

### 6. Test with Real Content

Always test bidirectional layouts with real multilingual content, not placeholder text.

## Advanced BIDI Management with JavaScript

### Detecting Text Direction

```javascript
function getTextDirection(text) {
  // RTL markers and common RTL script characters
  const rtlChars = /[\u0591-\u07FF\u200F\u202B\u202E\uFB1D-\uFDFD\uFE70-\uFEFC]/;
  return rtlChars.test(text) ? 'rtl' : 'ltr';
}

// Set direction based on content
function setElementDirection(element) {
  const direction = getTextDirection(element.textContent);
  element.dir = direction;
}
```

### Working with Form Inputs

```javascript
// Auto-detect and set direction for input fields
document.querySelectorAll('input[type="text"]').forEach(input => {
  input.addEventListener('input', function() {
    this.dir = getTextDirection(this.value);
  });
});
```

## Conclusion

Understanding the Unicode Bidirectional Algorithm is essential for creating truly multilingual applications and websites. By properly implementing BIDI support through appropriate HTML attributes, CSS properties, and following best practices, you can ensure that mixed-direction text displays correctly and predictably across different languages and scripts.

The BIDI algorithm's complexity reflects the challenge of seamlessly integrating writing systems with different natural flow directions. With proper implementation, users can experience content in their native scripts without disruption to the reading experience.

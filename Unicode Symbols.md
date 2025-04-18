## Windows Guide

### 1. Alt + X Method (Hexadecimal)

1. In most Windows text fields (Word, Notepad, etc.), type the **hexadecimal** codepoint (e.g., `2620`) where you want the character.
    
2. Press and release **Alt + X**. The code will convert into the corresponding Unicode character (e.g., `☠`).
    
3. If the codepoint abuts other text, highlight only the hexadecimal digits before pressing **Alt + X**.
    

### 2. Alt + Numpad Method (Decimal)

1. Ensure **Num Lock** is enabled and use the numeric keypad.
    
2. Press and hold **Alt**, type the **decimal** codepoint (e.g., `9760` for U+2620), then release **Alt**.
    
3. Note that this method is officially supported only for values up to `65535` and may vary by application and code page.
    

### 3. Registry‑Enabled Hex Input (Full Unicode)

1. Run **regedit** and navigate to  
    `HKEY_CURRENT_USER\Control Panel\Input Method`
    
2. Create a new **String Value** named `EnableHexNumpad` and set its data to `1`.
    
3. Log out and back in (or reboot).
    
4. With **Num Lock** on, hold **Alt**, press `+` on the numeric keypad, type the **hexadecimal** codepoint (e.g., `2620`), then release **Alt**.
    

## macOS Guide

### 4. Option‑Key Hex Input

1. Open **System Settings** and go to **Keyboard > Input Sources**, then click **+**.
    
2. Add **Unicode Hex Input** from the list of input sources.
    
3. Switch to the **Unicode Hex Input** layout (via the menu bar or shortcut).
    
4. Hold **Option**, type the four‑digit **hexadecimal** code (e.g., `2620`), then release **Option**.
    

### 5. Programmer Calculator Utility (Alternative)

1. Open the **Calculator** app and switch to **Programmer** mode.
    
2. Click the **Unicode** button, enter the hexadecimal codepoint (e.g., `2620`), and copy the resulting symbol.
    

## Linux Guide

### 6. Ctrl + Shift + U Method (GTK/Qt)

1. In most Linux GUI applications, press **Ctrl + Shift + U**, then release.
    
2. Type the **hexadecimal** codepoint (e.g., `2620`).
    
3. Press **Enter** or **Space** to commit the character (e.g., `☠`).
    

## Important Considerations

- **Font Support**  
    Characters will render only if the active font includes that glyph.
    
- **Application Support**  
    Not all applications support every input method; for example, Alt + X works broadly in Office apps but may not in some legacy editors.
    
- **Hexadecimal vs. Decimal**  
    Alt + X and registry methods use **hex**; classic Alt codes use **decimal**.
    
- **Numeric Keypad Requirements**  
    Windows Alt‑based methods require the **numeric keypad** (not the top‑row numbers) with **Num Lock** enabled.

| Symbol | Name                                 | Codepoint | Block                                 | Category     |
| ------ | ------------------------------------ | --------- | ------------------------------------- | ------------ |
| ☣      | Biohazard Sign                       | U+2623    | Miscellaneous Symbols                 | Other Symbol |
| ☢      | Radioactive Sign                     | U+2622    | Miscellaneous Symbols                 | Other Symbol |
| ☠      | Skull and Crossbones                 | U+2620    | Miscellaneous Symbols                 | Other Symbol |
| ⚡      | High Voltage Sign                    | U+26A1    | Miscellaneous Symbols                 | Other Symbol |
| ✨      | Sparkles                             | U+2728    | Dingbats                              | Other Symbol |
| ❄      | Snowflake                            | U+2744    | Dingbats                              | Other Symbol |
| ⚽      | Soccer Ball                          | U+26BD    | Miscellaneous Symbols                 | Other Symbol |
| ♞      | Black Chess Knight                   | U+265E    | Miscellaneous Symbols                 | Other Symbol |
| ☯      | Yin Yang                             | U+262F    | Miscellaneous Symbols                 | Other Symbol |
| ☘      | Shamrock                             | U+2618    | Miscellaneous Symbols                 | Other Symbol |
| ❇      | Sparkle                              | U+2747    | Dingbats                              | Other Symbol |
| ✂      | Black Scissors                       | U+2702    | Dingbats                              | Other Symbol |
| ✈      | Airplane                             | U+2708    | Dingbats                              | Other Symbol |
| ✉      | Envelope                             | U+2709    | Dingbats                              | Other Symbol |
| ❥      | Rotated Heavy Black Heart Bullet     | U+2765    | Dingbats                              | Other Symbol |
| ❦      | Floral Heart Decoration              | U+2766    | Dingbats                              | Other Symbol |
| ✆      | Telephone Location Sign              | U+2706    | Dingbats                              | Other Symbol |
| ☂      | Umbrella                             | U+2602    | Miscellaneous Symbols                 | Other Symbol |
| ☔      | Umbrella with Rain Drops             | U+2614    | Miscellaneous Symbols                 | Other Symbol |
| ☃      | Snowman                              | U+2603    | Miscellaneous Symbols                 | Other Symbol |
| ♻      | Black Universal Recycling Symbol     | U+2672    | Miscellaneous Symbols                 | Other Symbol |
| ⚙      | Gear                                 | U+2699    | Miscellaneous Symbols                 | Other Symbol |
| ⚔      | Crossed Swords                       | U+2694    | Miscellaneous Symbols                 | Other Symbol |
| ⚜      | Fleur‑de‑lis                         | U+269C    | Miscellaneous Symbols                 | Other Symbol |
| ⚛      | Atom Symbol                          | U+269B    | Miscellaneous Symbols                 | Other Symbol |
| ♕      | White Chess Queen                    | U+2655    | Miscellaneous Symbols                 | Other Symbol |
| ♟      | Black Chess Pawn                     | U+265F    | Miscellaneous Symbols                 | Other Symbol |
| ♤      | White Spade Suit                     | U+2664    | Miscellaneous Symbols                 | Other Symbol |
| ♡      | White Heart Suit                     | U+2661    | Miscellaneous Symbols                 | Other Symbol |
| ♨      | Hot Springs                          | U+2668    | Miscellaneous Symbols                 | Other Symbol |
| ☮      | Peace Symbol                         | U+262E    | Miscellaneous Symbols                 | Other Symbol |
| ☭      | Hammer and Sickle                    | U+262D    | Miscellaneous Symbols                 | Other Symbol |
| ✪      | Circled White Star                   | U+272A    | Dingbats                              | Other Symbol |
| ✰      | Star with Right Half Black           | U+2730    | Dingbats                              | Other Symbol |
| ☕      | Hot Beverage                         | U+2615    | Miscellaneous Symbols                 | Other Symbol |
| ♛      | White Chess Bishop                   | U+265B    | Miscellaneous Symbols                 | Other Symbol |
| ⚐      | White Flag                           | U+2690    | Miscellaneous Symbols                 | Other Symbol |
| ⚑      | Black Flag                           | U+2691    | Miscellaneous Symbols                 | Other Symbol |
| ♩      | Quarter Note                         | U+2669    | Miscellaneous Symbols                 | Other Symbol |
| ♪      | Eighth Note                          | U+266A    | Miscellaneous Symbols                 | Other Symbol |
| ♫      | Beamed Eighth Notes                  | U+266B    | Miscellaneous Symbols                 | Other Symbol |
| ♬      | Beamed Sixteenth Notes               | U+266C    | Miscellaneous Symbols                 | Other Symbol |
| ☀      | Black Sun with Rays                  | U+2600    | Miscellaneous Symbols                 | Other Symbol |
| ☽      | First Quarter Moon                   | U+263D    | Miscellaneous Symbols                 | Other Symbol |
| ☾      | Last Quarter Moon                    | U+263E    | Miscellaneous Symbols                 | Other Symbol |
| ☤      | Caduceus                             | U+2624    | Miscellaneous Symbols                 | Other Symbol |
| ☥      | Ankh                                 | U+2625    | Miscellaneous Symbols                 | Other Symbol |
| ☦      | Orthodox Cross                       | U+2626    | Miscellaneous Symbols                 | Other Symbol |
| ☧      | Chi Rho                              | U+2627    | Miscellaneous Symbols                 | Other Symbol |
| ☨      | Cross of Lorraine                    | U+2628    | Miscellaneous Symbols                 | Other Symbol |
| ✵      | Six Pointed Black Star               | U+2735    | Dingbats                              | Other Symbol |
| ∞      | Infinity                             | U+221E    | Mathematical Operators                | Math Symbol  |
| ∂      | Partial Differential                 | U+2202    | Mathematical Operators                | Math Symbol  |
| ∑      | N-Ary Summation                      | U+2211    | Mathematical Operators                | Math Symbol  |
| ∏      | N-Ary Product                        | U+220F    | Mathematical Operators                | Math Symbol  |
| √      | Square Root                          | U+221A    | Mathematical Operators                | Math Symbol  |
| ≈      | Almost Equal To                      | U+2248    | Mathematical Operators                | Math Symbol  |
| ≠      | Not Equal To                         | U+2260    | Mathematical Operators                | Math Symbol  |
| ≤      | Less-Than or Equal To                | U+2264    | Mathematical Operators                | Math Symbol  |
| ≥      | Greater-Than or Equal To             | U+2265    | Mathematical Operators                | Math Symbol  |
| ∅      | Empty Set                            | U+2205    | Mathematical Operators                | Math Symbol  |
| ✡      | Star of David                        | U+2721    | Dingbats                              | Other Symbol |
| ✢      | Four Teardrop-Spoked Asterisk        | U+2722    | Dingbats                              | Other Symbol |
| ❖      | Black Diamond Minus White X          | U+2756    | Dingbats                              | Other Symbol |
| ❂      | Sun with Rays                        | U+2742    | Dingbats                              | Other Symbol |
| ✤      | Heavy Four Balloon-Spoked Asterisk   | U+2724    | Dingbats                              | Other Symbol |
| ✧      | Sparkle                              | U+2727    | Dingbats                              | Other Symbol |
| ✩      | Stress Outlined White Star           | U+2729    | Dingbats                              | Other Symbol |
| ✫      | Open Centre Black Star               | U+272B    | Dingbats                              | Other Symbol |
| ✬      | Heavy Open Centre Black Star         | U+272C    | Dingbats                              | Other Symbol |
| ✭      | Black Centre White Star              | U+272D    | Dingbats                              | Other Symbol |
| ▲      | Black Up-Pointing Triangle           | U+25B2    | Geometric Shapes                      | Other Symbol |
| ▼      | Black Down-Pointing Triangle         | U+25BC    | Geometric Shapes                      | Other Symbol |
| ◀      | Black Left-Pointing Triangle         | U+25C0    | Geometric Shapes                      | Other Symbol |
| ▶      | Black Right-Pointing Triangle        | U+25B6    | Geometric Shapes                      | Other Symbol |
| ◆      | Black Diamond                        | U+25C6    | Geometric Shapes                      | Other Symbol |
| ◇      | White Diamond                        | U+25C7    | Geometric Shapes                      | Other Symbol |
| ■      | Black Square                         | U+25A0    | Geometric Shapes                      | Other Symbol |
| □      | White Square                         | U+25A1    | Geometric Shapes                      | Other Symbol |
| ○      | White Circle                         | U+25CB    | Geometric Shapes                      | Other Symbol |
| ●      | Black Circle                         | U+25CF    | Geometric Shapes                      | Other Symbol |
| ⌘      | Place of Interest Sign (Command)     | U+2318    | Miscellaneous Technical               | Other Symbol |
| ⌥      | Option Key                           | U+2325    | Miscellaneous Technical               | Other Symbol |
| ⌫      | Erase to the Left                    | U+232B    | Miscellaneous Technical               | Other Symbol |
| ⏎      | Return Symbol                        | U+23CE    | Miscellaneous Technical               | Other Symbol |
| ⏏      | Eject Symbol                         | U+23CF    | Miscellaneous Technical               | Other Symbol |
| ─      | Box Drawings Light Horizontal        | U+2500    | Box Drawing                           | Other Symbol |
| │      | Box Drawings Light Vertical          | U+2502    | Box Drawing                           | Other Symbol |
| ┌      | Box Drawings Light Down and Right    | U+250C    | Box Drawing                           | Other Symbol |
| ┐      | Box Drawings Light Down and Left     | U+2510    | Box Drawing                           | Other Symbol |
| └      | Box Drawings Light Up and Right      | U+2514    | Box Drawing                           | Other Symbol |
| ←      | Leftwards Arrow                      | U+2190    | Arrows                                | Other Symbol |
| ↑      | Upwards Arrow                        | U+2191    | Arrows                                | Other Symbol |
| →      | Rightwards Arrow                     | U+2192    | Arrows                                | Other Symbol |
| ↓      | Downwards Arrow                      | U+2193    | Arrows                                | Other Symbol |
| ↔      | Left Right Arrow                     | U+2194    | Arrows                                | Other Symbol |
| 🤖     | Robot Face                           | U+1F916   | Miscellaneous Symbols and Pictographs | Emoji        |
| 🧿     | Nazar Amulet                         | U+1F9FF   | Supplemental Symbols and Pictographs  | Emoji        |
| 🦄     | Unicorn Face                         | U+1F984   | Miscellaneous Symbols and Pictographs | Emoji        |
| 🐉     | Dragon                               | U+1F409   | Miscellaneous Symbols and Pictographs | Emoji        |
| 🍄     | Mushroom                             | U+1F344   | Miscellaneous Symbols and Pictographs | Emoji        |
| ⠁      | Braille Pattern Dot‑1                | U+2801    | Braille Patterns                      | Other Symbol |
| ⠿      | Braille Pattern Dots‑1‑2‑3‑4‑5‑6‑7‑8 | U+28FF    | Braille Patterns                      | Other Symbol |
| ▀      | Upper Half Block                     | U+2580    | Block Elements                        | Other Symbol |
| ▄      | Lower Half Block                     | U+2584    | Block Elements                        | Other Symbol |
| ␀      | Symbol for Null                      | U+2400    | Control Pictures                      | Other Symbol |
| ␊      | Symbol for Line Feed                 | U+240A    | Control Pictures                      | Other Symbol |
| ⑴      | Parenthesized Digit One              | U+2474    | Enclosed Alphanumerics                | Other Symbol |
| ⓿      | Parenthesized Number Zero            | U+24FF    | Enclosed Alphanumerics                | Other Symbol |
| ℑ      | Black‑Letter Capital I               | U+2111    | Letterlike Symbols                    | Other Symbol |
| ℎ      | Planck Constant                      | U+210E    | Letterlike Symbols                    | Other Symbol |
| ⅓      | Vulgar Fraction One Third            | U+2153    | Number Forms                          | Other Symbol |
| ⅝      | Vulgar Fraction Five Eighths         | U+215D    | Number Forms                          | Other Symbol |
| ⟀      | N‑Ary Circled Times Operator         | U+27C0    | Miscellaneous Mathematical Symbols‑A  | Math Symbol  |
| ⤀      | Rightwards Two‑Headed Arrow          | U+2900    | Supplemental Arrows‑B                 | Other Symbol |
| 🚃     | Train                                | U+1F683   | Transport and Map Symbols             | Pictograph   |
| 🚲     | Bicycle                              | U+1F6B2   | Transport and Map Symbols             | Pictograph   |
| 😎     | Smiling Face with Sunglasses         | U+1F60E   | Emoticons                             | Emoji        |
| 😱     | Face Screaming in Fear               | U+1F631   | Emoticons                             | Emoji        |
| ⸚      | Hyphen with Diaeresis                | U+2E1A    | Supplemental Punctuation              | Punctuation  |
| ⸽      | Vertical Six Dots                    | U+2E3D    | Supplemental Punctuation              | Punctuation  |
| ·      | North West Pointing Leaf Ornament    | U+1F650   | Ornamental Dingbats                   | Decorative   |
| ¸      | South West Pointing Leaf Ornament    | U+1F651   | Ornamental Dingbats                   | Decorative   |
| 🔴     | Large Red Circle                     | U+1F534   | Miscellaneous Symbols and Pictographs | Emoji        |
| 🔵     | Large Blue Circle                    | U+1F535   | Miscellaneous Symbols and Pictographs | Emoji        |
| 🟠     | Large Orange Circle                  | U+1F7E0   | Geometric Shapes Extended             | Geometric    |
| 🟡     | Large Yellow Circle                  | U+1F7E1   | Geometric Shapes Extended             | Geometric    |
| 🟢     | Large Green Circle                   | U+1F7E2   | Geometric Shapes Extended             | Geometric    |
| 🟣     | Large Purple Circle                  | U+1F7E3   | Geometric Shapes Extended             | Geometric    |
| 🟤     | Large Brown Circle                   | U+1F7E4   | Geometric Shapes Extended             | Geometric    |
| 🟥     | Large Red Square                     | U+1F7E5   | Geometric Shapes Extended             | Geometric    |
| 🟦     | Large Blue Square                    | U+1F7E6   | Geometric Shapes Extended             | Geometric    |
| 🟧     | Large Orange Square                  | U+1F7E7   | Geometric Shapes Extended             | Geometric    |
| 🟨     | Large Yellow Square                  | U+1F7E8   | Geometric Shapes Extended             | Geometric    |
| 🟩     | Large Green Square                   | U+1F7E9   | Geometric Shapes Extended             | Geometric    |
| 🟪     | Large Purple Square                  | U+1F7EA   | Geometric Shapes Extended             | Geometric    |
| 🟫     | Large Brown Square                   | U+1F7EB   | Geometric Shapes Extended             | Geometric    |

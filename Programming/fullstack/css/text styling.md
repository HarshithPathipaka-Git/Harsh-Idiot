# Text Styling ⭐⭐⭐

## What is Text Styling?

Text Styling is used to control the appearance of text.

Used for

- Color
- Font
- Size
- Alignment
- Spacing
- Decoration
- Effects

Example

```
h1{    color: blue;    font-size: 32px;}
```

---

# 1. color ⭐⭐⭐⭐⭐

Changes the text color.

Syntax

```
color: value;
```

Example

```
color: red;color: #ff0000;color: rgb(255,0,0);
```

Common Uses

- Headings
- Paragraphs
- Links
- Buttons

---

# 2. font-family ⭐⭐⭐⭐⭐

Changes the font.

Syntax

```
font-family: font-name;
```

Example

```
font-family: Arial;
```

Multiple Fonts

```
font-family: Arial, Helvetica, sans-serif;
```

The browser uses the first available font.

---

# 3. font-size ⭐⭐⭐⭐⭐

Changes text size.

Syntax

```
font-size: value;
```

Example

```
font-size:16px;font-size:2rem;
```

Common Units

- px
- rem
- em

Recommended

✔ `rem` for responsive designs

---

# 4. font-weight ⭐⭐⭐⭐

Controls text thickness.

Example

```
font-weight: normal;font-weight: bold;font-weight: 400;font-weight: 700;
```

Common Values

```
100 Thin300 Light400 Normal500 Medium600 Semi Bold700 Bold800 Extra Bold900 Black
```

---

# 5. font-style ⭐⭐

Changes the font style.

Example

```
font-style: normal;font-style: italic;font-style: oblique;
```

Mostly used for italic text.

---

# 6. line-height ⭐⭐⭐⭐

Controls space between lines.

Example

```
line-height:2;line-height:30px;line-height:1.5;
```

Useful for

- Paragraph readability
- Long text

---

# 7. letter-spacing ⭐⭐⭐

Controls space between letters.

Example

```
letter-spacing:2px;
```

Negative values

```
letter-spacing:-1px;
```

Used for

- Headings
- Logos
- Titles

---

# 8. word-spacing ⭐⭐

Controls space between words.

Example

```
word-spacing:10px;
```

Mostly used in paragraphs.

---

# 9. text-align ⭐⭐⭐⭐⭐

Aligns text horizontally.

Example

```
text-align:left;text-align:center;text-align:right;text-align:justify;
```

Most Used

- center
- left

---

# 10. text-decoration ⭐⭐⭐⭐

Adds or removes decorations.

Example

```
text-decoration:none;
```

```
text-decoration:underline;
```

```
text-decoration:line-through;
```

```
text-decoration:overline;
```

Most Common

```
a{    text-decoration:none;}
```

Removes the underline from links.

---

# 11. text-transform ⭐⭐⭐

Changes letter casing.

Example

```
text-transform:uppercase;
```

```
text-transform:lowercase;
```

```
text-transform:capitalize;
```

```
text-transform:none;
```

Output

```
hello world↓HELLO WORLD
```

---

# 12. text-indent ⭐⭐

Adds indentation to the first line.

Example

```
text-indent:40px;
```

Mostly used in articles and books.

---

# 13. text-shadow ⭐⭐⭐

Adds shadow to text.

Syntax

```
text-shadow:horizontalverticalblurcolor;
```

Example

```
text-shadow:2px 2px 5px gray;
```

Useful for

- Titles
- Hero Sections
- Logos

---

# 14. white-space ⭐⭐⭐

Controls how whitespace and line breaks are handled.

Common Values

```
white-space: normal;
```

(Default)

```
white-space: nowrap;
```

(Text stays on one line)

```
white-space: pre;
```

(Preserves spaces and line breaks)

Common Use

```
white-space: nowrap;
```

Prevents text from wrapping.

---

# 15. overflow-wrap ⭐⭐⭐

Breaks long words to prevent overflow.

Example

```
overflow-wrap: break-word;
```

Useful for

- Long URLs
- Long email addresses
- Large words

---

# Font Shorthand ⭐⭐⭐⭐

Instead of writing multiple properties separately:

```
font-style: italic;font-weight: bold;font-size: 20px;line-height: 1.5;font-family: Arial, sans-serif;
```

You can write:

```
font: italic bold 20px/1.5 Arial, sans-serif;
```

✔ Cleaner code

✔ Common in professional projects

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|color|⭐⭐⭐⭐⭐|
|font-family|⭐⭐⭐⭐⭐|
|font-size|⭐⭐⭐⭐⭐|
|text-align|⭐⭐⭐⭐⭐|
|font-weight|⭐⭐⭐⭐|
|text-decoration|⭐⭐⭐⭐|
|line-height|⭐⭐⭐⭐|
|text-transform|⭐⭐⭐|
|text-shadow|⭐⭐⭐|
|letter-spacing|⭐⭐⭐|
|white-space|⭐⭐⭐|
|overflow-wrap|⭐⭐⭐|
|word-spacing|⭐⭐|
|font-style|⭐⭐|
|text-indent|⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Text Color

```
color:red;
```

---

### Font

```
font-family:Arial, sans-serif;
```

---

### Font Size

```
font-size:2rem;
```

---

### Font Weight

```
font-weight:700;
```

---

### Font Style

```
font-style:italic;
```

---

### Line Height

```
line-height:1.5;
```

---

### Letter Spacing

```
letter-spacing:2px;
```

---

### Word Spacing

```
word-spacing:10px;
```

---

### Text Align

```
text-align:center;
```

---

### Text Decoration

```
text-decoration:none;
```

---

### Text Transform

```
text-transform:uppercase;
```

---

### Text Indent

```
text-indent:40px;
```

---

### Text Shadow

```
text-shadow:2px 2px 5px gray;
```

---

### White Space

```
white-space:nowrap;
```

---

### Overflow Wrap

```
overflow-wrap:break-word;
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. color ⭐⭐⭐⭐⭐2. font-size ⭐⭐⭐⭐⭐3. font-family ⭐⭐⭐⭐⭐4. text-align ⭐⭐⭐⭐⭐5. font-weight ⭐⭐⭐⭐6. line-height ⭐⭐⭐⭐7. text-decoration ⭐⭐⭐⭐8. text-transform ⭐⭐⭐9. letter-spacing ⭐⭐⭐10. text-shadow ⭐⭐11. white-space ⭐⭐12. overflow-wrap ⭐⭐13. font-style ⭐⭐14. word-spacing ⭐15. text-indent ⭐
```

---

## 💡 Full Stack Tip

In day-to-day frontend development, you'll use these properties constantly:

- `color`
- `font-family`
- `font-size`
- `font-weight`
- `line-height`
- `text-align`
- `text-decoration`

Master these first, and you'll be able to style almost all text on a website.
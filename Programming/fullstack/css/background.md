#  Background ⭐⭐⭐

## What is Background?

The **background** is the area behind an element's content.

Used for:

- Colors
- Images
- Gradients
- Hero Sections
- Cards
- Buttons

Example

```
body{    background-color: lightblue;}
```

---

# 1. background-color ⭐⭐⭐⭐⭐

Sets the background color of an element.

Syntax

```
background-color: value;
```

Example

```
body{    background-color: white;}div{    background-color: #f5f5f5;}button{    background-color: rgb(0,123,255);}
```

Common Uses

- Body
- Cards
- Buttons
- Sections

---

# 2. background-image ⭐⭐⭐⭐

Adds an image as the background.

Syntax

```
background-image: url("image.jpg");
```

Example

```
body{    background-image: url("bg.jpg");}
```

You can also use gradients.

```
background-image: linear-gradient(red, blue);
```

---

# 3. background-repeat ⭐⭐⭐

Controls whether the background image repeats.

Default

```
background-repeat: repeat;
```

Common Values

```
background-repeat: repeat;background-repeat: no-repeat;background-repeat: repeat-x;background-repeat: repeat-y;
```

### Meaning

|Value|Result|
|---|---|
|repeat|Repeat both directions (Default)|
|no-repeat|Show once|
|repeat-x|Repeat horizontally|
|repeat-y|Repeat vertically|

Most websites use

```
background-repeat: no-repeat;
```

---

# 4. background-position ⭐⭐⭐

Controls where the background image appears.

Example

```
background-position: center;
```

Common Values

```
background-position: left;background-position: center;background-position: right;background-position: top;background-position: bottom;background-position: center center;
```

You can also use pixel or percentage values.

```
background-position: 50% 50%;background-position: 20px 40px;
```

---

# 5. background-size ⭐⭐⭐⭐

Controls the size of the background image.

Common Values

```
background-size: auto;background-size: cover;background-size: contain;background-size: 300px 200px;
```

### cover ⭐⭐⭐⭐⭐

Fills the entire element.

Image may be cropped.

```
background-size: cover;
```

---

### contain ⭐⭐⭐

Shows the complete image.

May leave empty space.

```
background-size: contain;
```

---

# cover vs contain ⭐⭐⭐⭐

|cover|contain|
|---|---|
|Fills container|Shows full image|
|May crop image|May leave empty space|
|Most commonly used|Used when full image must be visible|

---

# 6. background-attachment ⭐⭐

Controls whether the background scrolls.

Values

```
background-attachment: scroll;background-attachment: fixed;background-attachment: local;
```

### fixed

Background stays fixed while the page scrolls.

```
background-attachment: fixed;
```

Used for simple parallax-like effects.

---

# 7. background-origin ⭐

Defines where the background starts.

Values

```
background-origin: padding-box;background-origin: border-box;background-origin: content-box;
```

Usually left as the default.

---

# 8. background-clip ⭐

Controls how far the background extends.

Values

```
background-clip: border-box;background-clip: padding-box;background-clip: content-box;
```

Commonly used with borders.

---

# 9. Background Shorthand ⭐⭐⭐⭐

Instead of writing:

```
background-color: black;background-image: url("bg.jpg");background-repeat: no-repeat;background-position: center;background-size: cover;
```

You can write:

```
background: black url("bg.jpg") no-repeat center/cover;
```

This is called the **background shorthand**.

✔ Cleaner code

✔ Common in real projects

---

# Complete Example ⭐⭐⭐⭐⭐

```
body{    background: #000 url("bg.jpg") no-repeat center/cover;}
```

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|background-color|⭐⭐⭐⭐⭐|
|background-image|⭐⭐⭐⭐|
|background-size|⭐⭐⭐⭐|
|background-position|⭐⭐⭐⭐|
|background-repeat|⭐⭐⭐|
|background shorthand|⭐⭐⭐⭐|
|background-attachment|⭐⭐|
|background-origin|⭐|
|background-clip|⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Background Color

```
background-color: lightblue;
```

---

### Background Image

```
background-image: url("bg.jpg");
```

---

### Background Repeat

```
background-repeat: no-repeat;
```

---

### Background Position

```
background-position: center;
```

---

### Background Size

```
background-size: cover;
```

---

### Background Attachment

```
background-attachment: fixed;
```

---

### Background Origin

```
background-origin: padding-box;
```

---

### Background Clip

```
background-clip: border-box;
```

---

### Background Shorthand

```
background: #000 url("bg.jpg") no-repeat center/cover;
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. background-color ⭐⭐⭐⭐⭐2. background-size: cover ⭐⭐⭐⭐⭐3. background-image ⭐⭐⭐⭐4. background-position ⭐⭐⭐⭐5. background shorthand ⭐⭐⭐⭐6. background-repeat ⭐⭐⭐7. background-attachment ⭐⭐8. background-origin ⭐9. background-clip ⭐
```

---

## 💡 Full Stack Tip

In day-to-day frontend development, you'll mostly use:

- `background-color` → Cards, buttons, sections
- `background-image` → Hero sections, banners
- `background-size: cover` → Full-width backgrounds
- `background-position: center` → Center images
- `background-repeat: no-repeat` → Prevent tiling
- `background` (shorthand) → Cleaner, professional CSS

You may rarely use `background-origin` and `background-clip`, but it's useful to recognize them when reading existing code.

---
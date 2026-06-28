
# 3. Colors ⭐⭐

## What are Colors?

CSS colors are used to change the appearance of elements.

Used for

- Text
- Backgrounds
- Borders
- Shadows
- Gradients

Example

```
h1{    color: blue;}
```

---

# 1. Color Names ⭐⭐

Use predefined color names.

Example

```
h1{    color: red;}p{    color: blue;}body{    background: white;}
```

Some common color names

```
redbluegreenblackwhitegrayyelloworangepurplepinkbrowncyan
```

✔ Easy to use  
❌ Limited choices

---

# 2. HEX Color ⭐⭐⭐

HEX (Hexadecimal) starts with `#`.

Syntax

```
#RRGGBB
```

Example

```
color: #ff0000;
```

Meaning

```
#ff0000 → Red#00ff00 → Green#0000ff → Blue#ffffff → White#000000 → Black
```

Short form

```
#fff#000#f00
```

✔ Most commonly used in web development.

---

# 3. RGB ⭐⭐⭐

RGB = Red Green Blue

Syntax

```
rgb(red, green, blue)
```

Each value ranges from **0–255**.

Example

```
color: rgb(255,0,0);
```

Examples

```
rgb(255,0,0)      /* Red */rgb(0,255,0)      /* Green */rgb(0,0,255)      /* Blue */rgb(255,255,255)  /* White */rgb(0,0,0)        /* Black */
```

---

# 4. RGBA ⭐⭐⭐

RGBA = RGB + Alpha (Transparency)

Syntax

```
rgba(red, green, blue, alpha)
```

Alpha ranges from **0–1**.

```
0   → Invisible0.5 → 50% Visible1   → Fully Visible
```

Example

```
background: rgba(255,0,0,0.5);
```

Used when transparency is needed.

---

# 5. HSL ⭐⭐

HSL = Hue, Saturation, Lightness

Syntax

```
hsl(hue, saturation, lightness)
```

Example

```
color: hsl(0,100%,50%);
```

Meaning

- Hue → Color (0°–360°)
- Saturation → Color intensity
- Lightness → Brightness

Common Hue Values

```
0°    Red60°   Yellow120°  Green180°  Cyan240°  Blue300°  Purple360°  Red
```

Useful for creating color variations.

---

# 6. HSLA ⭐⭐

HSLA = HSL + Alpha

Example

```
background: hsla(240,100%,50%,0.4);
```

Adds transparency to HSL colors.

---

# 7. Opacity ⭐⭐

Controls the transparency of an entire element.

Syntax

```
opacity: value;
```

Range

```
0   → Invisible0.5 → Half Visible1   → Fully Visible
```

Example

```
img{    opacity:0.5;}
```

### Difference: RGBA vs Opacity ⭐⭐⭐

```
background: rgba(255,0,0,0.5);
```

✔ Only the **background color** becomes transparent.

```
opacity:0.5;
```

✔ The **entire element** (text, images, borders, children) becomes transparent.

---

# Which Color Format Should I Use? ⭐⭐⭐⭐⭐

|Format|Usage|
|---|---|
|Color Name|Simple examples|
|HEX|⭐ Most common in projects|
|RGB|Dynamic colors (JavaScript)|
|RGBA|Transparent colors|
|HSL|Easy color adjustments|
|HSLA|HSL + transparency|
|Opacity|Transparent elements|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Color Names

```
color:red;
```

---

### HEX ⭐

```
color:#ff0000;
```

---

### RGB

```
color:rgb(255,0,0);
```

---

### RGBA

```
background:rgba(255,0,0,0.5);
```

---

### HSL

```
color:hsl(240,100%,50%);
```

---

### HSLA

```
background:hsla(240,100%,50%,0.5);
```

---

### Opacity

```
opacity:0.5;
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. HEX ⭐⭐⭐⭐⭐2. RGB ⭐⭐⭐⭐3. RGBA ⭐⭐⭐⭐4. HSL ⭐⭐5. HSLA ⭐6. Color Names ⭐7. Opacity ⭐⭐⭐
```

> In modern web development, **HEX**, **RGB/RGBA**, and **Opacity** are the formats you'll encounter most often. HSL is also useful, especially when creating themes or adjusting colors systematically.
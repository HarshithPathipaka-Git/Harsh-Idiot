# Units ⭐⭐⭐

## What are CSS Units?

CSS Units define the **size or length** of an element.

Used in

- Width
- Height
- Font Size
- Margin
- Padding
- Gap
- Border
- Position

Example

```
h1{    font-size: 32px;}
```

Here, `32px` is the unit.

---

# Types of Units

There are **2 categories**:

### Absolute Units

Fixed size.

Example

```
px
```

---

### Relative Units

Size depends on another value.

Example

```
%emremvwvhvminvmaxfr
```

---

# 1. px (Pixel) ⭐⭐⭐⭐⭐

The most common CSS unit.

Fixed size.

Example

```
font-size:20px;width:300px;margin:10px;
```

✔ Easy to use

✔ Exact size

❌ Doesn't scale automatically

Common Uses

- Borders
- Icons
- Small spacing
- Shadows

---

# 2. % (Percentage) ⭐⭐⭐⭐

Relative to the **parent element**.

Example

```
width:50%;
```

If parent width = **400px**

```
50% = 200px
```

Common Uses

- Width
- Height
- Responsive layouts

---

# 3. em ⭐⭐⭐

Relative to the **parent's font-size**.

Example

Parent

```
font-size:20px;
```

Child

```
font-size:2em;
```

Output

```
40px
```

Useful for

- Padding
- Margin
- Font Size

⚠ Nested `em` values can compound, making sizes harder to predict.

---

# 4. rem ⭐⭐⭐⭐⭐

Relative to the **root (`html`) font-size**.

Usually

```
html{    font-size:16px;}
```

Example

```
font-size:2rem;
```

Output

```
32px
```

Advantages

✔ Consistent sizing

✔ Easy responsive design

✔ Preferred over `em` for font sizes

---

# em vs rem ⭐⭐⭐⭐⭐

|em|rem|
|---|---|
|Parent font size|Root (`html`) font size|
|Changes with nesting|Same everywhere|
|Less predictable|More predictable|

**Use `rem` for most font sizes.**

---

# 5. vw (Viewport Width) ⭐⭐⭐⭐

Relative to the browser's **width**.

```
100vw = Full browser width
```

Example

```
width:100vw;
```

Common Uses

- Full-width sections
- Hero banners

---

# 6. vh (Viewport Height) ⭐⭐⭐⭐

Relative to the browser's **height**.

```
100vh = Full browser height
```

Example

```
height:100vh;
```

Common Uses

- Landing pages
- Full-screen layouts

---

# vw vs vh

|vw|vh|
|---|---|
|Browser Width|Browser Height|

---

# 7. vmin ⭐⭐

Uses the **smaller** of viewport width or height.

Example

```
width:50vmin;
```

If

```
Width = 1200pxHeight = 800px
```

Then

```
1vmin = 1% of 800px
```

Useful for elements that should fit within the smaller screen dimension.

---

# 8. vmax ⭐⭐

Uses the **larger** of viewport width or height.

Example

```
width:50vmax;
```

If

```
Width = 1200pxHeight = 800px
```

Then

```
1vmax = 1% of 1200px
```

Useful when you want sizing based on the larger screen dimension.

---

# 9. ch ⭐⭐

Represents the width of the **"0" (zero)** character in the current font.

Example

```
width:30ch;
```

Approximately fits **30 characters**.

Common Uses

- Forms
- Input fields
- Reading widths
- Code blocks

---

# 10. fr ⭐⭐⭐⭐

Used only in **CSS Grid**.

Represents a **fraction of available space**.

Example

```
display:grid;grid-template-columns:1fr 1fr;
```

Output

```
50% | 50%
```

Example

```
grid-template-columns:1fr 2fr;
```

Output

```
33% | 67%
```

Used only with **Grid Layout**.

---

# Which Unit Should I Use? ⭐⭐⭐⭐⭐

|Unit|Best For|
|---|---|
|px|Borders, icons, exact spacing|
|%|Responsive widths/heights|
|em|Relative spacing, component sizing|
|rem|⭐ Font sizes, consistent spacing|
|vw|Full-width layouts|
|vh|Full-height layouts|
|vmin|Responsive square elements|
|vmax|Large responsive elements|
|ch|Text widths, inputs|
|fr|Grid columns/rows|

---

# Quick Revision ⭐⭐⭐⭐⭐

### px

```
font-size:16px;
```

Fixed size

---

### %

```
width:50%;
```

Relative to parent

---

### em

```
font-size:2em;
```

Relative to parent font size

---

### rem

```
font-size:2rem;
```

Relative to root font size

---

### vw

```
width:100vw;
```

Viewport width

---

### vh

```
height:100vh;
```

Viewport height

---

### vmin

```
width:50vmin;
```

Smaller viewport dimension

---

### vmax

```
width:50vmax;
```

Larger viewport dimension

---

### ch

```
width:30ch;
```

Character width

---

### fr

```
grid-template-columns:1fr 2fr;
```

Fraction of available Grid space

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. rem ⭐⭐⭐⭐⭐2. px ⭐⭐⭐⭐⭐3. % ⭐⭐⭐⭐4. fr ⭐⭐⭐⭐5. vw ⭐⭐⭐⭐6. vh ⭐⭐⭐⭐7. em ⭐⭐⭐8. ch ⭐⭐9. vmin ⭐10. vmax ⭐
```

### 💡 Full Stack Tip

If you're building modern websites with **Flexbox**, **Grid**, and **responsive design**, you'll use these units the most:

- `rem` → Font sizes, padding, margin
- `px` → Borders, icons, small spacing
- `%` → Responsive widths
- `vw` / `vh` → Full-screen sections
- `fr` → Grid layouts

Master these five, and you'll cover the vast majority of CSS sizing in real-world projects.
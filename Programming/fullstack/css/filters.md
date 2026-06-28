# Filters ⭐⭐

## What are Filters?

The `filter` property applies **visual effects** to an element.

Works with

- Images (`<img>`)
- Backgrounds
- Videos
- Entire Elements

Used for

- Hover Effects
- Image Editing
- Dark Mode Effects
- Hero Sections
- Photo Galleries

Syntax

```
filter:function(value);
```

---

# Common Filter Functions

```
blur()brightness()contrast()grayscale()invert()sepia()drop-shadow()
```

---

# 1. blur() ⭐⭐⭐

Blurs an element.

Syntax

```
filter:blur(value);
```

Example

```
filter:blur(5px);
```

Result

✔ Soft, blurry image

Common Uses

- Loading placeholders
- Background effects
- Glassmorphism

---

# 2. brightness() ⭐⭐⭐⭐

Adjusts brightness.

Syntax

```
filter:brightness(value);
```

Examples

```
filter:brightness(50%);
```

Darker

```
filter:brightness(150%);
```

Brighter

Default

```
filter:brightness(100%);
```

---

# 3. contrast() ⭐⭐⭐

Adjusts contrast.

Syntax

```
filter:contrast(value);
```

Example

```
filter:contrast(150%);
```

Higher values make darks darker and lights lighter.

---

# 4. grayscale() ⭐⭐⭐⭐

Converts an image to black and white.

Syntax

```
filter:grayscale(value);
```

Example

```
filter:grayscale(100%);
```

Remove grayscale

```
filter:grayscale(0%);
```

Common Hover Effect

```
img{    filter:grayscale(100%);}img:hover{    filter:grayscale(0%);}
```

---

# 5. invert() ⭐⭐⭐

Inverts colors.

Syntax

```
filter:invert(value);
```

Example

```
filter:invert(100%);
```

Common Uses

- Dark mode icons
- Special effects

---

# 6. sepia() ⭐⭐

Applies a vintage brown tone.

Syntax

```
filter:sepia(value);
```

Example

```
filter:sepia(100%);
```

Used for

- Old photo effects
- Vintage designs

---

# 7. drop-shadow() ⭐⭐⭐

Adds a shadow around the visible shape of an element.

Syntax

```
filter:drop-shadow(x y blur color);
```

Example

```
filter:drop-shadow(2px 2px 5px gray);
```

Unlike `box-shadow`, it follows the **visible shape** (useful for transparent PNGs and SVGs).

---

# box-shadow vs drop-shadow ⭐⭐⭐⭐

|box-shadow|drop-shadow|
|---|---|
|Around the element's box|Around the visible shape|
|Works on all elements|Great for images & SVGs|
|Supports spread & inset|No spread or inset|

---

# Multiple Filters ⭐⭐⭐⭐

You can combine filters.

```
filter:blur(2px)brightness(120%)contrast(110%);
```

---

# Common Uses

### Blur Background

```
img{    filter:blur(3px);}
```

---

### Dark Hero Image

```
.hero img{    filter:brightness(60%);}
```

---

### Black & White Hover

```
img{    filter:grayscale(100%);}img:hover{    filter:grayscale(0%);}
```

---

### Transparent PNG Shadow

```
.logo{    filter:drop-shadow(0 4px 8px rgba(0,0,0,0.3));}
```

---

# Which Filters Are Used Most? ⭐⭐⭐⭐⭐

|Filter|Usage|
|---|---|
|brightness()|⭐⭐⭐⭐|
|grayscale()|⭐⭐⭐⭐|
|blur()|⭐⭐⭐|
|contrast()|⭐⭐⭐|
|drop-shadow()|⭐⭐⭐|
|invert()|⭐⭐|
|sepia()|⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Blur

```
filter:blur(5px);
```

---

### Brightness

```
filter:brightness(120%);
```

---

### Contrast

```
filter:contrast(150%);
```

---

### Grayscale

```
filter:grayscale(100%);
```

---

### Invert

```
filter:invert(100%);
```

---

### Sepia

```
filter:sepia(100%);
```

---

### Drop Shadow

```
filter:drop-shadow(2px 2px 5px gray);
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. brightness() ⭐⭐⭐⭐2. grayscale() ⭐⭐⭐⭐3. blur() ⭐⭐⭐4. contrast() ⭐⭐⭐5. drop-shadow() ⭐⭐⭐6. invert() ⭐⭐7. sepia() ⭐⭐
```

---

# 💡 Full Stack Tip

These are the filter effects you'll use most often:

### Hero Image

```
.hero img{    filter:brightness(70%);}
```

Makes text easier to read over an image.

---

### Gallery Hover

```
img{    filter:grayscale(100%);    transition:filter 0.3s ease;}img:hover{    filter:grayscale(0%);}
```

A popular portfolio and gallery effect.

---

### Transparent Logo

```
.logo{    filter:drop-shadow(0 3px 6px rgba(0,0,0,0.25));}
```

Adds a natural shadow around the visible shape of the logo.

> **Best Practice:** Filters can be computationally expensive, especially `blur()`. Use them sparingly and combine them with `transition` for smooth hover effects.

---

## 🚀 Filters Cheat Sheet

```
blur()brightness()contrast()grayscale()invert()sepia()drop-shadow()
```
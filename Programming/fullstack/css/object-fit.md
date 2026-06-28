> **Remember this:**
> 
> - **`background-size`** → Background Images
> - **`object-fit`** → HTML Images (`<img>`) & Videos (`<video>`)

---

# 22. Object Fit ⭐⭐

## What is Object Fit?

The `object-fit` property controls **how an image or video fits inside its container**.

Works with:

- `<img>`
- `<video>`

Syntax

```
object-fit:value;
```

Example

```
img{    width:300px;    height:200px;    object-fit:cover;}
```

---

# Why Use object-fit?

Without `object-fit`

❌ Images may stretch or look distorted.

With `object-fit`

✔ Images keep their aspect ratio.

✔ Images fit neatly inside containers.

---

# 1. object-fit ⭐⭐⭐⭐⭐

Controls how the image fills its container.

Common Values

```
fillcontaincovernonescale-down
```

---

## fill (Default)

Image stretches to fill the container.

```
object-fit:fill;
```

Characteristics

✔ Fills the container

❌ Image may become distorted

---

## contain ⭐⭐⭐⭐

Shows the **entire image**.

```
object-fit:contain;
```

Characteristics

✔ Entire image is visible

✔ Maintains aspect ratio

❌ May leave empty space

---

## cover ⭐⭐⭐⭐⭐

Fills the entire container.

```
object-fit:cover;
```

Characteristics

✔ Container completely filled

✔ Maintains aspect ratio

✔ Image may be cropped

⭐ **Most commonly used**

---

## none ⭐⭐

Keeps the image at its original size.

```
object-fit:none;
```

May overflow the container.

---

## scale-down ⭐⭐

Chooses the smaller result between `none` and `contain`.

```
object-fit:scale-down;
```

Rarely used.

---

# cover vs contain ⭐⭐⭐⭐⭐

|cover|contain|
|---|---|
|Fills container|Shows complete image|
|Crops image if needed|May leave empty space|
|Most commonly used|Used when full image must be visible|

---

# 2. object-position ⭐⭐⭐

Controls where the image is positioned inside its container.

Syntax

```
object-position:value;
```

Example

```
object-position:center;
```

Common Values

```
centertopbottomleftright
```

You can also use percentages.

```
object-position:50% 50%;
```

Or pixels.

```
object-position:20px 40px;
```

---

# Complete Example ⭐⭐⭐⭐⭐

```
img{width:300px;height:200px;object-fit:cover;object-position:center;}
```

Perfect for profile images and cards.

---

# Common Uses

### Profile Picture

```
img{    width:150px;    height:150px;    object-fit:cover;    border-radius:50%;}
```

---

### Product Card

```
img{    width:100%;    height:250px;    object-fit:cover;}
```

---

### Gallery

```
img{    width:100%;    height:200px;    object-fit:cover;}
```

---

# object-fit vs background-size ⭐⭐⭐⭐

|object-fit|background-size|
|---|---|
|`<img>` / `<video>`|Background images|
|Controls media element|Controls CSS background|
|Very common|Very common|

Example

```
img{    object-fit:cover;}
```

```
.hero{    background-size:cover;}
```

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|object-fit:cover|⭐⭐⭐⭐⭐|
|object-position:center|⭐⭐⭐⭐|
|object-fit:contain|⭐⭐⭐|
|object-fit:fill|⭐⭐|
|object-fit:none|⭐|
|object-fit:scale-down|⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Cover

```
object-fit:cover;
```

Fill container.

---

### Contain

```
object-fit:contain;
```

Show full image.

---

### Fill

```
object-fit:fill;
```

Stretch image.

---

### Position

```
object-position:center;
```

Center image.

---

### Top

```
object-position:top;
```

Align image to top.

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. object-fit:cover ⭐⭐⭐⭐⭐
2. object-position:center ⭐⭐⭐⭐
3. object-fit:contain ⭐⭐⭐
4. object-fit:fill ⭐⭐
5. object-fit:none ⭐
6. object-fit:scale-down ⭐
```

---

## 💡 Full Stack Tip

You'll use `object-fit: cover` in almost every modern project:

```
.card img{    width:100%;    height:250px;    object-fit:cover;}
```

For circular profile pictures:

```
.profile img{    width:120px;    height:120px;    border-radius:50%;    object-fit:cover;}
```

These patterns ensure images look clean and consistent without stretching or distortion.
> **emember this:**
> 
> - **Opacity** affects the **entire element**.
> - **RGBA / HSLA** affect only the **color**.

---

#  Opacity ⭐

## What is Opacity?

The `opacity` property controls the **transparency** of an entire element.

Syntax

```
opacity:value;
```

Range

```
0   → Completely Invisible0.5 → 50% Visible1   → Fully Visible (Default)
```

---

# 1. opacity ⭐⭐⭐⭐⭐

### Fully Visible

```
opacity:1;
```

(Default)

---

### Half Visible

```
opacity:0.5;
```

50% transparent.

---

### Invisible

```
opacity:0;
```

Element becomes invisible.

**Note:** The element is still present in the layout and can still receive pointer events unless you change other properties.

---

# Complete Example

```
.card{    opacity:0.8;}
```

---

# Hover Effect ⭐⭐⭐⭐⭐

One of the most common uses.

```
img{    opacity:0.7;}img:hover{    opacity:1;}
```

Creates a fade-in effect.

---

# Button Hover

```
button{    opacity:1;}button:hover{    opacity:0.8;}
```

Very common in websites.

---

# Opacity vs RGBA ⭐⭐⭐⭐⭐

### Opacity

```
opacity:0.5;
```

Everything becomes transparent.

✔ Text

✔ Images

✔ Border

✔ Background

---

### RGBA

```
background:rgba(0,0,0,0.5);
```

Only the **background color** becomes transparent.

Text stays fully visible.

---

# Opacity vs Visibility vs Display ⭐⭐⭐⭐⭐

|Property|Visible|Space|Clickable*|
|---|---|---|---|
|opacity:0|❌|✅|✅|
|visibility:hidden|❌|✅|❌|
|display:none|❌|❌|❌|

*By default. `opacity: 0` does not disable interactions; if needed, use `pointer-events: none;`.

---

# Common Uses

✔ Image Hover

✔ Card Hover

✔ Loading Screen

✔ Overlay

✔ Animations

✔ Disabled Effects

---

# Which Values Are Used Most? ⭐⭐⭐⭐⭐

|Value|Usage|
|---|---|
|opacity:1|⭐⭐⭐⭐⭐|
|opacity:0.8|⭐⭐⭐⭐|
|opacity:0.5|⭐⭐⭐⭐|
|opacity:0|⭐⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Visible

```
opacity:1;
```

---

### Half Transparent

```
opacity:0.5;
```

---

### Invisible

```
opacity:0;
```

---

### Hover Effect

```
img:hover{    opacity:0.8;}
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. opacity:1 ⭐⭐⭐⭐⭐2. opacity:0.8 ⭐⭐⭐⭐3. opacity:0.5 ⭐⭐⭐⭐4. opacity:0 ⭐⭐⭐
```

---

## 💡 Full Stack Tip

You'll use `opacity` mainly for hover effects and animations.

Image Hover

```
img{    opacity:0.8;    transition:0.3s;}img:hover{    opacity:1;}
```

Overlay

```
.overlay{    background:rgba(0,0,0,0.5);}
```

Notice that overlays usually use **`rgba()`** instead of `opacity`, because `opacity` would also make the text inside the overlay transparent.
# Gradients ⭐⭐

## What are Gradients?

A **gradient** is a smooth transition between two or more colors.

CSS supports **3 types**:

- Linear Gradient
- Radial Gradient
- Conic Gradient

Used for

- Hero Sections
- Buttons
- Cards
- Backgrounds
- Overlays

---

# Gradient Syntax

Gradients are usually used with the `background` or `background-image` property.

Example

```
background:linear-gradient(red, blue);
```

or

```
background-image:linear-gradient(red, blue);
```

---

# 1. Linear Gradient ⭐⭐⭐⭐⭐

Colors change in a **straight line**.

Syntax

```
linear-gradient(direction, color1, color2);
```

Basic Example

```
background:linear-gradient(red, blue);
```

Default Direction

Top → Bottom

---

## Direction

Left to Right

```
background:linear-gradient(to right, red, blue);
```

Right to Left

```
background:linear-gradient(to left, red, blue);
```

Top to Bottom

```
background:linear-gradient(to bottom, red, blue);
```

Bottom to Top

```
background:linear-gradient(to top, red, blue);
```

Using Degrees

```
background:linear-gradient(45deg, red, blue);
```

---

## Multiple Colors

```
background:linear-gradient(red, yellow, green);
```

---

# 2. Radial Gradient ⭐⭐⭐

Colors spread outward from the center.

Syntax

```
radial-gradient(color1, color2);
```

Example

```
background:radial-gradient(red, blue);
```

Result

```
      Blue   Blue BlueRed Red Red   Blue Blue      Blue
```

Common Shapes

Circle

```
background:radial-gradient(circle, red, blue);
```

Ellipse

```
background:radial-gradient(ellipse, red, blue);
```

---

# 3. Conic Gradient ⭐⭐

Colors rotate around a center point.

Syntax

```
conic-gradient(color1, color2);
```

Example

```
background:conic-gradient(red, yellow, green, blue);
```

Looks similar to a color wheel or pie chart.

Common Uses

- Pie Charts
- Circular Progress
- Decorative Backgrounds

---

# Linear vs Radial vs Conic ⭐⭐⭐⭐

|Gradient|Direction|Common Use|
|---|---|---|
|Linear|Straight line|Backgrounds, Buttons|
|Radial|Center outward|Highlights, Cards|
|Conic|Around center|Pie Charts, Decorative Effects|

---

# Common Examples

### Hero Section ⭐⭐⭐⭐⭐

```
.hero{    background:    linear-gradient(to right,#667eea,#764ba2);}
```

---

### Button

```
button{    background:    linear-gradient(to right,#ff512f,#dd2476);}
```

---

### Card Background

```
.card{    background:    linear-gradient(135deg,#74ebd5,#9face6);}
```

---

### Circular Background

```
.circle{    background:    radial-gradient(circle,#ffffff,#3498db);}
```

---

# Which Gradients Are Used Most? ⭐⭐⭐⭐⭐

|Gradient|Usage|
|---|---|
|Linear|⭐⭐⭐⭐⭐|
|Radial|⭐⭐⭐|
|Conic|⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Linear

```
background:linear-gradient(red, blue);
```

---

### Left to Right

```
background:linear-gradient(to right, red, blue);
```

---

### 45 Degrees

```
background:linear-gradient(45deg, red, blue);
```

---

### Radial

```
background:radial-gradient(red, blue);
```

---

### Conic

```
background:conic-gradient(red, yellow, green, blue);
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. linear-gradient() ⭐⭐⭐⭐⭐2. linear-gradient(to right, ...) ⭐⭐⭐⭐⭐3. linear-gradient(45deg, ...) ⭐⭐⭐⭐4. radial-gradient() ⭐⭐⭐5. conic-gradient() ⭐⭐
```

---

## 💡 Full Stack Tip

The vast majority of modern websites primarily use **Linear Gradients**.

### Hero Section

```
.hero{    background:    linear-gradient(to right,#4facfe,#00f2fe);}
```

---

### Button

```
button{    background:    linear-gradient(135deg,#ff416c,#ff4b2b);}
```

---

### Overlay

```
.overlay{    background:    linear-gradient(        rgba(0,0,0,0.7),        rgba(0,0,0,0.3)    );}
```

This creates a transparent overlay on top of an image while keeping text readable.

---
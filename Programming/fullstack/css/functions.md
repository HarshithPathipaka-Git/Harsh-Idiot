> **⭐ Interview Question**
> 
> **Why use CSS functions?**
> 
> They allow CSS values to be calculated or adjusted automatically based on available space or defined limits.

---

# 33. Functions ⭐⭐

## What are CSS Functions?

CSS Functions perform calculations or return values that CSS can use.

Common Functions

- `calc()`
- `min()`
- `max()`
- `clamp()`

Used for

- Responsive Layouts
- Dynamic Sizing
- Responsive Typography
- Flexible Spacing

---

# 1. calc() ⭐⭐⭐⭐⭐

Performs mathematical calculations.

Syntax

```
calc(expression)
```

Supports

```
+-*/
```

---

## Example

```
width:calc(100% - 50px);
```

Meaning

```
Element Width=100%-50px
```

---

## More Examples

Height

```
height:calc(100vh - 80px);
```

Useful for layouts with a fixed header.

Margin

```
margin-left:calc(2rem + 10px);
```

---

# Common Uses ⭐⭐⭐⭐⭐

```
.main{height:calc(100vh - 70px);}
```

Perfect for full-page layouts.

---

# 2. min() ⭐⭐⭐

Returns the **smallest** value.

Syntax

```
min(value1,value2);
```

Example

```
width:min(500px,90%);
```

Meaning

```
Use the smaller value.
```

Useful for responsive containers.

---

# 3. max() ⭐⭐⭐

Returns the **largest** value.

Syntax

```
max(value1,value2);
```

Example

```
width:max(300px,50%);
```

Meaning

```
Use the larger value.
```

Useful for setting minimum sizes.

---

# 4. clamp() ⭐⭐⭐⭐⭐

Keeps a value between a **minimum** and **maximum**.

Syntax

```
clamp(min, preferred, max)
```

Example

```
font-size:clamp(16px,2vw,32px);
```

Meaning

```
Minimum↓16px↓Preferred↓2vw↓Maximum↓32px
```

Font size grows with the screen but never becomes smaller than **16px** or larger than **32px**.

---

# Why clamp() is Amazing ⭐⭐⭐⭐⭐

Without `clamp()`

```
font-size:16px;@media(...){font-size:24px;}
```

With `clamp()`

```
font-size:clamp(16px,2vw,24px);
```

No media query needed.

---

# calc() vs min() vs max() vs clamp() ⭐⭐⭐⭐⭐

|Function|Purpose|
|---|---|
|`calc()`|Calculate values|
|`min()`|Choose the smaller value|
|`max()`|Choose the larger value|
|`clamp()`|Keep value between min & max|

---

# Common Uses

### Full Height Layout

```
height:calc(100vh - 80px);
```

---

### Responsive Width

```
width:min(1200px,90%);
```

---

### Minimum Width

```
width:max(300px,40%);
```

---

### Responsive Font

```
font-size:clamp(16px,2vw,32px);
```

---

# Which Functions Are Used Most? ⭐⭐⭐⭐⭐

|Function|Usage|
|---|---|
|`calc()`|⭐⭐⭐⭐⭐|
|`clamp()`|⭐⭐⭐⭐⭐|
|`min()`|⭐⭐⭐|
|`max()`|⭐⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Calculate

```
width:calc(100% - 20px);
```

---

### Minimum

```
width:min(500px,90%);
```

---

### Maximum

```
width:max(300px,40%);
```

---

### Clamp

```
font-size:clamp(16px,2vw,32px);
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. calc() ⭐⭐⭐⭐⭐2. clamp() ⭐⭐⭐⭐⭐3. min() ⭐⭐⭐4. max() ⭐⭐⭐
```

---

# 💡 Full Stack Tip

These are the function patterns you'll use most often:

### Full Page Content

```
.main{    height:calc(100vh - 70px);}
```

Subtracts the header height from the viewport height.

---

### Responsive Container

```
.container{    width:min(1200px,90%);}
```

Keeps the container responsive while limiting its maximum width.

---

### Responsive Typography

```
h1{    font-size:clamp(2rem,5vw,4rem);}
```

The font scales smoothly across screen sizes without media queries.

> **Best Practice:** For modern responsive design, **`clamp()`** is increasingly preferred for typography and spacing because it reduces the need for multiple media queries.

---

## 🚀 Functions Cheat Sheet

```
calc()
min()
max()
clamp()
```
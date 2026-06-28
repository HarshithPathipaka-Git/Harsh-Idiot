> **💡 Full Stack Tip**
> 
> Learn `float` and `clear` so you can **read and maintain older code**, not because you'll use them often in new projects.

---

# Float & Clear ⭐

## What is Float?

The `float` property moves an element to the **left or right** of its container, allowing surrounding content to wrap around it.

Originally designed for wrapping text around images.

Syntax

```
float: value;
```

Common Values

```
leftrightnone
```

---

# 1. float: left ⭐⭐⭐

Moves the element to the **left**.

Example

```
img{    float:left;}
```

Output

```
[Image]  Text continues here...
```

The text wraps around the image.

---

# 2. float: right ⭐⭐⭐

Moves the element to the **right**.

Example

```
img{    float:right;}
```

Output

```
Text continues here...   [Image]
```

---

# 3. float: none ⭐⭐

Default value.

The element behaves normally.

```
float:none;
```

---

# What Happens After Float?

Floated elements are **taken out of the normal document flow**.

This means nearby elements may move up or wrap around them.

Example

```
<div class="box1"></div><div class="box2"></div>
```

```
.box1{    float:left;}
```

`box2` may move beside or around `box1` instead of starting below it.

---

# What is Clear?

The `clear` property prevents an element from sitting next to floated elements.

Syntax

```
clear: value;
```

Common Values

```
leftrightbothnone
```

---

# 1. clear: left

Moves the element below left-floated elements.

```
clear:left;
```

---

# 2. clear: right

Moves the element below right-floated elements.

```
clear:right;
```

---

# 3. clear: both ⭐⭐⭐

Clears both left and right floats.

```
clear:both;
```

Most commonly used.

Example

```
.footer{    clear:both;}
```

The footer appears below all floated elements.

---

# Float vs Flexbox ⭐⭐⭐⭐⭐

|Float|Flexbox|
|---|---|
|Older layout method|Modern layout|
|Difficult to manage|Easy to manage|
|Limited control|Powerful alignment|
|Used mainly for text wrapping|Used for page layouts|

---

# Common Uses Today

✔ Wrap text around images

✔ Reading old code

✔ Legacy websites

❌ Not recommended for modern layouts

Instead use

```
display:flex;
```

or

```
display:grid;
```

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|float:left|⭐⭐⭐|
|clear:both|⭐⭐⭐|
|float:right|⭐⭐|
|float:none|⭐⭐|
|clear:left/right|⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Float Left

```
float:left;
```

Moves element to the left.

---

### Float Right

```
float:right;
```

Moves element to the right.

---

### Float None

```
float:none;
```

Default behavior.

---

### Clear Both

```
clear:both;
```

Moves the element below floated elements.

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. clear:both ⭐⭐⭐2. float:left ⭐⭐⭐3. float:right ⭐⭐4. float:none ⭐⭐
```

---

## 💡 Full Stack Tip

In **modern frontend development**, if you want elements side by side, don't use `float`.

❌ Old way

```
.left{    float:left;}.right{    float:right;}
```

✅ Modern way

```
.container{    display:flex;    justify-content:space-between;}
```

You'll use **Flexbox** for about **90% of layouts** and **Grid** for more complex two-dimensional layouts.

---
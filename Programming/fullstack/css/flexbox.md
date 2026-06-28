> **⭐ Interview Question**
> 
> "Explain Flexbox and its main properties."
> 
> This is one of the most common CSS interview questions.

---

# 17. Flexbox ⭐⭐⭐⭐⭐

## What is Flexbox?

**Flexbox (Flexible Box Layout)** is a **one-dimensional layout system** used to arrange items in a **row or column**.

It makes it easy to:

- Center elements
- Create responsive layouts
- Align items
- Distribute space
- Build navigation bars, cards, forms, etc.

---

# Important Terms ⭐⭐⭐⭐⭐

```
Flex Container        ↓display:flex;↓Flex Items(All direct children)
```

Example

```
<div class="container">    
<div>1</div>    
<div>2</div>    
<div>3</div>
</div>
```

```
.container{    display:flex;}
```

Here

```
.container → Flex Container1,2,3 → Flex Items
```

---

# Main Axis & Cross Axis ⭐⭐⭐⭐⭐

Before learning Flexbox properties, remember these two axes.

```
Default (flex-direction: row)

Main Axis  → → →

+----+----+----+
| 1  | 2  | 3  |
+----+----+----+

Cross Axis
     ↓
```

If `flex-direction: column`

```
Cross Axis →

+----+
| 1  |
+----+
| 2  |
+----+
| 3  |
+----+

Main Axis
    ↓
```

**Remember:**

- **Main Axis** → Controlled by `flex-direction`
- **Cross Axis** → Perpendicular to the Main Axis

---

# 1. display:flex ⭐⭐⭐⭐⭐

Turns an element into a Flex Container.

```
.container{    display:flex;}
```

Children automatically become Flex Items.

---

# 2. flex-direction ⭐⭐⭐⭐⭐

Controls the direction of Flex Items.

```
flex-direction: row;
```

Values

```
rowrow-reversecolumncolumn-reverse
```

Example

```
.container{    display:flex;    flex-direction:column;}
```

---

# 3. flex-wrap ⭐⭐⭐⭐

Controls whether items wrap to the next line.

Values

```
flex-wrap:nowrap;flex-wrap:wrap;flex-wrap:wrap-reverse;
```

Example

```
.container{    display:flex;    flex-wrap:wrap;}
```

Useful for responsive layouts.

---

# 4. flex-flow ⭐⭐⭐

Shorthand for

- flex-direction
- flex-wrap

Instead of

```
flex-direction:row;flex-wrap:wrap;
```

Use

```
flex-flow:row wrap;
```

---

# 5. justify-content ⭐⭐⭐⭐⭐

Aligns items along the **Main Axis**.

Values

```
justify-content:flex-start;
justify-content:center;
justify-content:flex-end;
justify-content:space-between;
justify-content:space-around;
justify-content:space-evenly;
```

Common Uses

```
justify-content:center;
```

Centers items.

```
justify-content:space-between;
```

Perfect for navigation bars.

---

# 6. align-items ⭐⭐⭐⭐⭐

Aligns items along the **Cross Axis**.

Values

```
align-items:flex-start;
align-items:center;
align-items:flex-end;
align-items:stretch;
align-items:baseline;
```

Example

```
align-items:center;
```

Centers items vertically (in a row layout).

---

# justify-content vs align-items ⭐⭐⭐⭐⭐

|justify-content|align-items|
|---|---|
|Main Axis|Cross Axis|
|Horizontal (default row)|Vertical (default row)|

---

# Center Everything ⭐⭐⭐⭐⭐

```
.container{    display:flex;    justify-content:center;    align-items:center;}
```

This is one of the most used Flexbox patterns.

---

# 7. align-content ⭐⭐⭐

Works **only when there are multiple rows or columns** (i.e., with wrapping).

Example

```
align-content:center;
```

Common Values

```
flex-start
center
flex-end
space-between
space-around
stretch
```

Rarely needed for single-line layouts.

---

# 8. gap ⭐⭐⭐⭐⭐

Adds space between Flex Items.

Example

```
gap:20px;
```

Instead of adding margins to each item.

You can also use

```
row-gap:20px;
column-gap:10px;
```

---

# 9. order ⭐⭐⭐

Changes the visual order of Flex Items.

Example

```
.item1{    order:2;}
.item2{    order:1;}
```

The item with the smaller order appears first.

Default

```
order:0;
```

---

# 10. flex-grow ⭐⭐⭐⭐

Controls how much an item grows.

Example

```
.item{    flex-grow:1;}
```

Example

```
.item1{    flex-grow:1;}.item2{    flex-grow:2;}
```

`item2` gets twice as much extra space.

---

# 11. flex-shrink ⭐⭐⭐

Controls how much an item shrinks.

Example

```
flex-shrink:1;
```

Prevent shrinking

```
flex-shrink:0;
```

Useful for logos and fixed-size elements.

---

# 12. flex-basis ⭐⭐⭐

Defines the initial size of a Flex Item.

Example

```
flex-basis:200px;
```

Often used instead of `width` in Flexbox.

---

# 13. align-self ⭐⭐⭐

Overrides `align-items` for a single item.

Example

```
.container{    align-items:center;}.item{    align-self:flex-start;}
```

Only that item changes alignment.

---

# Flex Shorthand ⭐⭐⭐⭐

Instead of

```
flex-grow:1;flex-shrink:1;flex-basis:200px;
```

Use

```
flex:1 1 200px;
```

Syntax

```
flex: grow shrink basis;
```

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|display:flex|⭐⭐⭐⭐⭐|
|justify-content|⭐⭐⭐⭐⭐|
|align-items|⭐⭐⭐⭐⭐|
|flex-direction|⭐⭐⭐⭐⭐|
|gap|⭐⭐⭐⭐⭐|
|flex-wrap|⭐⭐⭐⭐|
|flex-grow|⭐⭐⭐⭐|
|flex-basis|⭐⭐⭐|
|align-self|⭐⭐⭐|
|order|⭐⭐⭐|
|flex-shrink|⭐⭐|
|align-content|⭐⭐|
|flex-flow|⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Flex Container

```
display:flex;
```

---

### Direction

```
flex-direction:row;
```

---

### Wrap

```
flex-wrap:wrap;
```

---

### Main Axis

```
justify-content:center;
```

---

### Cross Axis

```
align-items:center;
```

---

### Gap

```
gap:20px;
```

---

### Grow

```
flex-grow:1;
```

---

### Basis

```
flex-basis:200px;
```

---

### Individual Alignment

```
align-self:center;
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. display:flex ⭐⭐⭐⭐⭐
2. justify-content ⭐⭐⭐⭐⭐
3. align-items ⭐⭐⭐⭐⭐
4. gap ⭐⭐⭐⭐⭐
5. flex-direction ⭐⭐⭐⭐⭐
6. flex-wrap ⭐⭐⭐⭐
7. flex-grow ⭐⭐⭐⭐
8. order ⭐⭐⭐
9. align-self ⭐⭐⭐
10. flex-basis ⭐⭐⭐
11. align-content ⭐⭐
12. flex-shrink ⭐⭐
13. flex-flow ⭐⭐
```

---

# 💡 Full Stack Tip

You'll use these Flexbox patterns almost every day:

### Center an Element

```
.container{    display:flex;    justify-content:center;    align-items:center;}
```

---

### Navbar

```
.nav{    display:flex;    justify-content:space-between;    align-items:center;}
```

---

### Responsive Card Layout

```
.cards{    display:flex;    flex-wrap:wrap;    gap:20px;}
```

---

### Equal Width Columns

```
.item{    flex:1;}
```

---

## 🚀 Flexbox Cheat Sheet (Remember These 5)

```
display:flex;              → Enable 
Flexboxflex-direction             → Row / Columnjustify-content            → Main
Axisalign-items                → Cross Axis
gap                        → Space Between Items
```

If you remember just these five properties, you'll already be able to build most Flexbox layouts.
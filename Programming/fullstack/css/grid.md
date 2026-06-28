> **Remember this forever:**
> 
> - **Flexbox = 1D Layout** (Row **or** Column)
> - **Grid = 2D Layout** (Rows **and** Columns)

Grid is perfect for dashboards, galleries, portfolios, admin panels, and complex page layouts.

---

# Grid ⭐⭐⭐⭐⭐

## What is CSS Grid?

**CSS Grid** is a **two-dimensional layout system** that arranges elements into **rows and columns**.

It makes complex layouts simple.

Used for

- Dashboards
- Galleries
- Cards
- Portfolios
- Admin Panels
- Website Layouts

---

# Important Terms ⭐⭐⭐⭐⭐

```
Grid Container       ↓display:grid;↓Grid Items(All direct children)
```

Example

```
<div class="container">    <div>1</div>    <div>2</div>    <div>3</div></div>
```

```
.container{    display:grid;}
```

Here

```
.container → Grid Container1,2,3 → Grid Items
```

---

# Rows & Columns ⭐⭐⭐⭐⭐

Grid creates

```
Columns↓+----+----+----+Rows → | 1 | 2 | 3 |+----+----+----+| 4 | 5 | 6 |+----+----+----+
```

Unlike Flexbox, Grid controls **both directions**.

---

# 1. display:grid ⭐⭐⭐⭐⭐

Turns an element into a Grid Container.

```
.container{    display:grid;}
```

Children become Grid Items.

---

# 2. Rows ⭐⭐⭐⭐

Create rows using

```
grid-template-rows
```

Example

```
grid-template-rows:100px 200px;
```

Creates

```
Row 1 → 100pxRow 2 → 200px
```

---

# 3. Columns ⭐⭐⭐⭐⭐

Create columns using

```
grid-template-columns
```

Example

```
grid-template-columns:1fr 1fr 1fr;
```

Creates

```
3 Equal Columns
```

Another Example

```
grid-template-columns:200px 1fr;
```

Creates

```
Sidebar | Content
```

---

# 4. gap ⭐⭐⭐⭐⭐

Adds spacing between Grid Items.

Example

```
gap:20px;
```

Separate Values

```
row-gap:20px;column-gap:10px;
```

---

# 5. repeat() ⭐⭐⭐⭐⭐

Avoids writing the same value multiple times.

Instead of

```
grid-template-columns:1fr 1fr 1fr;
```

Use

```
grid-template-columns:repeat(3,1fr);
```

Syntax

```
repeat(number,size)
```

---

# 6. minmax() ⭐⭐⭐⭐

Sets both minimum and maximum sizes.

Syntax

```
minmax(min,max)
```

Example

```
grid-template-columns:minmax(200px,1fr);
```

Meaning

```
Minimum = 200pxMaximum = Remaining Space
```

Useful for responsive layouts.

---

# 7. grid-area ⭐⭐⭐

Places an item in a specific grid area.

Example

```
.item{    grid-area:1 / 1 / 2 / 3;}
```

Meaning

```
Row StartColumn StartRow EndColumn End
```

Can also be used with named grid areas.

---

# 8. grid-template ⭐⭐⭐

Shorthand for

- grid-template-rows
- grid-template-columns
- grid-template-areas

Example

```
grid-template:100px auto /200px 1fr;
```

Less commonly used.

---

# 9. auto-fit ⭐⭐⭐⭐

Automatically fits as many columns as possible.

Example

```
grid-template-columns:repeat(auto-fit,minmax(250px,1fr));
```

If extra space exists

✔ Columns expand.

Best for responsive layouts.

---

# 10. auto-fill ⭐⭐⭐

Also creates responsive columns.

Example

```
grid-template-columns:repeat(auto-fill,minmax(250px,1fr));
```

Difference

- Keeps empty columns if space is available.

---

# auto-fit vs auto-fill ⭐⭐⭐⭐

|auto-fit|auto-fill|
|---|---|
|Expands existing columns|Keeps empty columns|
|Most commonly used|Less common|

---

# 11. place-items ⭐⭐⭐⭐

Shorthand for

```
align-itemsjustify-items
```

Example

```
place-items:center;
```

Centers every Grid Item.

---

# 12. place-content ⭐⭐⭐

Shorthand for

```
align-contentjustify-content
```

Example

```
place-content:center;
```

Centers the entire Grid.

---

# Grid Example ⭐⭐⭐⭐⭐

```
.container{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;}
```

Creates

```
+-----+-----+-----+| 1 | 2 | 3 |+-----+-----+-----+| 4 | 5 | 6 |+-----+-----+-----+
```

---

# Flexbox vs Grid ⭐⭐⭐⭐⭐

|Flexbox|Grid|
|---|---|
|1D Layout|2D Layout|
|Row OR Column|Rows AND Columns|
|Navigation|Page Layout|
|Cards|Dashboards|
|Components|Entire Sections|

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|display:grid|⭐⭐⭐⭐⭐|
|grid-template-columns|⭐⭐⭐⭐⭐|
|gap|⭐⭐⭐⭐⭐|
|repeat()|⭐⭐⭐⭐⭐|
|minmax()|⭐⭐⭐⭐|
|auto-fit|⭐⭐⭐⭐|
|grid-template-rows|⭐⭐⭐|
|place-items|⭐⭐⭐|
|auto-fill|⭐⭐⭐|
|grid-area|⭐⭐⭐|
|place-content|⭐⭐|
|grid-template|⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Grid Container

```
display:grid;
```

---

### Rows

```
grid-template-rows:100px auto;
```

---

### Columns

```
grid-template-columns:repeat(3,1fr);
```

---

### Gap

```
gap:20px;
```

---

### Repeat

```
repeat(3,1fr);
```

---

### Min Max

```
minmax(200px,1fr);
```

---

### Responsive Grid

```
repeat(auto-fit,minmax(250px,1fr));
```

---

### Place Items

```
place-items:center;
```

---

### Grid Area

```
grid-area:1 / 1 / 2 / 3;
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. display:grid ⭐⭐⭐⭐⭐2. grid-template-columns ⭐⭐⭐⭐⭐3. gap ⭐⭐⭐⭐⭐4. repeat() ⭐⭐⭐⭐⭐5. auto-fit ⭐⭐⭐⭐6. minmax() ⭐⭐⭐⭐7. grid-template-rows ⭐⭐⭐8. place-items ⭐⭐⭐9. grid-area ⭐⭐⭐10. auto-fill ⭐⭐⭐11. place-content ⭐⭐12. grid-template ⭐⭐
```

---

# 💡 Full Stack Tip

These are the Grid patterns you'll use most often:

### Equal Columns

```
.container{    display:grid;    grid-template-columns:repeat(3,1fr);    gap:20px;}
```

---

### Responsive Card Grid ⭐⭐⭐⭐⭐

```
.container{    display:grid;    grid-template-columns:    repeat(auto-fit,minmax(250px,1fr));    gap:20px;}
```

This is one of the **most common Grid layouts** in modern websites. It automatically adjusts the number of columns based on the available screen width.

---

### Center Items

```
.container{    display:grid;    place-items:center;}
```

---

# 🚀 Grid Cheat Sheet (Remember These 5)

```
display:gridgrid-template-columnsgaprepeat()repeat(auto-fit,minmax(250px,1fr))
```

If you remember these five concepts, you'll be able to build most Grid layouts you'll encounter in real-world frontend development.
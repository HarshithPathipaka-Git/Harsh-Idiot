> **Remember this forever:**
> 
> - **`visibility: hidden`** → Hidden **but keeps its space**
> - **`display: none`** → Hidden **and removes its space**

---

# 23. Visibility ⭐

## What is Visibility?

The `visibility` property controls **whether an element is visible or hidden** without changing the page layout.

Syntax

```
visibility:value;
```

Common Values

```
visiblehiddencollapse
```

---

# 1. visibility: visible ⭐⭐⭐

Default value.

The element is visible.

```
visibility:visible;
```

Example

```
.box{    visibility:visible;}
```

---

# 2. visibility: hidden ⭐⭐⭐⭐⭐

Hides the element but **keeps its space**.

```
visibility:hidden;
```

Characteristics

✔ Element is hidden

✔ Space is still reserved

✔ Layout doesn't change

Example

```
.box{    visibility:hidden;}
```

Output

```
[ Hidden Space ]Next Element
```

---

# 3. visibility: collapse ⭐

Used mainly for table rows and columns.

```
visibility:collapse;
```

Mostly works with

```
<tr><td><col>
```

Rarely used.

---

# visibility vs display ⭐⭐⭐⭐⭐

|visibility:hidden|display:none|
|---|---|
|Hidden|Hidden|
|Space remains|Space removed|
|Element still occupies layout|Element removed from layout|

Example

```
visibility:hidden;
```

```
[ Empty Space ]Next Element
```

---

```
display:none;
```

```
Next Element
```

(No empty space)

---

# Common Uses

### Hide Element (Keep Space)

```
visibility:hidden;
```

Useful for

- Hover effects
- Animations
- Temporary hiding

---

### Remove Element Completely

```
display:none;
```

Useful for

- Menus
- Modals
- Popups
- Tabs

---

# Which Property Should I Use?

|Situation|Property|
|---|---|
|Hide but keep layout|visibility:hidden|
|Remove completely|display:none|

---

# Which Values Are Used Most? ⭐⭐⭐⭐⭐

|Value|Usage|
|---|---|
|hidden|⭐⭐⭐⭐⭐|
|visible|⭐⭐⭐|
|collapse|⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Visible

```
visibility:visible;
```

Show element.

---

### Hidden

```
visibility:hidden;
```

Hide but keep space.

---

### Collapse

```
visibility:collapse;
```

Mainly for tables.

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. visibility:hidden ⭐⭐⭐⭐⭐
2. visibility:visible ⭐⭐⭐
3. visibility:collapse ⭐
```

---

## 💡 Full Stack Tip

This is the most common interview comparison:

```
visibility:hidden;
```

✔ Element is invisible.

✔ Layout space remains.

---

```
display:none;
```

✔ Element is invisible.

✔ Layout space is removed.

This difference is frequently tested in interviews and appears in real projects when showing or hiding UI elements.
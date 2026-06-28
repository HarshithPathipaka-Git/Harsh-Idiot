> **⭐ Interview Question**
> 
> **Difference between Pseudo Class and Pseudo Element?**
> 
> - **Pseudo Class (`:`)** → Styles an existing element in a specific **state** (`:hover`, `:focus`).
> - **Pseudo Element (`::`)** → Styles or creates a specific **part** of an element (`::before`, `::after`).

---

# 34. Pseudo Classes ⭐⭐⭐

## What are Pseudo Classes?

A **Pseudo Class** selects an element based on its **state**, **interaction**, or **position**.

Syntax

```
selector:pseudo-class{}
```

Example

```
button:hover{    background:blue;}
```

---

# Common Pseudo Classes

```
:hover:focus:active:visited:checked:disabled:nth-child():not()
```

---

# 1. :hover ⭐⭐⭐⭐⭐

Applies styles when the mouse pointer is over an element.

Example

```
button:hover{    background:blue;}
```

Common Uses

- Buttons
- Cards
- Images
- Links

Example

```
.card:hover{    transform:translateY(-5px);}
```

---

# 2. :focus ⭐⭐⭐⭐⭐

Applies styles when an element receives keyboard or mouse focus.

Commonly used with

- `<input>`
- `<textarea>`
- `<button>`
- `<select>`

Example

```
input:focus{    border-color:blue;}
```

Common Use

```
input:focus{    outline:none;}
```

> **Best Practice:** If you remove the default outline, provide another visible focus style (such as a custom border or box-shadow) so keyboard users can still see which element is focused.

---

# 3. :active ⭐⭐⭐

Applies while the element is being clicked or pressed.

Example

```
button:active{    transform:scale(0.95);}
```

Creates a button press effect.

---

# 4. :visited ⭐⭐⭐

Styles links that the user has already visited.

Example

```
a:visited{    color:purple;}
```

Works only with links.

---

# 5. :checked ⭐⭐⭐⭐

Styles checked form controls.

Works with

- Checkbox
- Radio Button

Example

```
input:checked{    accent-color:green;}
```

Common Uses

- Custom Checkboxes
- Toggle Switches

---

# 6. :disabled ⭐⭐⭐⭐

Styles disabled form controls.

Example

```
button:disabled{    opacity:0.5;    cursor:not-allowed;}
```

Common Uses

- Disabled Buttons
- Disabled Inputs

---

# 7. :nth-child() ⭐⭐⭐⭐

Selects elements based on their position.

Syntax

```
:nth-child(number)
```

Example

```
li:nth-child(2){    color:red;}
```

Second item becomes red.

---

## Odd Rows

```
tr:nth-child(odd){    background:#eee;}
```

---

## Even Rows

```
tr:nth-child(even){    background:#fff;}
```

Very common for tables.

---

# 8. :not() ⭐⭐⭐⭐

Selects everything **except** the specified selector.

Syntax

```
:not(selector)
```

Example

```
button:not(.primary){    background:gray;}
```

Meaning

Style every button except `.primary`.

---

# Common Combinations ⭐⭐⭐⭐

Hover + Transition

```
button{    transition:0.3s;}button:hover{    background:blue;}
```

---

Focus + Border

```
input:focus{    border-color:#2563eb;}
```

---

Disabled Button

```
button:disabled{    cursor:not-allowed;    opacity:0.5;}
```

---

# Which Pseudo Classes Are Used Most? ⭐⭐⭐⭐⭐

|Pseudo Class|Usage|
|---|---|
|:hover|⭐⭐⭐⭐⭐|
|:focus|⭐⭐⭐⭐⭐|
|:checked|⭐⭐⭐⭐|
|:disabled|⭐⭐⭐⭐|
|:nth-child()|⭐⭐⭐⭐|
|:active|⭐⭐⭐|
|:not()|⭐⭐⭐|
|:visited|⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Hover

```
button:hover{background:blue;}
```

---

### Focus

```
input:focus{border-color:blue;}
```

---

### Active

```
button:active{transform:scale(0.95);}
```

---

### Checked

```
input:checked{accent-color:green;}
```

---

### Disabled

```
button:disabled{opacity:0.5;}
```

---

### nth-child

```
li:nth-child(2){color:red;}
```

---

### Not

```
button:not(.primary){background:gray;}
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. :hover ⭐⭐⭐⭐⭐2. :focus ⭐⭐⭐⭐⭐3. :checked ⭐⭐⭐⭐4. :disabled ⭐⭐⭐⭐5. :nth-child() ⭐⭐⭐⭐6. :active ⭐⭐⭐7. :not() ⭐⭐⭐8. :visited ⭐⭐
```

---

# 💡 Full Stack Tip

These pseudo classes appear in almost every frontend project:

### Button Hover

```
button:hover{    background:#2563eb;}
```

---

### Input Focus

```
input:focus{    border-color:#2563eb;    box-shadow:0 0 5px rgba(37,99,235,0.3);}
```

---

### Disabled Button

```
button:disabled{    opacity:0.5;    cursor:not-allowed;}
```

---

### Zebra Table Rows

```
tr:nth-child(even){    background:#f5f5f5;}
```

Very common in dashboards and admin panels.

---

## 🚀 Pseudo Classes Cheat Sheet

```
:hover
:focus
:active
:visited
:checked
:disabled
:nth-child()
:not()
```
# Border ⭐⭐⭐

## What is Border?

A **border** is a line drawn around an HTML element.

Used for

- Buttons
- Cards
- Images
- Forms
- Tables
- Containers

Example

```
div{    border:2px solid black;}
```

---

# Border Structure ⭐⭐⭐⭐⭐

A border has **3 main parts**.

```
Border = Width + Style + Color
```

Example

```
border:2px solid red;
```

```
2px   → Widthsolid → Stylered   → Color
```

---

# 1. border ⭐⭐⭐⭐⭐

The shorthand property for adding a border.

Syntax

```
border: width style color;
```

Example

```
border:2px solid black;
```

Another Example

```
button{    border:3px dashed blue;}
```

Most Common

```
border:1px solid #ccc;
```

---

# 2. border-width ⭐⭐⭐

Controls the thickness of the border.

Example

```
border-width:2px;
```

Different Widths

```
border-width:1px;border-width:5px;
```

Individual Sides

```
border-top-width:2px;border-right-width:3px;border-bottom-width:4px;border-left-width:5px;
```

---

# 3. border-style ⭐⭐⭐

Defines the border style.

Common Values

```
border-style:solid;border-style:dashed;border-style:dotted;border-style:double;border-style:none;
```

### Common Styles

|Value|Result|
|---|---|
|solid|Solid line|
|dashed|Dashed line|
|dotted|Dotted line|
|double|Double line|
|none|No border|

**Most projects use `solid`.**

---

# 4. border-color ⭐⭐⭐

Sets the border color.

Example

```
border-color:red;
```

Using HEX

```
border-color:#3498db;
```

Using RGB

```
border-color:rgb(255,0,0);
```

Individual Sides

```
border-top-color:red;border-right-color:blue;border-bottom-color:green;border-left-color:black;
```

---

# 5. border-radius ⭐⭐⭐⭐⭐

Creates rounded corners.

Example

```
border-radius:10px;
```

Circle

```
border-radius:50%;
```

Useful for

- Buttons
- Cards
- Profile Images
- Avatars

Different Corners

```
border-top-left-radius:10px;border-top-right-radius:20px;border-bottom-left-radius:30px;border-bottom-right-radius:40px;
```

---

# 6. outline ⭐⭐⭐

Adds an outline outside the border.

Example

```
outline:2px solid blue;
```

Difference

```
border
```

Takes up space.

```
outline
```

Does **not** take up space.

Mostly used for

- Input fields
- Focus effects
- Accessibility

Example

```
input:focus{    outline:2px solid blue;}
```

---

# Border vs Outline ⭐⭐⭐⭐

|Border|Outline|
|---|---|
|Around element|Outside border|
|Takes space|Doesn't take space|
|Part of box model|Not part of box model|
|Used everywhere|Mostly for focus states|

---

# Border Shorthand ⭐⭐⭐⭐

Instead of

```
border-width:2px;border-style:solid;border-color:black;
```

Use

```
border:2px solid black;
```

✔ Cleaner

✔ Easier

✔ Professional

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|border|⭐⭐⭐⭐⭐|
|border-radius|⭐⭐⭐⭐⭐|
|border-style|⭐⭐⭐|
|border-width|⭐⭐⭐|
|border-color|⭐⭐⭐|
|outline|⭐⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Border

```
border:2px solid black;
```

---

### Border Width

```
border-width:2px;
```

---

### Border Style

```
border-style:solid;
```

---

### Border Color

```
border-color:red;
```

---

### Border Radius

```
border-radius:10px;
```

Circle

```
border-radius:50%;
```

---

### Outline

```
outline:2px solid blue;
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. border ⭐⭐⭐⭐⭐2. border-radius ⭐⭐⭐⭐⭐3. outline ⭐⭐⭐⭐ (Forms & Accessibility)4. border-color ⭐⭐⭐5. border-style ⭐⭐⭐6. border-width ⭐⭐⭐
```

---

## 💡 Full Stack Tip

In real-world frontend development, you'll use these most often:

```
border:1px solid #ddd;border-radius:8px;outline:none;
```

These three properties alone are used in **buttons, cards, forms, navigation bars, modals, images, and containers** across almost every website.

**⚠️ Best Practice:** Avoid removing outlines (`outline: none;`) unless you replace them with a visible focus style, otherwise keyboard users may not know which element is focused.

Example:

```
button:focus{    outline:2px solid blue;}
```
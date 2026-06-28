
## What are Selectors?

A **CSS Selector** is used to **select HTML elements** so CSS can style them.

**Syntax**

```
selector{    property: value;}
```

Example

```
h1{    color: blue;}
```

Here,

- `h1` → Selector
- `color` → Property
- `blue` → Value

---

# 1. Universal Selector (`*`) ⭐⭐

Selects **every element** on the page.

```
*{    margin: 0;    padding: 0;}
```

Example

```
<h1>Hello</h1><p>World</p>
```

Both `<h1>` and `<p>` are selected.

### Common Uses

- CSS Reset
- Remove default spacing
- Apply global styles

---

# 2. Element Selector ⭐⭐⭐

Selects all elements with the given tag name.

```
p{    color: blue;}
```

Example

```
<p>First</p><p>Second</p>
```

Both paragraphs become blue.

### Common Uses

- Headings
- Paragraphs
- Buttons
- Images

---

# 3. Class Selector (`.`) ⭐⭐⭐⭐⭐

Selects elements with the same class.

Syntax

```
.class-name{}
```

Example

```
<p class="red">Hello</p><h1 class="red">World</h1>
```

```
.red{    color:red;}
```

Output

Both become red.

### Important

- Starts with `.`
- Can be used on multiple elements
- Most commonly used selector in CSS

---

# 4. ID Selector (`#`) ⭐⭐⭐⭐

Selects one unique element.

Syntax

```
#id-name{}
```

Example

```
<h1 id="title">Hello</h1>
```

```
#title{    color:blue;}
```

### Important

- Starts with `#`
- Should be unique
- One ID per page (best practice)

---

# Difference: Class vs ID ⭐⭐⭐⭐⭐

|Class|ID|
|---|---|
|`.`|`#`|
|Reusable|Unique|
|Multiple elements|One element|
|Used most|Used less|

---

# 5. Group Selector ⭐⭐

Select multiple elements together.

```
h1,p,button{    color:red;}
```

Instead of

```
h1{    color:red;}p{    color:red;}button{    color:red;}
```

### Saves code.

---

# 6. Descendant Selector (Space) ⭐⭐⭐⭐

Selects **all matching elements inside another element**, no matter how deeply nested.

Syntax

```
parent child{}
```

Example

```
<div>    <p>Hello</p></div>
```

```
div p{    color:red;}
```

Every `<p>` inside `<div>` is selected.

---

# 7. Child Selector (`>`) ⭐⭐⭐⭐

Selects only **direct children**.

```
div > p{    color:blue;}
```

Example

```
<div>    <p>Selected</p>    <section>        <p>Not Selected</p>    </section></div>
```

Only the first `<p>` is selected.

---

# Descendant vs Child ⭐⭐⭐⭐⭐

```
div p
```

All `<p>` inside `<div>`.

```
div > p
```

Only direct `<p>` children.

---

# 8. Adjacent Sibling (`+`) ⭐⭐⭐

Selects the **immediately next sibling**.

```
h1 + p{    color:red;}
```

Example

```
<h1>Title</h1><p>Selected</p><p>Not Selected</p>
```

Only the first `<p>` is selected.

---

# 9. General Sibling (`~`) ⭐⭐⭐

Selects **all following siblings**.

```
h1 ~ p{    color:green;}
```

Example

```
<h1>Title</h1><p>One</p><p>Two</p><p>Three</p>
```

All paragraphs after `<h1>` are selected.

---

# `+` vs `~`

|`+`|`~`|
|---|---|
|Next sibling only|All following siblings|

---

# 10. Attribute Selector ⭐⭐⭐

Selects elements using attributes.

Example

```
input[type="text"]{    border:2px solid blue;}
```

```
<input type="text"><input type="password">
```

Only the text input is selected.

Common examples

```
input[type="email"]img[alt]a[target="_blank"]input[required]
```

---

# 11. Pseudo Classes ⭐⭐⭐⭐

Select elements based on **state or condition**.

Syntax

```
selector:pseudo-class{}
```

Examples

```
button:hover
```

```
input:focus
```

```
li:first-child
```

```
li:last-child
```

```
input:checked
```

```
input:disabled
```

```
a:visited
```

More pseudo classes will be covered in **Topic 34**.

---

# 12. Pseudo Elements ⭐⭐⭐

Style a **part of an element**.

Syntax

```
selector::pseudo-element{}
```

Examples

```
p::first-letter
```

```
p::first-line
```

```
::selection
```

```
input::placeholder
```

```
::before
```

```
::after
```

These will be covered in detail in **Topic 35**.

---

# Selector Priority (Most Used)

⭐⭐⭐⭐⭐

```
1. Class Selector2. Element Selector3. ID Selector4. Descendant Selector5. Child Selector6. Pseudo Classes7. Pseudo Elements8. Attribute Selector9. Group Selector10. Universal Selector
```

> **Note:** This list reflects **how frequently you'll use them in everyday CSS**, **not CSS specificity** (which you'll learn in Topic 36).

---

# Quick Revision ⭐⭐⭐⭐⭐

|Selector|Symbol|Purpose|
|---|---|---|
|Universal|`*`|All elements|
|Element|`p`|Tag name|
|Class|`.`|Multiple elements|
|ID|`#`|One unique element|
|Group|`,`|Multiple selectors|
|Descendant|Space|Any nested child|
|Child|`>`|Direct child|
|Adjacent|`+`|Next sibling|
|General|`~`|All following siblings|
|Attribute|`[]`|By attribute|
|Pseudo Class|`:`|State/condition|
|Pseudo Element|`::`|Part of an element|
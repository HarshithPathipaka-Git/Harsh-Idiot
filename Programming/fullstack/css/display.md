#  Display ⭐⭐⭐⭐

## What is Display?

The `display` property controls **how an HTML element is displayed** and how it behaves in the page layout.

Syntax

```
display: value;
```

Common Values

```
blockinlineinline-blocknonecontents
```

---

# Default HTML Display

Some HTML elements are **Block Elements** by default.

Examples

```
<div><h1><p><section><header><footer>
```

Some HTML elements are **Inline Elements**.

Examples

```
<span><a><strong><em><img>
```

CSS can change an element's default display.

---

# 1. display: block ⭐⭐⭐⭐⭐

A block element starts on a **new line** and takes the **full available width**.

Example

```
display:block;
```

Example

```
<div>One</div><div>Two</div>
```

Output

```
OneTwo
```

### Characteristics

✔ Starts on a new line

✔ Takes full width

✔ Width and height work

✔ Margin and padding work

Common Block Elements

```
divph1-h6sectionarticleheaderfooter
```

---

# 2. display: inline ⭐⭐⭐⭐

Inline elements stay on the **same line**.

Example

```
display:inline;
```

Example

```
<span>Hello</span><span>World</span>
```

Output

```
Hello World
```

### Characteristics

✔ Same line

✔ Takes only required width

❌ Width doesn't work

❌ Height doesn't work

✔ Left & right padding/margin work

⚠ Top & bottom margin has little or no effect on layout.

Common Inline Elements

```
spanastrongemlabel
```

---

# 3. display: inline-block ⭐⭐⭐⭐⭐

Combination of **inline** and **block**.

Example

```
display:inline-block;
```

Output

```
[Button] [Button] [Button]
```

### Characteristics

✔ Same line

✔ Width works

✔ Height works

✔ Margin works

✔ Padding works

Most Common Uses

- Navigation Links
- Buttons
- Small Cards
- Badges

---

# Block vs Inline vs Inline-Block ⭐⭐⭐⭐⭐

|Property|Block|Inline|Inline-Block|
|---|---|---|---|
|New Line|✅|❌|❌|
|Width|✅|❌|✅|
|Height|✅|❌|✅|
|Margin|✅|Left & Right|✅|
|Padding|✅|Left & Right|✅|

---

# 4. display: none ⭐⭐⭐⭐⭐

Hides the element completely.

Example

```
display:none;
```

The element

- Not visible
- Doesn't occupy space
- Removed from the page layout

Example

```
.menu{    display:none;}
```

Used for

- Mobile menus
- Popups
- Dropdowns
- JavaScript interactions

---

# display:none vs visibility:hidden ⭐⭐⭐⭐

|display:none|visibility:hidden|
|---|---|
|Hidden|Hidden|
|No space occupied|Space still occupied|
|Removed from layout|Stays in layout|

---

# 5. display: contents ⭐⭐

Makes the element itself disappear from the layout while keeping **its children**.

Example

```
<div class="wrapper">    <p>One</p>    <p>Two</p></div>
```

```
.wrapper{    display:contents;}
```

Result

The `<div>` behaves as if it doesn't exist, but the `<p>` elements remain.

### Uses

- Advanced layouts
- Flexbox/Grid helpers

Rarely used.

---

# Changing Display

Example

HTML

```
<span>Hello</span>
```

CSS

```
span{    display:block;}
```

Now the `<span>` behaves like a block element.

---

# Which Display Should I Use?

|Situation|Display|
|---|---|
|Full-width sections|block|
|Text inside a paragraph|inline|
|Buttons in one row|inline-block|
|Hide an element|none|
|Advanced layouts|contents|

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Value|Usage|
|---|---|
|block|⭐⭐⭐⭐⭐|
|inline|⭐⭐⭐⭐|
|inline-block|⭐⭐⭐⭐⭐|
|none|⭐⭐⭐⭐⭐|
|contents|⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Block

```
display:block;
```

New line + Full width

---

### Inline

```
display:inline;
```

Same line

---

### Inline Block

```
display:inline-block;
```

Same line + Width & Height

---

### None

```
display:none;
```

Hidden + No space

---

### Contents

```
display:contents;
```

Parent disappears, children remain

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. block ⭐⭐⭐⭐⭐2. inline-block ⭐⭐⭐⭐⭐3. none ⭐⭐⭐⭐⭐4. inline ⭐⭐⭐⭐5. contents ⭐
```

---

## 💡 Full Stack Tip

In modern frontend development:

- `display: block` → Sections, containers, cards
- `display: inline-block` → Buttons, badges, navigation items (though Flexbox is now often preferred)
- `display: none` → Menus, modals, dropdowns, toggles
- `display: inline` → Text-level elements like links and spans

**Important:** Once you learn **Flexbox** and **Grid**, you'll also use:

```
display:flex;display:grid;
```

These are the most common `display` values in modern web development and will be covered in the next major topics.
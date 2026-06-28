#  Lists ⭐

## What are List Styles?

CSS list properties are used to **change the appearance of HTML lists** (`<ul>`, `<ol>`, `<li>`).

Used for

- Navigation Menus
- Sidebars
- Bullet Lists
- Numbered Lists

Example

```
<ul>    <li>Home</li>    <li>About</li></ul>
```

---

# 1. list-style ⭐⭐⭐

Shorthand property for

- list-style-type
- list-style-position
- list-style-image

Syntax

```
list-style:type position image;
```

Example

```
ul{    list-style:square inside;}
```

---

# 2. list-style-type ⭐⭐⭐⭐

Changes the bullet or numbering style.

Example

```
list-style-type:circle;
```

### Common Values (Unordered List)

```
disc;circle;square;none;
```

Example

```
ul{    list-style-type:square;}
```

---

### Common Values (Ordered List)

```
decimal;upper-alpha;lower-alpha;upper-roman;lower-roman;
```

Example

```
ol{    list-style-type:upper-roman;}
```

Output

```
IIIIII
```

---

### Remove Bullets ⭐⭐⭐⭐⭐

Very common.

```
ul{    list-style-type:none;}
```

Used in

- Navigation Bars
- Sidebars
- Menus

---

# 3. list-style-position ⭐⭐

Controls where the marker (bullet or number) appears.

Values

```
outside;inside;
```

### Outside (Default)

```
list-style-position:outside;
```

```
• Item
```

Bullet stays outside the content.

---

### Inside

```
list-style-position:inside;
```

```
• Item
```

Bullet becomes part of the content block.

Useful for custom layouts.

---

# 4. list-style-image ⭐

Uses an image instead of a bullet.

Example

```
list-style-image:url("star.png");
```

Example

```
ul{    list-style-image:url("check.png");}
```

Rarely used today.

Most developers use:

- Icons
- SVGs
- CSS `::before`

Instead.

---

# List Shorthand ⭐⭐⭐

Instead of

```
list-style-type:square;list-style-position:inside;
```

Use

```
list-style:square inside;
```

Cleaner and shorter.

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|list-style-type|⭐⭐⭐⭐|
|list-style|⭐⭐⭐|
|list-style-position|⭐⭐|
|list-style-image|⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### List Style

```
list-style:square inside;
```

---

### Bullet Type

```
list-style-type:square;
```

---

### Remove Bullets

```
list-style-type:none;
```

---

### Position

```
list-style-position:inside;
```

---

### Image

```
list-style-image:url("icon.png");
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. list-style-type:none ⭐⭐⭐⭐⭐2. list-style ⭐⭐⭐3. list-style-type:square ⭐⭐⭐4. list-style-position ⭐⭐5. list-style-image ⭐
```

---

## 💡 Full Stack Tip

The most common use of list styling is building navigation menus.

```
nav ul{    list-style:none;    padding:0;    margin:0;}
```

You'll see this in almost every website because navigation menus are usually built with `<ul>` and `<li>`, but the default bullets are removed.
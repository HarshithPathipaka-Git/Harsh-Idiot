#  Overflow ⭐⭐

## What is Overflow?

The `overflow` property controls **how content behaves when it exceeds the size of an element**.

Example

```
.box{    width:200px;    height:100px;}
```

If the content is larger than the box, **overflow** decides what happens.

---

# Syntax

```
overflow: value;
```

Common Values

```
visiblehiddenscrollauto
```

---

# 1. overflow: visible ⭐⭐

Default value.

Content is **not clipped** and continues outside the element.

Example

```
overflow: visible;
```

Characteristics

✔ Default behavior

✔ Content remains visible

❌ May overlap other elements

Example

```
.box{    width:200px;    height:100px;    overflow:visible;}
```

---

# 2. overflow: hidden ⭐⭐⭐⭐

Extra content is **hidden**.

Example

```
overflow:hidden;
```

Characteristics

✔ Hides overflowing content

✔ No scrollbar

✔ Keeps layout clean

Common Uses

- Cards
- Images
- Rounded corners
- Cropping content

---

# 3. overflow: scroll ⭐⭐⭐

Always shows scrollbars.

Example

```
overflow:scroll;
```

Characteristics

✔ Scrollbars always visible

✔ User can scroll

❌ Scrollbars appear even when not needed

Common Uses

- Code editors
- Chat windows
- Fixed-size containers

---

# 4. overflow: auto ⭐⭐⭐⭐⭐

Shows scrollbars **only when needed**.

Example

```
overflow:auto;
```

Characteristics

✔ Scrollbars appear automatically

✔ Cleaner than `scroll`

✔ Most commonly used

Common Uses

- Long content
- Tables
- Cards
- Containers

---

# Hidden vs Scroll vs Auto ⭐⭐⭐⭐⭐

|Property|Scrollbar|Hidden Content|
|---|---|---|
|hidden|❌|Yes|
|scroll|Always|No|
|auto|Only if needed|No|

---

# overflow-x & overflow-y ⭐⭐⭐

Control horizontal and vertical overflow separately.

### Horizontal

```
overflow-x:auto;
```

### Vertical

```
overflow-y:auto;
```

Example

```
.box{    width:300px;    height:200px;    overflow-y:auto;    overflow-x:hidden;}
```

Useful for

- Tables
- Code blocks
- Chat windows

---

# Which Property Should I Use?

|Situation|Property|
|---|---|
|Default behavior|visible|
|Hide extra content|hidden|
|Always allow scrolling|scroll|
|Scroll only when needed|auto|

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|auto|⭐⭐⭐⭐⭐|
|hidden|⭐⭐⭐⭐|
|scroll|⭐⭐⭐|
|visible|⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Visible

```
overflow:visible;
```

Default

---

### Hidden

```
overflow:hidden;
```

Hide extra content

---

### Scroll

```
overflow:scroll;
```

Always show scrollbars

---

### Auto

```
overflow:auto;
```

Show scrollbars only when needed

---

### Horizontal

```
overflow-x:auto;
```

---

### Vertical

```
overflow-y:auto;
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. overflow:auto ⭐⭐⭐⭐⭐2. overflow:hidden ⭐⭐⭐⭐3. overflow-y:auto ⭐⭐⭐⭐4. overflow-x:auto ⭐⭐⭐5. overflow:scroll ⭐⭐6. overflow:visible ⭐⭐
```

---

## 💡 Full Stack Tip

These are the patterns you'll see most often:

```
.card{    overflow:hidden;}
```

Used to clip images inside cards, especially when combined with `border-radius`.

```
.table-container{    overflow-x:auto;}
```

Allows wide tables to scroll horizontally on smaller screens.

```
.chat-box{    max-height:400px;    overflow-y:auto;}
```

Creates a vertically scrollable chat or message area.

---
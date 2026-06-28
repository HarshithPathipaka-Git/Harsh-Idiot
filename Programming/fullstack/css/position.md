> **⭐ Interview Question**
> 
> "Explain the difference between `relative`, `absolute`, `fixed`, and `sticky`."

---

# 14. Position ⭐⭐⭐⭐

## What is Position?

The `position` property controls **where an element is placed** on a webpage.

Syntax

```
position: value;
```

Common Values

```
static
relative
absolute
fixed
sticky
```

Positioned elements can also use:

```
top
right
bottom
left
z-index
```

---

# Offset Properties

These work with positioned elements.

```
top
right
bottom
left
```

Example

```
position:relative;
top:20px;
left:30px;
```

Moves the element

- 20px from the top
- 30px from the left

---

# 1. position: static ⭐⭐

Default position.

```
position:static;
```

Characteristics

✔ Default

✔ Normal document flow

❌ `top`, `left`, `right`, `bottom` don't work

Example

```
div{    position:static;}
```

---

# 2. position: relative ⭐⭐⭐⭐⭐

Moves the element **relative to its original position**.

Syntax

```
position:relative;
```

Example

```
.box{    
position:relative;    
top:20px;    
left:30px;
}
```

Characteristics

✔ Keeps original space

✔ Can use `top`, `left`, `right`, `bottom`

✔ Often used as a parent for `absolute`

---

# 3. position: absolute ⭐⭐⭐⭐⭐

Removes the element from the normal document flow.

Position is based on the **nearest positioned parent** (a parent with `position` other than `static`). If none exists, it's positioned relative to the page.

Example

```
.parent{    
position:relative;
}

.child{    
position:absolute;    
top:0;    
right:0;
}
```

Characteristics

✔ Removed from normal flow

✔ Doesn't reserve space

✔ Uses nearest positioned parent

Common Uses

- Badges
- Icons
- Tooltips
- Dropdowns

---

# Relative vs Absolute ⭐⭐⭐⭐⭐

|Relative|Absolute|
|---|---|
|Keeps space|Removes space|
|Moves from original position|Moves relative to positioned parent|
|Used as parent|Used as child|

Common Pattern

```
.card{    position:relative;}

.badge{    position:absolute;    top:10px;    right:10px;}
```

---

# 4. position: fixed ⭐⭐⭐⭐

Fixed relative to the **browser window (viewport)**.

```
position:fixed;
```

Example

```
button{    position:fixed;    bottom:20px;    right:20px;}
```

Characteristics

✔ Always stays visible

✔ Doesn't move while scrolling

✔ Removed from normal flow

Common Uses

- Chat button
- Back to top button
- Floating action button

---

# 5. position: sticky ⭐⭐⭐⭐

Acts like `relative` until a scroll position is reached, then behaves like `fixed`.

Example

```
header{    position:sticky;    top:0;}
```

Characteristics

✔ Scrolls normally

✔ Sticks when reaching the specified position

✔ Requires at least one offset (`top`, `bottom`, etc.)

Common Uses

- Sticky Navbar
- Sticky Sidebar
- Sticky Table Header

---

# Fixed vs Sticky ⭐⭐⭐⭐

|Fixed|Sticky|
|---|---|
|Always fixed|Becomes fixed while scrolling|
|Ignores document flow|Starts in normal flow|
|Relative to viewport|Relative to scroll container|

---

# 6. z-index ⭐⭐⭐⭐⭐

Controls which element appears **on top** when elements overlap.

Higher value = Appears above lower values.

Example

```
.box1{    position:absolute;    
z-index:1;}.

box2{    position:absolute;    z-index:10;}
```

Result

```
box2box1
```

### Important

`z-index` works on **positioned elements** (`relative`, `absolute`, `fixed`, `sticky`).

---

# Position Summary ⭐⭐⭐⭐⭐

|Position|Removes Space?|Moves?|Common Use|
|---|---|---|---|
|static|❌|❌|Default|
|relative|❌|✅|Parent element|
|absolute|✅|✅|Badges, tooltips|
|fixed|✅|✅|Floating buttons|
|sticky|❌|✅|Sticky navbar|

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|relative|⭐⭐⭐⭐⭐|
|absolute|⭐⭐⭐⭐⭐|
|fixed|⭐⭐⭐⭐|
|sticky|⭐⭐⭐⭐|
|z-index|⭐⭐⭐⭐|
|static|⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Static

```
position:static;
```

Default

---

### Relative

```
position:relative;
```

Moves from original position

---

### Absolute

```
position:absolute;top:0;right:0;
```

Moves relative to positioned parent

---

### Fixed

```
position:fixed;bottom:20px;right:20px;
```

Fixed to viewport

---

### Sticky

```
position:sticky;top:0;
```

Sticks while scrolling

---

### z-index

```
z-index:100;
```

Higher value = On top

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. relative ⭐⭐⭐⭐⭐2. absolute ⭐⭐⭐⭐⭐3. z-index ⭐⭐⭐⭐4. fixed ⭐⭐⭐⭐5. sticky ⭐⭐⭐⭐6. static ⭐⭐
```

---

## 💡 Full Stack Tip

You'll constantly see patterns like these in real projects:

```
.card{    position:relative;}.badge{    position:absolute;    top:10px;    right:10px;}
```

Notification badge on a card.

```
header{    position:sticky;    top:0;    z-index:1000;}
```

Sticky navigation bar.

```
.chat-button{    position:fixed;    bottom:20px;    right:20px;}
```

Floating chat or "Back to Top" button.
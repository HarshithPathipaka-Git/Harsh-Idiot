#  Width & Height ⭐⭐⭐

## What are Width & Height?

They define the **size of an element**.

- **Width** → Horizontal size
- **Height** → Vertical size

Example

```
div{    width:300px;    height:200px;}
```

---

# 1. width ⭐⭐⭐⭐⭐

Sets the width of an element.

Syntax

```
width:value;
```

Example

```
width:300px;
```

Using Percentage

```
width:50%;
```

Using Viewport

```
width:100vw;
```

Using Auto

```
width:auto;
```

Common Units

- px
- %
- rem
- vw

---

# 2. height ⭐⭐⭐⭐⭐

Sets the height of an element.

Syntax

```
height:value;
```

Example

```
height:200px;
```

Using Percentage

```
height:100%;
```

Using Viewport

```
height:100vh;
```

Using Auto

```
height:auto;
```

Common Units

- px
- %
- vh
- rem

---

# 3. min-width ⭐⭐⭐

Defines the **minimum width** an element can have.

Example

```
min-width:250px;
```

Meaning

```
Element width ≥ 250px
```

Even if the content is smaller, the width won't go below **250px**.

Useful for

- Buttons
- Cards
- Forms

---

# 4. max-width ⭐⭐⭐⭐⭐

Defines the **maximum width** an element can have.

Example

```
max-width:1200px;
```

Meaning

```
Element width ≤ 1200px
```

Most Common Example

```
.container{    width:100%;    max-width:1200px;    margin:0 auto;}
```

This makes the container responsive while preventing it from becoming too wide.

---

# 5. min-height ⭐⭐⭐

Defines the **minimum height**.

Example

```
min-height:300px;
```

Meaning

```
Height ≥ 300px
```

The element can grow taller if needed but won't be shorter than **300px**.

Useful for

- Cards
- Sections
- Containers

---

# 6. max-height ⭐⭐

Defines the **maximum height**.

Example

```
max-height:500px;
```

Meaning

```
Height ≤ 500px
```

Often used with scrolling.

Example

```
max-height:400px;overflow:auto;
```

---

# width vs max-width ⭐⭐⭐⭐⭐

|width|max-width|
|---|---|
|Fixed or relative width|Maximum allowed width|
|Can overflow on small screens|Responsive|
|Less flexible|More flexible|

Example

```
width:1200px;
```

❌ On a 768px screen, it may overflow.

```
width:100%;max-width:1200px;
```

✔ Responsive.

---

# height vs min-height ⭐⭐⭐⭐

|height|min-height|
|---|---|
|Fixed height|Minimum height|
|Content may overflow|Grows with content|

Example

```
height:200px;
```

Content larger than **200px** may overflow.

```
min-height:200px;
```

The box starts at **200px** and grows if more content is added.

---

# Common Uses

### Width

```
width:100%;
```

Responsive containers.

---

### Max Width

```
max-width:1200px;
```

Main website container.

---

### Height

```
height:100vh;
```

Full-screen hero section.

---

### Min Height

```
min-height:300px;
```

Cards with consistent starting height.

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|width|⭐⭐⭐⭐⭐|
|height|⭐⭐⭐⭐|
|max-width|⭐⭐⭐⭐⭐|
|min-height|⭐⭐⭐⭐|
|min-width|⭐⭐⭐|
|max-height|⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Width

```
width:300px;
```

---

### Height

```
height:200px;
```

---

### Minimum Width

```
min-width:250px;
```

---

### Maximum Width

```
max-width:1200px;
```

---

### Minimum Height

```
min-height:300px;
```

---

### Maximum Height

```
max-height:500px;
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. width ⭐⭐⭐⭐⭐2. max-width ⭐⭐⭐⭐⭐3. height ⭐⭐⭐⭐4. min-height ⭐⭐⭐⭐5. min-width ⭐⭐⭐6. max-height ⭐⭐
```

---

## 💡 Full Stack Tip

You'll see these patterns in almost every modern website:

```
.container{    width:100%;    max-width:1200px;    margin:0 auto;}
```

Responsive container.

```
.hero{    height:100vh;}
```

Full-screen landing page.

```
.card{    min-height:250px;}
```
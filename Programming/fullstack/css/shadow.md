# Shadows ⭐⭐

## What are Shadows?

CSS shadows add a **shadow effect** to elements or text.

There are **2 types**:

- `box-shadow` → For elements
- `text-shadow` → For text

Used for

- Cards
- Buttons
- Images
- Inputs
- Modals
- Headings

---

# Shadow Syntax

Both shadows follow a similar pattern.

```
Horizontal Vertical Blur Spread Color
```

> **Spread** is only available for `box-shadow`.

---

# 1. box-shadow ⭐⭐⭐⭐⭐

Adds a shadow around an element.

Syntax

```
box-shadow: x-offset y-offset blur spread color;
```

Basic Example

```
box-shadow:5px 5px 10px gray;
```

Meaning

```
5px   → Horizontal Offset5px   → Vertical Offset10px  → Blurgray  → Color
```

---

## Complete Example

```
.card{    box-shadow:0 4px 10px rgba(0,0,0,0.2);}
```

Very common for cards.

---

## Multiple Shadows

You can add more than one shadow.

```
box-shadow:0 2px 5px gray,0 8px 20px rgba(0,0,0,0.2);
```

---

## Inset Shadow ⭐⭐⭐

Creates a shadow **inside** the element.

```
box-shadow:inset 0 2px 5px gray;
```

Commonly used for

- Input fields
- Pressed buttons

---

# 2. text-shadow ⭐⭐⭐⭐

Adds a shadow behind text.

Syntax

```
text-shadow:x-offset y-offset blur color;
```

Basic Example

```
text-shadow:2px 2px 5px gray;
```

---

## Heading Example

```
h1{    text-shadow:2px 2px 4px black;}
```

Makes headings stand out.

---

## Glowing Text

```
text-shadow:0 0 10px cyan;
```

Commonly used in

- Logos
- Gaming websites
- Neon effects

---

# box-shadow vs text-shadow ⭐⭐⭐⭐⭐

|box-shadow|text-shadow|
|---|---|
|Elements|Text|
|Supports spread|No spread|
|Supports inset|No inset|
|Used for cards, buttons|Used for headings, logos|

---

# Common Uses

### Card

```
.card{    box-shadow:0 4px 8px rgba(0,0,0,0.2);}
```

---

### Button

```
button{    box-shadow:0 2px 5px rgba(0,0,0,0.3);}
```

---

### Input

```
input{    box-shadow:0 0 5px rgba(0,0,0,0.2);}
```

---

### Heading

```
h1{    text-shadow:2px 2px 5px gray;}
```

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|box-shadow|⭐⭐⭐⭐⭐|
|text-shadow|⭐⭐⭐⭐|
|inset box-shadow|⭐⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Box Shadow

```
box-shadow:5px 5px 10px gray;
```

---

### Modern Card Shadow

```
box-shadow:0 4px 10px rgba(0,0,0,0.2);
```

---

### Inset Shadow

```
box-shadow:inset 0 2px 5px gray;
```

---

### Text Shadow

```
text-shadow:2px 2px 5px black;
```

---

### Glow Effect

```
text-shadow:0 0 10px cyan;
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. box-shadow ⭐⭐⭐⭐⭐2. box-shadow:0 4px 10px rgba(...) ⭐⭐⭐⭐⭐3. text-shadow ⭐⭐⭐⭐4. inset box-shadow ⭐⭐⭐
```

---

## 💡 Full Stack Tip

These are the shadow patterns you'll use most often:

### Card Shadow

```
.card{    box-shadow:0 4px 12px rgba(0,0,0,0.15);}
```

---

### Button Shadow

```
button{    box-shadow:0 2px 6px rgba(0,0,0,0.2);}
```

---

### Text Shadow

```
h1{    text-shadow:2px 2px 4px rgba(0,0,0,0.3);}
```

> **Best Practice:** Use subtle shadows. Heavy shadows can make a UI look outdated. Modern designs typically use soft shadows with low opacity, such as `rgba(0,0,0,0.1)` to `rgba(0,0,0,0.2)`.
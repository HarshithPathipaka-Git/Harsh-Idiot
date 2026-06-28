> **⭐ Interview Question**
> 
> **What are CSS Variables?**
> 
> CSS Variables are reusable values stored in custom properties and accessed using `var()`.

---

# Variables ⭐⭐⭐

## What are CSS Variables?

CSS Variables store reusable values like:

- Colors
- Fonts
- Spacing
- Border Radius
- Shadows
- Sizes

Instead of repeating the same value many times, define it once and reuse it.

Without Variables

```
button{    background:#2563eb;}.card{    border:2px solid #2563eb;}h1{    color:#2563eb;}
```

Same color repeated multiple times.

---

With Variables

```
:root{    --primary:#2563eb;}button{    background:var(--primary);}.card{    border:2px solid var(--primary);}h1{    color:var(--primary);}
```

Change the color once, and every usage updates automatically.

---

# 1. CSS Variables ⭐⭐⭐⭐⭐

Variables are created using **custom properties**.

Syntax

```
--variable-name:value;
```

Example

```
:root{    --primary-color:#2563eb;}
```

Rules

- Variable names start with `--`
- Use meaningful names
- Commonly defined inside `:root`

---

## Why `:root`?

`:root` represents the highest-level element (`<html>`).

Variables declared in `:root` are available throughout the entire stylesheet.

Example

```
:root{    --font-size:18px;}
```

---

# 2. var() ⭐⭐⭐⭐⭐

The `var()` function is used to read a CSS variable.

Syntax

```
var(--variable-name)
```

Example

```
:root{    --primary:#2563eb;}button{    background:var(--primary);}
```

---

## Fallback Value

Use a fallback if the variable doesn't exist.

Syntax

```
var(--variable, fallback)
```

Example

```
color:var(--text-color, black);
```

If `--text-color` is undefined, the color becomes `black`.

---

# Local Variables ⭐⭐⭐

Variables can also be scoped to a specific element.

```
.card{    --card-color:#f5f5f5;    background:var(--card-color);}
```

The variable is only available inside `.card` and its descendants.

---

# Global vs Local Variables ⭐⭐⭐⭐

|Global (`:root`)|Local (Element)|
|---|---|
|Available everywhere|Available only in that element and its children|
|Used for themes|Used for component-specific values|

---

# Common Variables

### Colors

```
:root{    --primary:#2563eb;    --secondary:#64748b;}
```

---

### Fonts

```
:root{    --font:"Poppins", sans-serif;}
```

---

### Spacing

```
:root{    --space:20px;}
```

---

### Border Radius

```
:root{    --radius:10px;}
```

---

### Shadow

```
:root{    
--shadow:    0 4px 10px rgba(0,0,0,0.2);
}
```

---

# Complete Example ⭐⭐⭐⭐⭐

```
:root{
--primary:#2563eb;
--radius:8px;
}
button{
background:var(--primary);
border-radius:var(--radius);
}
```

---

# Which Features Are Used Most? ⭐⭐⭐⭐⭐

|Feature|Usage|
|---|---|
|CSS Variables|⭐⭐⭐⭐⭐|
|var()|⭐⭐⭐⭐⭐|
|:root|⭐⭐⭐⭐⭐|
|Fallback Values|⭐⭐⭐|
|Local Variables|⭐⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Create Variable

```
--primary:#2563eb;
```

---

### Global Variable

```
:root{--primary:#2563eb;}
```

---

### Use Variable

```
color:var(--primary);
```

---

### Fallback

```
color:var(--text, black);
```

---

### Local Variable

```
.card{--card-bg:#eee;}
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. CSS Variables ⭐⭐⭐⭐⭐2. var() ⭐⭐⭐⭐⭐3. :root ⭐⭐⭐⭐⭐4. Fallback Values ⭐⭐⭐5. Local Variables ⭐⭐⭐
```

---

# 💡 Full Stack Tip

Most projects start with a set of global design variables.

```
:root{    --primary:#2563eb;    --secondary:#64748b;    --radius:8px;    --shadow:0 4px 10px rgba(0,0,0,0.15);}
```

Then use them everywhere.

```
.card{    background:var(--primary);    border-radius:var(--radius);    box-shadow:var(--shadow);}
```

This makes your CSS easier to maintain and is especially useful when implementing **dark mode** or changing a website's theme—you update the variable once instead of searching through the entire stylesheet.

---

## 🚀 Variables Cheat Sheet

```
:root
--variable-name
var(--variable)
var(--variable, fallback)
```
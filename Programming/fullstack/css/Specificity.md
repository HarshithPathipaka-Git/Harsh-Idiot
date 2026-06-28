> **"Why isn't my CSS working?"**

Most of the time, the answer is **Specificity**, **Cascade**, or **Inheritance**.

> **⭐ Interview Question**
> 
> **What is CSS Specificity?**
> 
> Specificity is the set of rules browsers use to decide **which CSS rule wins** when multiple rules target the same element.

---

# 36. Specificity ⭐⭐⭐⭐

## What is Specificity?

Specificity determines **which CSS rule has higher priority** when multiple rules apply to the same element.

Example

```
p{    color:blue;}.text{    color:red;}
```

```
<p class="text">Hello</p>
```

Output

```
Red
```

Because the **class selector** has higher specificity than the **element selector**.

---

# CSS Priority Order ⭐⭐⭐⭐⭐

Highest → Lowest

```
!!important

↓

Inline Style

↓

ID Selector

↓

Class / Attribute / Pseudo Class

↓

Element / Pseudo Element

↓

Universal Selector (*)
```

Remember this order.

---

# 1. Selector Priority ⭐⭐⭐⭐⭐

### Universal Selector

```
*{    color:black;}
```

Lowest priority.

---

### Element Selector

```
p{    color:blue;}
```

Higher than `*`.

---

### Class Selector

```
.text{    color:red;}
```

Higher than element selectors.

---

### ID Selector

```
#title{    color:green;}
```

Higher than classes.

---

### Inline Style

```
<p style="color:purple;">
```

Higher than IDs.

---

### !important

```
p{    color:red !important;}
```

Overrides almost everything.

---

# Specificity Table ⭐⭐⭐⭐⭐

|Selector|Priority|
|---|---|
|`!important`|⭐ Highest|
|Inline Style|High|
|ID (`#`)|High|
|Class (`.`), Attribute (`[]`), Pseudo Class (`:hover`)|Medium|
|Element (`p`), Pseudo Element (`::before`)|Low|
|Universal (`*`)|Lowest|

---

# 2. !important ⭐⭐⭐

Forces a rule to override almost all other rules.

Example

```
p{    color:red !important;}
```

Even if another selector has higher specificity, this usually wins.

### Avoid Overusing

❌ Too much `!important` makes CSS difficult to maintain.

Use it only when necessary.

---

# 3. Cascade ⭐⭐⭐⭐⭐

Cascade means **when two rules have the same specificity, the one written later wins**.

Example

```
p{    color:blue;}p{    color:red;}
```

Output

```
Red
```

Because the second rule comes later.

---

# 4. Inheritance ⭐⭐⭐⭐

Some CSS properties automatically pass from a parent to its children.

Example

```
body{    color:blue;}
```

```
<body><p>Hello</p></body>
```

The `<p>` text becomes blue.

---

## Common Inherited Properties

```
color
font-family
font-size
line-height
text-align
```

---

## Properties That Do NOT Inherit

```
margin
padding
border
width
height
background
```

These must be set explicitly if needed.

---

# Specificity Example ⭐⭐⭐⭐⭐

```
p{    color:blue;}.text{    color:red;}#title{    color:green;}
```

```
<p id="title" class="text">    Hello</p>
```

Output

```
Green
```

Because the **ID selector** has the highest specificity among these selectors.

---

# Specificity vs Cascade ⭐⭐⭐⭐

|Specificity|Cascade|
|---|---|
|Higher priority selector wins|If priority is equal, the later rule wins|

---

# Which Concepts Are Used Most? ⭐⭐⭐⭐⭐

|Concept|Usage|
|---|---|
|Selector Priority|⭐⭐⭐⭐⭐|
|Cascade|⭐⭐⭐⭐⭐|
|Inheritance|⭐⭐⭐⭐|
|`!important`|⭐⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Class Beats Element

```
p{    color:blue;}.text{    color:red;}
```

---

### ID Beats Class

```
.text{    color:red;}#title{    color:green;}
```

---

### `!important`

```
color:red !important;
```

---

### Cascade

```
p{    color:blue;}p{    color:red;}
```

Later rule wins.

---

### Inheritance

```
body{    color:blue;}
```

Children inherit the text color.

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. Selector Priority ⭐⭐⭐⭐⭐2. Cascade ⭐⭐⭐⭐⭐3. Inheritance ⭐⭐⭐⭐4. !important ⭐⭐⭐
```

---

# 💡 Full Stack Tip

When CSS isn't behaving as expected, check these in order:

1. **Specificity** – Is another selector more specific?
2. **Cascade** – Is another rule written later?
3. **Inheritance** – Is the property inherited from a parent?
4. **Browser DevTools** – Inspect the element to see which rule is applied or overridden.

Try to avoid this:

```
color:red !important;
```

Instead, write a more specific selector when possible.

```
.card .title{    color:red;}
```

This keeps your CSS cleaner and easier to maintain.

---

## 🚀 Specificity Cheat Sheet

```
!important
Inline Style
ID
Class
Element
Universal (*)
↓
Higher → Lower Priority
```
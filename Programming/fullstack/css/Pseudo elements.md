> **⭐ Interview Question**
> 
> **Pseudo Class vs Pseudo Element**
> 
> - **Pseudo Class (`:`)** → Styles an element based on its **state** (`:hover`, `:focus`).
> - **Pseudo Element (`::`)** → Styles a **part** of an element (`::before`, `::after`).

---

# 35. Pseudo Elements ⭐⭐

## What are Pseudo Elements?

Pseudo Elements allow you to style a **specific part** of an element or insert generated content without modifying the HTML.

Syntax

```
selector::pseudo-element{}
```

Example

```
p::first-letter{    color:red;}
```

---

# Common Pseudo Elements

```
::before::after::first-letter::first-line::selection::placeholder
```

---

# 1. ::before ⭐⭐⭐⭐⭐

Inserts content **before** an element.

Syntax

```
selector::before{content:"";}
```

Example

```
h2::before{    content:"★ ";}
```

Output

```
★ Heading
```

Common Uses

- Icons
- Decorative Lines
- Badges
- Labels

---

# 2. ::after ⭐⭐⭐⭐⭐

Inserts content **after** an element.

Example

```
h2::after{    content:" ✔";}
```

Output

```
Heading ✔
```

Common Uses

- Decorative Elements
- Underlines
- Badges

---

# Important

`::before` and `::after` **must** include the `content` property.

Example

```
.card::before{    content:"";}
```

Without `content`, they won't appear.

---

# 3. ::first-letter ⭐⭐⭐

Styles only the first letter.

Example

```
p::first-letter{    font-size:2rem;    color:red;}
```

Common Uses

- Blog articles
- Magazines
- News websites

---

# 4. ::first-line ⭐⭐⭐

Styles only the first line.

Example

```
p::first-line{    font-weight:bold;}
```

Used for

- Articles
- Blog Posts

---

# 5. ::selection ⭐⭐⭐

Styles selected text.

Example

```
::selection{    background:#2563eb;    color:white;}
```

Common Uses

- Branding
- Better user experience

---

# 6. ::placeholder ⭐⭐⭐⭐

Styles placeholder text inside form controls.

Example

```
input::placeholder{    color:gray;}
```

Common Uses

- Forms
- Login Pages
- Search Boxes

---

# before vs after ⭐⭐⭐⭐⭐

|::before|::after|
|---|---|
|Inserts before content|Inserts after content|
|Needs `content`|Needs `content`|
|Decorative icons|Decorative icons|

---

# Common Uses

### Decorative Line

```
h2::after{    content:"";    display:block;    width:50px;    height:3px;    background:#2563eb;}
```

---

### Icon Before Text

```
li::before{    content:"✔ ";}
```

---

### Placeholder

```
input::placeholder{    color:#888;}
```

---

### Selected Text

```
::selection{    background:black;    color:white;}
```

---

# Which Pseudo Elements Are Used Most? ⭐⭐⭐⭐⭐

|Pseudo Element|Usage|
|---|---|
|::before|⭐⭐⭐⭐⭐|
|::after|⭐⭐⭐⭐⭐|
|::placeholder|⭐⭐⭐⭐|
|::selection|⭐⭐⭐|
|::first-letter|⭐⭐⭐|
|::first-line|⭐⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Before

```
h1::before{    content:"★ ";}
```

---

### After

```
h1::after{    content:" ✔";}
```

---

### First Letter

```
p::first-letter{    font-size:2rem;}
```

---

### First Line

```
p::first-line{    font-weight:bold;}
```

---

### Selection

```
::selection{    background:#2563eb;    color:white;}
```

---

### Placeholder

```
input::placeholder{    color:gray;}
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. ::before ⭐⭐⭐⭐⭐2. ::after ⭐⭐⭐⭐⭐3. ::placeholder ⭐⭐⭐⭐4. ::selection ⭐⭐⭐5. ::first-letter ⭐⭐⭐6. ::first-line ⭐⭐
```

---

# 💡 Full Stack Tip

These pseudo elements are used frequently in modern websites:

### Decorative Underline

```
.title::after{    content:"";    display:block;    width:60px;    height:3px;    background:#2563eb;}
```

---

### Custom List Icon

```
li::before{    content:"✓ ";    color:green;}
```

---

### Search Placeholder

```
input::placeholder{    color:#999;}
```

> **Best Practice:** Use `::before` and `::after` for **decorative content only**. Don't use them to insert important information that users or assistive technologies must rely on. Essential content should be present in the HTML.

---

## 🚀 Pseudo Elements Cheat Sheet

```
::before::after::first-letter::first-line::selection::placeholder
```
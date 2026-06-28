# Introduction to CSS ⭐⭐⭐

## What is CSS?

**CSS (Cascading Style Sheets)** is used to style and design HTML elements.

Without CSS → HTML looks plain.  
With CSS → HTML becomes attractive and responsive.

### CSS is used for

- Colors
- Fonts
- Spacing
- Layout
- Animations
- Responsive Design

---

## Why CSS?

HTML = Structure 🏠

CSS = Design 🎨

JavaScript = Functionality ⚙️

Example

```
HTML<h1>Hello</h1>↓CSSh1{    color: blue;    font-size:40px;}↓OutputBlue "Hello"
```

---

## Types of CSS

There are **3 ways** to apply CSS.

### 1. Inline CSS

CSS written inside the HTML element.

```
<h1 style="color:red;">Hello</h1>
```

✔ Used for testing  
❌ Not recommended for large projects

---

### 2. Internal CSS

CSS written inside the `<style>` tag.

```
<head>    <style>        h1{            color:red;        }    </style></head>
```

✔ Good for single-page websites

---

### 3. External CSS ⭐⭐⭐⭐⭐

CSS written in a separate `.css` file.

```
style.css
```

Linked using

```
<link rel="stylesheet" href="style.css">
```

✔ Best Practice  
✔ Reusable  
✔ Easy to maintain  
✔ Used in real projects

---

## CSS Syntax

Basic Structure

```
selector{    property: value;}
```

Example

```
h1{    color: blue;}
```

Breakdown

```
h1        → Selectorcolor     → Propertyblue      → Value
```

General Form

```
selector{    property: value;    property: value;    property: value;}
```

---

## CSS Comments

Single-line or multi-line comments.

```
/* This is a comment */
```

Example

```
/* Heading Color */h1{    color:red;}
```

Comments are ignored by the browser.

Used for

- Explaining code
- Organizing sections
- Temporarily disabling CSS

---

# Quick Revision ⭐⭐⭐⭐⭐

### CSS

- Styles HTML
- Controls design
- Makes websites responsive

---

### Types

- Inline
- Internal
- External ⭐

---

### Syntax

```
selector{    property:value;}
```

---

### Comment

```
/* Comment */
```

---

### Real Project Usage

|Type|Used?|
|---|---|
|Inline|Rarely|
|Internal|Sometimes|
|External|⭐ Almost Always|
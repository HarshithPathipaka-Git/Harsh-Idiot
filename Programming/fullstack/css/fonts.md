# 6. Fonts ⭐⭐

## What are Fonts?

Fonts define the **style or appearance** of text on a webpage.

They improve:

- Readability
- User Experience (UX)
- Branding
- Design

Example

```
h1{    font-family: Arial, sans-serif;}
```

---

# Types of Fonts

There are **3 common ways** to use fonts in CSS.

- Web Safe Fonts
- Google Fonts
- `@font-face`

---

# 1. Web Safe Fonts ⭐⭐⭐

These are fonts that are **already installed** on most operating systems.

No download is required.

Example

```
font-family: Arial, sans-serif;
```

Common Web Safe Fonts

```
ArialHelveticaVerdanaTahomaTrebuchet MSTimes New RomanGeorgiaCourier New
```

### Font Family Categories

```
font-family: Arial, sans-serif;font-family: Georgia, serif;font-family: "Courier New", monospace;
```

|Family|Example|
|---|---|
|serif|Times New Roman, Georgia|
|sans-serif|Arial, Helvetica, Verdana|
|monospace|Courier New, Consolas|
|cursive|Brush Script MT|
|fantasy|Papyrus (rarely used)|

### Advantages

✔ Fast

✔ No internet needed

✔ Works on almost every browser

---

# 2. Google Fonts ⭐⭐⭐⭐⭐

The most common way to use fonts in modern websites.

Google provides **free fonts** that can be loaded from the web.

### Step 1

Choose a font from

> [https://fonts.google.com](https://fonts.google.com)

---

### Step 2

Add the `<link>` inside `<head>`

Example

```
<link rel="preconnect" href="https://fonts.googleapis.com"><link rel="preconnect" href="https://fonts.gstatic.com" crossorigin><link href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;700&display=swap" rel="stylesheet">
```

---

### Step 3

Use it in CSS

```
body{    font-family: "Poppins", sans-serif;}
```

### Advantages

✔ Hundreds of fonts

✔ Easy to use

✔ Widely used

✔ Free

---

# 3. @font-face ⭐⭐⭐⭐

Used to load **custom font files** from your project.

Example Folder

```
project/│── index.html│── style.css│── fonts/      Roboto-Regular.ttf
```

CSS

```
@font-face{    font-family:"MyFont";    src:url("fonts/Roboto-Regular.ttf");}body{    font-family:"MyFont";}
```

Supported Formats

```
.woff2 ⭐ (Best).woff.ttf.otf
```

### Advantages

✔ Works offline

✔ Custom branding

✔ No dependency on Google Fonts

---

# Google Fonts vs @font-face ⭐⭐⭐⭐

|Google Fonts|@font-face|
|---|---|
|Online|Local font files|
|Easy setup|More setup required|
|Free fonts|Any custom font|
|Most common|Used for branding or offline fonts|

---

# Font Fallback ⭐⭐⭐

Always specify a fallback font.

Example

```
font-family:"Poppins", Arial, sans-serif;
```

If **Poppins** isn't available, the browser tries:

1. Arial
2. sans-serif

---

# Best Practice ⭐⭐⭐⭐⭐

Always use a fallback font.

```
font-family: Arial, sans-serif;
```

or

```
font-family: "Poppins", sans-serif;
```

---

# Quick Revision ⭐⭐⭐⭐⭐

### Web Safe Font

```
font-family: Arial, sans-serif;
```

---

### Google Fonts

```
<link href="https://fonts.googleapis.com/..." rel="stylesheet">
```

```
font-family:"Poppins", sans-serif;
```

---

### @font-face

```
@font-face{    font-family:"MyFont";    src:url("font.woff2");}
```

---

### Fallback Font

```
font-family:"Roboto", Arial, sans-serif;
```

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. Google Fonts ⭐⭐⭐⭐⭐2. Web Safe Fonts ⭐⭐⭐⭐3. @font-face ⭐⭐⭐
```

---

## 💡 Full Stack Tip

In modern frontend development:

- **Google Fonts** → Used in most websites and personal projects.
- **Web Safe Fonts** → Good fallback if custom fonts fail to load.
- **`@font-face`** → Used when hosting your own fonts (common in branded websites, company projects, or offline apps).
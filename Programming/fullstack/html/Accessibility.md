#  Accessibility

## ARIA

**Purpose:** Improves accessibility for assistive technologies.

**Example**

```html
<button aria-label="Close"></button>
```

**Use**

- Screen readers
    
- Custom UI components
    

⭐ Use only when semantic HTML isn't enough.

---

## `alt`

**Purpose:** Provides alternative text for images.

**Example**

```html
<img src="logo.png" alt="Company Logo">
```

**Use**

- Accessibility
    
- SEO
    
- Displays text if the image fails to load
    

⭐ Always include meaningful `alt` text.

---

## `<label>`

**Purpose:** Associates text with form controls.

**Example**

```html
<label for="email">Email</label>
<input id="email" type="email">
```

**Use**

- Forms
    
- Accessibility
    

⭐ Always pair labels with form inputs.

---

## Semantic Elements

**Purpose:** Give meaning to page structure.

**Examples**

- `<header>`
    
- `<nav>`
    
- `<main>`
    
- `<section>`
    
- `<article>`
    
- `<footer>`
    

**Use**

- Better accessibility
    
- Better SEO
    

⭐ Prefer semantic elements over generic `<div>` elements when appropriate.

---

## Keyboard Navigation

**Purpose:** Allows users to navigate without a mouse.

**Use**

- `Tab`
    
- `Shift + Tab`
    
- `Enter`
    
- `Space`
    

⭐ Ensure all interactive elements are keyboard accessible.

---

## Screen Readers

**Purpose:** Read webpage content aloud for visually impaired users.

**Works Best With**

- Semantic HTML
    
- `alt` text
    
- `<label>`
    
- ARIA attributes
    
- Proper heading structure
    

---

# ⭐ Most Used

- `alt`
    
- `<label>`
    
- Semantic Elements
    
- ARIA
    

---

# ✅ Best Practices

- Always add `alt` to images.
    
- Use `<label>` for every form input.
    
- Use semantic HTML whenever possible.
    
- Test keyboard navigation.
    
- Use ARIA only when necessary.
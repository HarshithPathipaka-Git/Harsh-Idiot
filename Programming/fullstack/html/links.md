# Links

## `<a>`

**Purpose:** Creates a hyperlink.

**Syntax**

```html
<a href="https://example.com">Visit</a>
```

**Use**

- Navigate between pages
    
- External websites
    
- Downloads
    
- Email & Phone links
    

⭐ Most used HTML tag.

---

## `href`

**Purpose:** Specifies the destination URL.

**Syntax**

```html
<a href="about.html">About</a>
```

**Values**

- URL
    
- File
    
- Email
    
- Phone
    
- Anchor
    

---

## `target`

**Purpose:** Specifies where the linked page opens.

**Common Values**

```html
_self
```

Default (same tab)

```html
_blank
```

New tab

**Example**

```html
<a href="https://google.com" target="_blank">
```

⭐ Most commonly used: `_blank`

---

## `download`

**Purpose:** Downloads a file instead of opening it.

**Example**

```html
<a href="resume.pdf" download>Download Resume</a>
```

---

## `mailto`

**Purpose:** Opens the user's email application.

**Example**

```html
<a href="mailto:abc@gmail.com">
```

**Use**

- Contact pages
    
- Support email
    

---

## `tel`

**Purpose:** Opens the phone dialer.

**Example**

```html
<a href="tel:+919876543210">
```

**Use**

- Contact pages
    
- Mobile websites
    

---

## Relative URLs

**Purpose:** Link within the same website.

**Examples**

```html
href="about.html"

href="contact.html"

href="../images/logo.png"
```

⭐ Used for internal navigation.

---

## Absolute URLs

**Purpose:** Link to another website.

**Example**

```html
href="https://www.google.com"
```

⭐ Used for external websites.

---

## Anchor Links

**Purpose:** Jump to a specific section of the same page.

### Step 1

```html
<h2 id="contact">Contact</h2>
```

### Step 2

```html
<a href="#contact">Go to Contact</a>
```

⭐ Useful for long webpages and documentation.

---

# ⭐ Most Used

- `<a>`
    
- `href`
    
- `target`
    
- Relative URLs
    
- Absolute URLs
    

---

# ⭐ Occasionally Used

- `download`
    
- `mailto`
    
- `tel`
    
- Anchor Links
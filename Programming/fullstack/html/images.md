
#  Images

## `<img>`

**Purpose:** Displays an image.

**Syntax**

```html
<img src="image.jpg" alt="Description">
```

**Use**

- Photos
    
- Logos
    
- Icons
    
- Banners
    

⭐ Most used image tag.

---

## `src`

**Purpose:** Specifies the image file location.

**Example**

```html
<img src="images/logo.png">
```

**Supports**

- Relative URL
    
- Absolute URL
    

---

## `alt`

**Purpose:** Alternative text if the image cannot load.

**Example**

```html
<img src="logo.png" alt="Company Logo">
```

**Use**

- Accessibility
    
- SEO
    
- Broken images
    

⭐ Always provide meaningful `alt` text.

---

## `width`

**Purpose:** Sets image width.

**Example**

```html
<img src="logo.png" width="300">
```

---

## `height`

**Purpose:** Sets image height.

**Example**

```html
<img src="logo.png" height="200">
```

⚠️ Maintain the correct aspect ratio to avoid distortion.

---

## `loading="lazy"`

**Purpose:** Loads images only when needed.

**Example**

```html
<img src="photo.jpg" loading="lazy">
```

**Benefits**

- Faster page loading
    
- Better performance
    

⭐ Recommended for most images below the visible area.

---

## `<picture>`

**Purpose:** Displays different images for different screen sizes or formats.

**Example**

```html
<picture>
    <source srcset="mobile.jpg" media="(max-width:768px)">
    <img src="desktop.jpg" alt="Banner">
</picture>
```

**Use**

- Responsive images
    
- Modern image formats
    

---

## `<source>`

**Purpose:** Defines alternate image or media sources.

**Use**

- Inside `<picture>`
    
- Inside `<audio>`
    
- Inside `<video>`
    

---

## `<figure>`

**Purpose:** Groups an image with related content.

**Example**

```html
<figure>
    <img src="mountain.jpg" alt="Mountain">
</figure>
```

**Use**

- Images
    
- Charts
    
- Diagrams
    
- Code snippets
    

---

## `<figcaption>`

**Purpose:** Adds a caption to a `<figure>`.

**Example**

```html
<figure>
    <img src="mountain.jpg" alt="Mountain">
    <figcaption>Beautiful mountain view</figcaption>
</figure>
```

---

# ⭐ Most Used

- `<img>`
    
- `src`
    
- `alt`
    
- `width`
    
- `height`
    
- `loading="lazy"`
    

---

# ⭐ Occasionally Used

- `<picture>`
    
- `<source>`
    
- `<figure>`
    
- `<figcaption>`
    

---

# ✅ Best Practices

- Always add `alt`.
    
- Use `loading="lazy"` for non-critical images.
    
- Optimize image size before uploading.
    
- Prefer modern formats like **WebP** or **AVIF** when supported.
    
- Use `<picture>` for responsive images when different image versions are needed.
# HTML Attributes

## `id`

**Purpose:** Uniquely identifies an element.

**Example**

```html
<div id="header"></div>
```

**Use**

- CSS
    
- JavaScript
    
- Anchor links
    

⭐ Must be unique.

---

## `class`

**Purpose:** Groups multiple elements.

**Example**

```html
<div class="card"></div>
```

**Use**

- CSS styling
    
- JavaScript
    
- Reusable components
    

⭐ Most used attribute.

---

## `style`

**Purpose:** Applies inline CSS.

**Example**

```html
<p style="color:red;">Hello</p>
```

**Use**

- Quick styling
    

⚠️ Avoid for large projects.

---

## `title`

**Purpose:** Shows tooltip text.

**Example**

```html
<button title="Save">💾</button>
```

**Use**

- Extra information
    
- Accessibility
    

---

## `hidden`

**Purpose:** Hides an element.

**Example**

```html
<div hidden></div>
```

**Use**

- Hide content until needed.
    

---

## `draggable`

**Purpose:** Makes an element draggable.

**Example**

```html
<div draggable="true"></div>
```

**Use**

- Drag & Drop interfaces
    

---

## `contenteditable`

**Purpose:** Allows users to edit content.

**Example**

```html
<p contenteditable="true">Edit me</p>
```

**Use**

- Text editors
    
- Notes apps
    

---

## `tabindex`

**Purpose:** Controls keyboard navigation order.

**Example**

```html
<input tabindex="1">
```

**Use**

- Accessibility
    
- Forms
    

---

## `spellcheck`

**Purpose:** Enables or disables spell checking.

**Example**

```html
<textarea spellcheck="true"></textarea>
```

**Values**

- true
    
- false
    

---

## `translate`

**Purpose:** Controls automatic translation.

**Example**

```html
<p translate="no">ChatGPT</p>
```

**Values**

- yes
    
- no
    

---

## `data-*`

**Purpose:** Stores custom data.

**Example**

```html
<div data-id="101"></div>
```

**Use**

- JavaScript
    
- Custom attributes
    

⭐ Very common in web apps.

---

## `aria-*`

**Purpose:** Improves accessibility.

**Example**

```html
<button aria-label="Close"></button>
```

**Use**

- Screen readers
    
- Accessible websites
    

⭐ Important for accessibility.

---

# ⭐ Most Used

- `id`
    
- `class`
    
- `style`
    
- `title`
    
- `data-*`
    
- `aria-*`
    

---

# ⭐ Occasionally Used

- `hidden`
    
- `draggable`
    
- `contenteditable`
    
- `tabindex`
    
- `spellcheck`
    
- `translate`
    

---

# ✅ Best Practices

- Use `id` only once per page.
    
- Reuse `class` for styling.
    
- Prefer external CSS over `style`.
    
- Use `data-*` for custom data.
    
- Add `aria-*` attributes to improve accessibility.
    
- Use `tabindex` carefully to maintain logical keyboard navigation.
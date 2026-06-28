#  Lists

## `<ul>`

**Purpose:** Creates an unordered (bulleted) list.

**Syntax**

```html
<ul>
    <li>HTML</li>
    <li>CSS</li>
</ul>
```

**Use**

- Navigation menus
    
- Feature lists
    
- Categories
    

⭐ Most commonly used list.

---

## `<ol>`

**Purpose:** Creates an ordered (numbered) list.

**Syntax**

```html
<ol>
    <li>Install Git</li>
    <li>Configure Git</li>
</ol>
```

**Use**

- Step-by-step instructions
    
- Rankings
    
- Procedures
    

---

## `<li>`

**Purpose:** Defines a list item.

**Syntax**

```html
<li>JavaScript</li>
```

**Use**

- Inside `<ul>` or `<ol>`.
    

⭐ Required for ordered and unordered lists.

---

## `<dl>`

**Purpose:** Creates a description list.

**Syntax**

```html
<dl>
    <dt>HTML</dt>
    <dd>Markup Language</dd>
</dl>
```

**Use**

- Definitions
    
- Glossaries
    
- FAQs
    

---

## `<dt>`

**Purpose:** Defines the term in a description list.

**Example**

```html
<dt>CSS</dt>
```

---

## `<dd>`

**Purpose:** Defines the description of a term.

**Example**

```html
<dd>Styles web pages.</dd>
```

---

## Nested Lists

**Purpose:** Creates lists inside other lists.

**Example**

```html
<ul>
    <li>Frontend
        <ul>
            <li>HTML</li>
            <li>CSS</li>
        </ul>
    </li>
</ul>
```

**Use**

- Menus
    
- Categories
    
- Documentation
    
- File structures
    

---

# ⭐ Most Used

- `<ul>`
    
- `<ol>`
    
- `<li>`
    

---

# ⭐ Occasionally Used

- `<dl>`
    
- `<dt>`
    
- `<dd>`
    
- Nested Lists
    

---

# ✅ Best Practices

- Use `<ul>` for unordered content.
    
- Use `<ol>` for ordered steps.
    
- Always place `<li>` inside `<ul>` or `<ol>`.
    
- Use nested lists for hierarchical data.
    
- Use description lists for terms and definitions, not general layouts.
# Forms ⭐

## `<form>`

**Purpose:** Creates a form to collect user input.

**Syntax**

```html
<form action="/submit" method="POST">
```

**Use**

- Login
    
- Signup
    
- Contact forms
    
- Search
    

---

## `<input>`

**Purpose:** Accepts user input.

**Example**

```html
<input type="text">
```

⭐ Most used form element.

---

## `<label>`

**Purpose:** Adds a label to an input.

**Example**

```html
<label for="email">Email</label>
```

⭐ Improves accessibility.

---

## `<textarea>`

**Purpose:** Multi-line text input.

**Example**

```html
<textarea></textarea>
```

**Use**

- Comments
    
- Messages
    
- Feedback
    

---

## `<button>`

**Purpose:** Creates a clickable button.

**Types**

- submit
    
- reset
    
- button
    

**Example**

```html
<button type="submit">Submit</button>
```

---

## `<select>`

**Purpose:** Creates a dropdown list.

**Example**

```html
<select></select>
```

---

## `<option>`

**Purpose:** Defines an item inside `<select>`.

**Example**

```html
<option>India</option>
```

---

## `<optgroup>`

**Purpose:** Groups related options.

**Example**

```html
<optgroup label="Asia">
```

---

## `<datalist>`

**Purpose:** Provides input suggestions.

**Example**

```html
<input list="cities">
```

---

## `<fieldset>`

**Purpose:** Groups related form controls.

**Use**

- Registration forms
    
- Survey sections
    

---

## `<legend>`

**Purpose:** Adds a title to a `<fieldset>`.

**Example**

```html
<legend>Personal Information</legend>
```

---

## `<output>`

**Purpose:** Displays calculation results.

**Use**

- Calculators
    
- Dynamic forms
    

---

# Input Types ⭐

- text
    
- password
    
- email
    
- number
    
- tel
    
- url
    
- search
    
- date
    
- time
    
- datetime-local
    
- month
    
- week
    
- color
    
- range
    
- file
    
- checkbox
    
- radio
    
- submit
    
- reset
    
- hidden
    

⭐ Most used:

- text
    
- password
    
- email
    
- number
    
- file
    
- checkbox
    
- radio
    
- submit
    

---

# Validation

**Purpose:** Validates user input before submission.

---

## `required`

**Purpose:** Makes a field mandatory.

**Example**

```html
<input required>
```

---

## `placeholder`

**Purpose:** Shows hint text.

**Example**

```html
<input placeholder="Enter email">
```

---

## `pattern`

**Purpose:** Validates input using a regular expression.

**Example**

```html
<input pattern="[A-Za-z]{3,}">
```

---

## `autocomplete`

**Purpose:** Enables or disables browser autofill.

**Values**

- on
    
- off
    

**Example**

```html
<input autocomplete="off">
```

---

## `enctype`

**Purpose:** Specifies how form data is encoded.

**Common Values**

- application/x-www-form-urlencoded (Default)
    
- multipart/form-data ⭐ (File upload)
    
- text/plain
    

**Example**

```html
<form enctype="multipart/form-data">
```

---

# GET vs POST

### GET

- Sends data in URL
    
- Visible to user
    
- Used for search/filter
    
- Limited data size
    

### POST

- Sends data in request body
    
- Hidden from URL
    
- Used for login, signup, file upload
    
- Supports large data
    

⭐ Use **POST** for sensitive or form submission data.

---

# ⭐ Most Used

- form
    
- input
    
- label
    
- textarea
    
- button
    
- select
    
- option
    
- required
    
- placeholder
    
- GET & POST
    

---

# ⭐ Occasionally Used

- fieldset
    
- legend
    
- datalist
    
- optgroup
    
- output
    
- pattern
    
- autocomplete
    
- enctype
    

---

# ✅ Best Practices

- Always use `<label>` with inputs.
    
- Validate user input.
    
- Use meaningful placeholders.
    
- Use `required` for mandatory fields.
    
- Use **POST** for forms containing sensitive data.
    
- Use `multipart/form-data` when uploading files.
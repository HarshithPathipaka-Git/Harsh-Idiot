# Cursor ⭐

## What is Cursor?

The `cursor` property changes the **mouse pointer** when it moves over an element.

Used for

- Buttons
- Links
- Forms
- Images
- Disabled Elements
- Loading States

Syntax

```
cursor:value;
```

---

# Common Cursor Values ⭐⭐⭐⭐⭐

### pointer ⭐⭐⭐⭐⭐

Shows a hand pointer.

```
cursor:pointer;
```

Used for

- Buttons
- Links
- Clickable Cards

---

### default ⭐⭐⭐

Default arrow cursor.

```
cursor:default;
```

---

### text ⭐⭐⭐

Shows the text selection cursor (I-beam).

```
cursor:text;
```

Used for

- Input fields
- Paragraphs
- Text areas

---

### not-allowed ⭐⭐⭐⭐

Shows a prohibited (🚫) cursor.

```
cursor:not-allowed;
```

Used for

- Disabled buttons
- Restricted actions

---

### wait ⭐⭐⭐

Shows a loading cursor.

```
cursor:wait;
```

Used while waiting for a process to finish.

---

### move ⭐⭐

Shows a move cursor.

```
cursor:move;
```

Used for

- Drag & Drop
- Draggable Items

---

### grab ⭐⭐⭐

Shows an open-hand cursor.

```
cursor:grab;
```

When dragging

```
cursor:grabbing;
```

Used for

- Sliders
- Image galleries
- Drag-and-drop interfaces

---

### crosshair ⭐⭐

Shows a cross (+) cursor.

```
cursor:crosshair;
```

Used in

- Drawing tools
- Image editors

---

### help ⭐

Shows a help cursor.

```
cursor:help;
```

Used for

- Help icons
- Tooltips

---

### progress ⭐⭐

Shows that something is loading, but the page is still usable.

```
cursor:progress;
```

---

# Complete Example

```
button{
    cursor:pointer;
}
input{    
cursor:text;
}
.disabled{    
cursor:not-allowed;
}
```

---

# Which Cursor Should I Use?

|Element|Cursor|
|---|---|
|Button|pointer|
|Link|pointer|
|Text|text|
|Disabled Button|not-allowed|
|Loading|wait / progress|
|Draggable Item|grab|

---

# Which Values Are Used Most? ⭐⭐⭐⭐⭐

|Cursor|Usage|
|---|---|
|pointer|⭐⭐⭐⭐⭐|
|text|⭐⭐⭐⭐|
|not-allowed|⭐⭐⭐⭐|
|default|⭐⭐⭐|
|grab|⭐⭐⭐|
|wait|⭐⭐⭐|
|move|⭐⭐|
|progress|⭐⭐|
|crosshair|⭐|
|help|⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Pointer

```
cursor:pointer;
```

Clickable element.

---

### Default

```
cursor:default;
```

Normal arrow.

---

### Text

```
cursor:text;
```

Text selection.

---

### Disabled

```
cursor:not-allowed;
```

Not allowed.

---

### Loading

```
cursor:wait;
```

Waiting.

---

### Drag

```
cursor:grab;
```

Draggable element.

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. cursor:pointer ⭐⭐⭐⭐⭐
2. cursor:text ⭐⭐⭐⭐
3. cursor:not-allowed ⭐⭐⭐⭐
4. cursor:default ⭐⭐⭐
5. cursor:grab ⭐⭐⭐
6. cursor:wait ⭐⭐⭐
```

---

## 💡 Full Stack Tip

You'll see these patterns in almost every project:

```
button{    cursor:pointer;}
```

Clickable buttons.

```
input{    cursor:text;}
```

Text inputs.

```
button:disabled{    cursor:not-allowed;}
```

Disabled buttons.

> **Note:** HTML links (`<a href="...">`) already show the **pointer** cursor by default, so you usually don't need to set it manually. For custom clickable elements like `<div>` or `<button>`, `cursor: pointer` is commonly used to make them feel interactive.
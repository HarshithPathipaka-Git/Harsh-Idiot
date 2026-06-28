#  Tables

## `<table>`

**Purpose:** Creates a table.

**Syntax**

```html
<table>
    ...
</table>
```

**Use**

- Display tabular data
    
- Reports
    
- Admin dashboards
    

---

## `<tr>`

**Purpose:** Defines a table row.

**Syntax**

```html
<tr>
    ...
</tr>
```

---

## `<td>`

**Purpose:** Defines a table data cell.

**Syntax**

```html
<td>John</td>
```

---

## `<th>`

**Purpose:** Defines a table header cell.

**Syntax**

```html
<th>Name</th>
```

**Default**

- Bold
    
- Center aligned
    

---

## `<thead>`

**Purpose:** Groups table header rows.

**Syntax**

```html
<thead>
    ...
</thead>
```

---

## `<tbody>`

**Purpose:** Groups the main table data.

**Syntax**

```html
<tbody>
    ...
</tbody>
```

---

## `<tfoot>`

**Purpose:** Groups footer rows.

**Syntax**

```html
<tfoot>
    ...
</tfoot>
```

**Use**

- Totals
    
- Summary rows
    

---

## `<caption>`

**Purpose:** Adds a title to the table.

**Syntax**

```html
<caption>Student Details</caption>
```

---

## `colspan`

**Purpose:** Merges multiple columns.

**Example**

```html
<td colspan="2">Total</td>
```

---

## `rowspan`

**Purpose:** Merges multiple rows.

**Example**

```html
<td rowspan="2">John</td>
```

---

# ⭐ Most Used

- `<table>`
    
- `<tr>`
    
- `<td>`
    
- `<th>`
    
- `<thead>`
    
- `<tbody>`
    

---

# ⭐ Occasionally Used

- `<tfoot>`
    
- `<caption>`
    
- `colspan`
    
- `rowspan`
    

---

# ✅ Best Practices

- Use `<th>` for headings.
    
- Use `<thead>`, `<tbody>`, and `<tfoot>` for better structure.
    
- Use tables only for **tabular data**, not for page layouts.
    
- Add `<caption>` when the table needs a title.
    
- Use `colspan` and `rowspan` only when necessary.
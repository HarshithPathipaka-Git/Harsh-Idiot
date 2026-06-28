# Tables ⭐

## What is Table Styling?

CSS table properties are used to control the appearance and layout of HTML tables.

Used for

- Data Tables
- Reports
- Dashboards
- Invoices
- Timetables

Example

```
<table> 
   <tr>        
	   <th>Name</th>        
	   <th>Age</th>    
   </tr>
   
   <tr>        
	   <td>Harshith</td>        
	   <td>19</td>    
   </tr>
</table>
```

---

# 1. border-collapse ⭐⭐⭐⭐

Controls whether table borders are separated or merged.

Syntax

```
border-collapse:value;
```

Values

```
border-collapse:collapse;
border-collapse:separate;
```

### collapse ⭐⭐⭐⭐⭐

Merges adjacent borders into one.

```
table{    border-collapse:collapse;}
```

Output

```
+------+------+
| Name | Age  |
+------+------+
| John | 20   |
+------+------+
```

✔ Most commonly used.

---

### separate (Default)

Each cell has its own border.

```
table{    border-collapse:separate;}
```

Output

```
+----+  +----+
|    |  |    |
+----+  +----+
```

---

# 2. border-spacing ⭐⭐

Sets the space between table cells.

Works **only when**:

```
border-collapse:separate;
```

Example

```
table{    border-spacing:10px;}
```

Different Values

```
border-spacing:10px 20px;
```

```
Horizontal = 10pxVertical = 20px
```

---

# 3. table-layout ⭐⭐⭐

Controls how column widths are calculated.

Values

```
table-layout:auto;table-layout:fixed;
```

---

### auto (Default)

Columns adjust based on their content.

```
table{    table-layout:auto;}
```

---

### fixed ⭐⭐⭐

Columns have fixed widths.

```
table{    table-layout:fixed;}
```

Advantages

✔ Faster rendering

✔ Equal column widths

✔ Better for large tables

---

# 4. caption-side ⭐

Controls where the table caption appears.

Example

```
caption-side:top;
```

Values

```
caption-side:top;caption-side:bottom;
```

HTML

```
<table><caption>Student List</caption></table>
```

---

# Complete Example ⭐⭐⭐

```
table{width:100%;border-collapse:collapse;table-layout:fixed;}th,td{border:1px solid #ccc;padding:10px;text-align:left;}
```

This is a common starting style for tables.

---

# Which Properties Are Used Most? ⭐⭐⭐⭐⭐

|Property|Usage|
|---|---|
|border-collapse|⭐⭐⭐⭐⭐|
|table-layout|⭐⭐⭐|
|border-spacing|⭐⭐|
|caption-side|⭐|

---

# Quick Revision ⭐⭐⭐⭐⭐

### Border Collapse

```
border-collapse:collapse;
```

Merge borders.

---

### Border Spacing

```
border-spacing:10px;
```

Space between cells.

---

### Table Layout

```
table-layout:fixed;
```

Fixed column widths.

---

### Caption Position

```
caption-side:top;
```

Move caption.

---

# Most Used in Real Projects ⭐⭐⭐⭐⭐

```
1. border-collapse:collapse ⭐⭐⭐⭐⭐2. table-layout:fixed ⭐⭐⭐3. border-spacing ⭐⭐4. caption-side ⭐
```

---

## 💡 Full Stack Tip

The table styles you'll use most often are:

```
table{    width:100%;    border-collapse:collapse;}th,td{    border:1px solid #ddd;    padding:10px;}
```

This creates clean, readable tables and is commonly used in **admin dashboards**, **student records**, **billing systems**, and **reports**.

For responsive websites, you'll often combine tables with:

```
.table-container{    overflow-x:auto;}
```

This allows wide tables to scroll horizontally on smaller screens instead of breaking the layout.
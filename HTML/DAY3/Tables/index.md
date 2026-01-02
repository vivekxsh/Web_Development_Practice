

---

## 1. What is an HTML Table?

An HTML table is used to **display data in rows and columns**, similar to a spreadsheet.

Examples of when to use tables:

* Timetables
* Marks/grades
* Product comparison
* Reports and structured data

⚠️ **Tables are for data, not layout** (modern layouts use CSS like Flexbox or Grid).

---

## 2. Basic Table Structure

```html
<table>
  <tr>
    <td>Row 1, Column 1</td>
    <td>Row 1, Column 2</td>
  </tr>
  <tr>
    <td>Row 2, Column 1</td>
    <td>Row 2, Column 2</td>
  </tr>
</table>
```

### Tags explained:

| Tag       | Meaning           |
| --------- | ----------------- |
| `<table>` | Defines the table |
| `<tr>`    | Table row         |
| `<td>`    | Table data (cell) |

---

## 3. Table Headers (`<th>`)

Headers describe the columns or rows.

```html
<table>
  <tr>
    <th>Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Alice</td>
    <td>16</td>
  </tr>
</table>
```

### Differences:

| `<th>`              | `<td>`           |
| ------------------- | ---------------- |
| Header cell         | Normal data cell |
| Bold by default     | Normal text      |
| Centered by default | Left-aligned     |

---

## 4. Table Caption

Adds a title to the table.

```html
<table>
  <caption>Student Details</caption>
  <tr>
    <th>Name</th>
    <th>Class</th>
  </tr>
</table>
```

✔️ Improves **accessibility and readability**

---

## 5. Table Sections

HTML allows tables to be divided into logical sections.

```html
<table>
  <thead>
    <tr>
      <th>Subject</th>
      <th>Marks</th>
    </tr>
  </thead>

  <tbody>
    <tr>
      <td>Math</td>
      <td>90</td>
    </tr>
  </tbody>

  <tfoot>
    <tr>
      <td>Total</td>
      <td>90</td>
    </tr>
  </tfoot>
</table>
```

### Purpose:

| Section   | Use            |
| --------- | -------------- |
| `<thead>` | Header rows    |
| `<tbody>` | Main data      |
| `<tfoot>` | Summary/footer |

---

## 6. Rowspan and Colspan

### `colspan` – merge columns

```html
<td colspan="2">Merged Columns</td>
```

### `rowspan` – merge rows

```html
<td rowspan="2">Merged Rows</td>
```

### Example:

```html
<table border="1">
  <tr>
    <th>Name</th>
    <th colspan="2">Marks</th>
  </tr>
  <tr>
    <td>Alice</td>
    <td>Math</td>
    <td>90</td>
  </tr>
</table>
```

---

## 7. Table Borders (Old vs Modern Way)

### ❌ Old (HTML attribute – not recommended)

```html
<table border="1">
```

### ✅ Modern (CSS)

```html
<style>
  table, th, td {
    border: 1px solid black;
    border-collapse: collapse;
  }
</style>
```

---

## 8. Styling Tables with CSS

### Example:

```html
<style>
  table {
    width: 100%;
  }

  th {
    background-color: #333;
    color: white;
  }

  td, th {
    padding: 10px;
    text-align: center;
  }

  tr:nth-child(even) {
    background-color: #f2f2f2;
  }
</style>
```

### Common CSS properties:

| Property          | Use                   |
| ----------------- | --------------------- |
| `border-collapse` | Remove double borders |
| `padding`         | Space inside cells    |
| `text-align`      | Align text            |
| `nth-child()`     | Zebra stripes         |

---

## 9. Accessibility Best Practices ♿

```html
<th scope="col">Name</th>
<th scope="row">Alice</th>
```

### Tips:

* Use `<caption>`
* Use `<th>` instead of `<td>` for headers
* Use `scope="row"` or `scope="col"`
* Avoid tables for layout

---

## 10. Nested Tables (Allowed but Avoid if Possible)

```html
<table>
  <tr>
    <td>
      <table border="1">
        <tr>
          <td>Inner Table</td>
        </tr>
      </table>
    </td>
  </tr>
</table>
```

⚠️ Makes code harder to read and maintain.

---

## 11. Common Mistakes ❌

* Using tables for page layout
* Forgetting `<tr>`
* Mixing `<th>` and `<td>` incorrectly
* Not using CSS for styling
* Missing `<caption>`

---

## 12. Complete Example (Exam-Ready)

```html
<!DOCTYPE html>
<html>
<head>
  <title>HTML Table</title>
  <style>
    table {
      width: 60%;
      border-collapse: collapse;
    }
    th, td {
      border: 1px solid black;
      padding: 8px;
      text-align: center;
    }
    th {
      background-color: lightgray;
    }
  </style>
</head>
<body>

<table>
  <caption>Student Marks</caption>
  <thead>
    <tr>
      <th>Name</th>
      <th>Math</th>
      <th>Science</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Alice</td>
      <td>90</td>
      <td>85</td>
    </tr>
  </tbody>
</table>

</body>
</html>
```

---

## 13. Quick Revision Table 🧠

| Element     | Purpose         |
| ----------- | --------------- |
| `<table>`   | Table container |
| `<tr>`      | Row             |
| `<td>`      | Data cell       |
| `<th>`      | Header cell     |
| `<caption>` | Table title     |
| `rowspan`   | Merge rows      |
| `colspan`   | Merge columns   |

---


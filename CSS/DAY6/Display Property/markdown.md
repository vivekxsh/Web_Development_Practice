In CSS, the **`display`** property controls **how an element is rendered and how it participates in layout** (block, inline, grid, etc.).

Here are the **most important `display` values**, explained simply:

---

## Common `display` values

### 1. `block`

* Takes **full width** available
* Starts on a **new line**
* Can set width/height

**Examples:** `<div>`, `<p>`, `<h1>`

```css
div {
  display: block;
}
```

---

### 2. `inline`

* Takes **only as much width as needed**
* **Does not start** on a new line
* Cannot set width/height

**Examples:** `<span>`, `<a>`

```css
span {
  display: inline;
}
```

---

### 3. `inline-block`

* Behaves like inline
* Allows **width and height**
* Does not break line

```css
button {
  display: inline-block;
}
```

---

### 4. `none`

* **Removes element completely**
* No space is reserved

```css
.hidden {
  display: none;
}
```

---

## Layout display types

### 5. `flex`

* Enables **Flexbox layout**
* Used for one-dimensional layouts (row or column)

```css
.container {
  display: flex;
}
```

Common flex properties:

```css
justify-content: center;
align-items: center;
```

---

### 6. `grid`

* Enables **CSS Grid**
* Used for two-dimensional layouts

```css
.container {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}
```

---

## Table-related values

```css
display: table;
display: table-row;
display: table-cell;
```

Used to mimic table behavior without `<table>` tags.

---

## Other useful values

### 7. `contents`

* Removes the element itself
* Keeps its children in layout

```css
.wrapper {
  display: contents;
}
```

### 8. `inherit`

* Takes display value from parent

```css
.child {
  display: inherit;
}
```

---

## Quick comparison

| Value        | New Line | Width/Height | Layout Type |
| ------------ | -------- | ------------ | ----------- |
| block        | Yes      | Yes          | Normal      |
| inline       | No       | No           | Text-like   |
| inline-block | No       | Yes          | Hybrid      |
| none         | —        | —            | Removed     |
| flex         | Yes      | Yes          | Flexbox     |
| grid         | Yes      | Yes          | Grid        |

---

## 📦 `<div>` element in HTML

The **`<div>` (division) element** is a **block-level, non-semantic container** used to group HTML elements so they can be **styled or arranged with CSS** or **controlled with JavaScript**.

---

## 🔹 Basic syntax

```html
<div>
  Content goes here
</div>
```

---

## 🔹 Key characteristics

* Block-level element
* Starts on a **new line**
* Takes **full width** by default
* Has **no visual style** on its own
* Used mainly for **layout and grouping**

---

## 🔹 Why we use `<div>`

* Group elements together
* Apply CSS styles
* Create layouts (rows, columns, sections)
* Target content with JavaScript

Example:

```html
<div class="card">
  <h2>Title</h2>
  <p>Description text</p>
</div>
```

---

## 🔹 `<div>` with CSS

```html
<div class="box">Hello</div>
```

```css
.box {
  width: 200px;
  padding: 10px;
  border: 2px solid black;
  background-color: lightblue;
}
```

---

## 🔹 `<div>` vs semantic elements

| `<div>`          | Semantic tags      |
| ---------------- | ------------------ |
| No meaning       | Have meaning       |
| Generic          | Descriptive        |
| Used for styling | Used for structure |

Semantic alternatives:

* `<header>`
* `<nav>`
* `<section>`
* `<article>`
* `<footer>`

👉 **Use semantic tags when possible; use `<div>` when no suitable semantic tag exists.**

---

## 🔹 `<div>` vs `<span>`

| `<div>`     | `<span>`      |
| ----------- | ------------- |
| Block-level | Inline        |
| Full width  | Content width |
| Layout      | Text styling  |

---

## 🔹 Common attributes

* `class` – for styling
* `id` – unique identifier
* `style` – inline CSS
* `title` – tooltip

Example:

```html
<div id="main" class="container" title="Main section">
  Content
</div>
```

---

## 🔹 Important notes

* Overusing `<div>` is called **“div soup”** ❌
* HTML5 prefers **semantic structure**
* `<div>` is still essential for complex layouts

---

### 📌 Exam-ready definition

> **`<div>` is a block-level container used to group elements for styling and layout purposes.**



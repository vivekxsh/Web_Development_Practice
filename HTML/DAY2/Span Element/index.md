## 🏷️ `<span>` element in HTML

The **`<span>` element** is an **inline, non-semantic container** used to **style or manipulate small parts of text or inline content** without breaking the line.

---

## 🔹 Basic syntax

```html
<span>Text here</span>
```

---

## 🔹 Key characteristics

* **Inline element**
* Does **not start a new line**
* Takes **only the width of its content**
* Has **no default styling**
* Used mainly for **text-level styling**

---

## 🔹 Why we use `<span>`

* Apply styles to part of a sentence
* Target text with CSS or JavaScript
* Highlight or modify specific words

Example:

```html
<p>
  This is <span class="highlight">important</span> text.
</p>
```

```css
.highlight {
  color: red;
  font-weight: bold;
}
```

---

## 🔹 `<span>` vs `<div>`

| `<span>`         | `<div>`         |
| ---------------- | --------------- |
| Inline           | Block-level     |
| Used inside text | Used for layout |
| Small content    | Large sections  |

---

## 🔹 Common attributes

* `class` – for styling
* `id` – for JavaScript targeting
* `style` – inline CSS
* `title` – tooltip

Example:

```html
<span id="price" style="color: green;">$99</span>
```

---

## 🔹 Styling behavior

By default, `<span>`:

* Cannot set width/height
* Accepts left & right margin/padding

You can change behavior using CSS:

```css
span {
  display: inline-block;
}
```

---

## 🔹 Semantic alternatives (when applicable)

Instead of `<span>`, use:

* `<strong>` for importance
* `<em>` for emphasis
* `<mark>` for highlight

👉 Use `<span>` **only when no semantic tag fits**.

---

### 📌 Exam-ready definition

> **`<span>` is an inline container used to style or manipulate a part of text without changing the layout.**

---


## ➖ `<hr>` tag in HTML

The **`<hr>` (horizontal rule) tag** is used to **separate content** in an HTML page.
In HTML5, it represents a **thematic break** between sections, not just a line.

---

## 🔹 Basic syntax

```html
<hr>
```

👉 `<hr>` is a **void (self-closing) element** — it has **no closing tag**.

---

## 🔹 Purpose of `<hr>`

* Separates sections of content
* Shows a change in topic
* Visually displays a horizontal line by default

Example:

```html
<p>Introduction</p>
<hr>
<p>Details</p>
```

---

## 🔹 Key characteristics

* Block-level element
* Starts on a new line
* Has default styling (horizontal line)
* Semantic meaning: **thematic break**

---

## 🔹 Styling `<hr>` with CSS

You can change its appearance using CSS:

```html
<hr class="line">
```

```css
.line {
  border: none;
  height: 2px;
  background-color: black;
  width: 50%;
}
```

---

## 🔹 `<hr>` vs `<br>`

| `<hr>`             | `<br>`              |
| ------------------ | ------------------- |
| Separates sections | Breaks a line       |
| Semantic meaning   | No semantic meaning |
| Visible line       | No line             |

---

## 🔹 Common attributes

* `class`
* `id`
* `style`
* Global HTML attributes

Example:

```html
<hr id="divider">
```

---

## 🔹 Important notes

* Do **not** use `<hr>` just for decoration
* Use it when there is a **change in topic**
* For spacing only, use **CSS margin or padding**

---

### 📌 Exam-ready definition

> **`<hr>` tag is used to define a thematic break between sections of content in HTML.**

---


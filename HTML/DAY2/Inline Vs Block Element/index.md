In HTML, elements are mainly divided into **block-level** and **inline** elements based on how they appear and behave on a web page.

---

## 🧱 Block-level elements

### What they do

* Always start on a **new line**
* Take up the **full width** available
* Can contain **inline and other block elements**

### Examples

```html
<div>Div</div>
<p>Paragraph</p>
<h1>Heading</h1>
<section>Section</section>
```

### Common block elements

* `<div>`
* `<p>`
* `<h1>` to `<h6>`
* `<header>`, `<footer>`
* `<section>`, `<article>`
* `<nav>`
* `<ul>`, `<ol>`, `<li>`
* `<table>`
* `<form>`

---

## 🔤 Inline elements

### What they do

* Do **not** start on a new line
* Take up **only as much width as needed**
* Usually contain **text or other inline elements**

### Examples

```html
<span>Span</span>
<a href="#">Link</a>
<img src="img.jpg">
<strong>Bold</strong>
```

### Common inline elements

* `<span>`
* `<a>`
* `<img>`
* `<strong>`
* `<em>`
* `<b>`, `<i>`, `<u>`
* `<small>`
* `<sub>`, `<sup>`

---

## ⚖️ Key differences (table)

| Feature        | Block          | Inline                 |
| -------------- | -------------- | ---------------------- |
| New line       | Yes            | No                     |
| Width          | Full width     | Content width          |
| Height & width | Can be set     | Cannot normally be set |
| Margin/padding | All sides      | Left & right only      |
| Can contain    | Block + inline | Inline only            |

---

## 🔄 Inline-block (CSS concept)

```css
display: inline-block;
```

### Why use it?

* Behaves like **inline** (same line)
* Accepts **width, height, margin, padding** like block

Example:

```html
<button>OK</button>
<button>Cancel</button>
```

---

## 📝 Important notes

* You can change behavior using CSS:

```css
display: block;
display: inline;
```

* `<img>` is inline but behaves like inline-block
* HTML5 focuses more on **semantic meaning**, CSS controls layout

---

### 📌 Exam tip

> **Block elements start on a new line; inline elements do not.**


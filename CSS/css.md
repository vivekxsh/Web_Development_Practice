**CSS in Web Development** 🎨

**CSS (Cascading Style Sheets)** is the language used to control how a website looks. While **HTML** structures the content and **JavaScript** adds behavior, **CSS handles design and layout**.

---

## What CSS Does

CSS lets you:

* Change **colors, fonts, and sizes**
* Control **layout** (positioning, spacing, alignment)
* Create **responsive designs** for phones, tablets, and desktops
* Add **animations and transitions**
* Improve **user experience** and visual appeal

---

## How CSS Works

CSS applies styles to HTML elements using **selectors**.

```css
p {
  color: blue;
  font-size: 16px;
}
```

This means:

* Select all `<p>` (paragraph) elements
* Make the text blue
* Set font size to 16 pixels

---

## Ways to Use CSS

### 1. Inline CSS (not recommended)

```html
<p style="color:red;">Hello</p>
```

### 2. Internal CSS

```html
<style>
  p { color: red; }
</style>
```

### 3. External CSS (best practice)

```html
<link rel="stylesheet" href="style.css">
```

---

## Core CSS Concepts

### Selectors

* Element: `div`
* Class: `.box`
* ID: `#header`

### Box Model

Every element has:

* **Content**
* **Padding**
* **Border**
* **Margin**

### Layout Systems

* **Flexbox** – one-dimensional layouts (rows or columns)
* **Grid** – two-dimensional layouts (rows and columns)

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

---

## Responsive Design

CSS adapts layouts to different screen sizes using **media queries**.

```css
@media (max-width: 600px) {
  body {
    background-color: lightgray;
  }
}
```

---

## Modern CSS Features

* **CSS Variables**
* **Animations & Transitions**
* **Pseudo-classes** (`:hover`, `:focus`)
* **Frameworks** (Bootstrap, Tailwind CSS)

---

## Why CSS Is Important

✔ Makes websites visually attractive
✔ Improves usability and accessibility
✔ Separates design from content
✔ Essential for professional web development

---

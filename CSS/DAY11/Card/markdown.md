Bootstrap **cards** are a flexible, all-purpose UI component for displaying content in a clean, boxed layout. Think of them as the modern replacement for panels, wells, and thumbnails.

Here’s the quick, practical rundown 👇

---

## What is a Bootstrap card?

A **card** is a container that can hold:

* text
* images
* buttons
* lists
* headers & footers

They’re commonly used for:

* product listings
* blog previews
* user profiles
* dashboards

---

## Basic card structure

```html
<div class="card" style="width: 18rem;">
  <img src="image.jpg" class="card-img-top" alt="...">

  <div class="card-body">
    <h5 class="card-title">Card title</h5>
    <p class="card-text">Some quick example text.</p>
    <a href="#" class="btn btn-primary">Go somewhere</a>
  </div>
</div>
```

---

## Common card parts

| Class          | Purpose        |
| -------------- | -------------- |
| `card`         | Main wrapper   |
| `card-body`    | Main content   |
| `card-title`   | Title text     |
| `card-text`    | Paragraph text |
| `card-img-top` | Image at top   |
| `card-header`  | Header section |
| `card-footer`  | Footer section |

---

## Card with header & footer

```html
<div class="card">
  <div class="card-header">
    Featured
  </div>

  <div class="card-body">
    <h5 class="card-title">Special title</h5>
    <p class="card-text">More content here.</p>
  </div>

  <div class="card-footer text-muted">
    2 days ago
  </div>
</div>
```

---

## Card layouts (very common)

### Cards in a grid

```html
<div class="row">
  <div class="col-md-4">
    <div class="card">...</div>
  </div>
  <div class="col-md-4">
    <div class="card">...</div>
  </div>
</div>
```

### Card groups

```html
<div class="card-group">
  <div class="card">...</div>
  <div class="card">...</div>
  <div class="card">...</div>
</div>
```

---

## Styling cards

* Background: `bg-primary`, `bg-light`, etc.
* Text: `text-white`, `text-dark`
* Borders: `border`, `border-danger`
* Shadows: `shadow`, `shadow-lg`

Example:

```html
<div class="card shadow-lg border-0">
```

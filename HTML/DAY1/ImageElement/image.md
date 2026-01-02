In HTML, the **image element** is `<img>`. It’s used to display images on a web page.

---

## Basic syntax

```html
<img src="image.jpg" alt="Description of the image">
```

### Key attributes

* **`src`** (required)
  The path or URL to the image.

  ```html
  <img src="photos/cat.png">
  ```

* **`alt`** (required for accessibility)
  Text shown if the image can’t load and read by screen readers.

  ```html
  <img src="cat.png" alt="A gray cat sleeping on a sofa">
  ```

* **`width`** and **`height`**
  Set the image size (in pixels by default).

  ```html
  <img src="cat.png" alt="Cat" width="200" height="150">
  ```

---

## Common additional attributes

* **`title`** – Tooltip text when hovering

  ```html
  <img src="cat.png" alt="Cat" title="My pet cat">
  ```

* **`loading`** – Controls lazy loading

  ```html
  <img src="cat.png" alt="Cat" loading="lazy">
  ```

* **`srcset`** and **`sizes`** – Responsive images

  ```html
  <img 
    src="cat-small.jpg"
    srcset="cat-small.jpg 480w, cat-large.jpg 800w"
    sizes="(max-width: 600px) 480px, 800px"
    alt="Cat">
  ```

---

## Styling images with CSS

```html
<img src="cat.png" alt="Cat" class="profile-pic">
```

```css
.profile-pic {
  width: 150px;
  border-radius: 50%;
}
```

---

## Important notes

* `<img>` is a **self-closing (void) element** — it has no closing tag.
* Always use `alt` for **accessibility and SEO**.
* Images are **inline elements** by default.

---


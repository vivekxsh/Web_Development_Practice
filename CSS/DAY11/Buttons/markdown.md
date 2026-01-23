Bootstrap doesn’t have a single component literally called **“About Button”**, but it *does* give you several **button components** you’d typically use for an “About” action (like linking to an About page or opening a modal).

Here’s a quick, practical breakdown 👇

---

## 1. Basic Bootstrap Button

This is the most common “About” button:

```html
<button type="button" class="btn btn-primary">
  About
</button>
```

Common variants:

* `btn-primary`
* `btn-secondary`
* `btn-success`
* `btn-outline-primary`
* `btn-link`

Example:

```html
<button class="btn btn-outline-info">About Us</button>
```

---

## 2. “About” Button as a Link

If “About” navigates to another page:

```html
<a href="/about" class="btn btn-primary">
  About Us
</a>
```

Bootstrap treats links and buttons the same visually.



---

## 3. Button Sizes (if needed)

```html
<button class="btn btn-primary btn-lg">About</button>
<button class="btn btn-primary btn-sm">About</button>
```

---

## 4. Icon Button (Optional, looks nice)

If you’re using Bootstrap Icons:

```html
<button class="btn btn-secondary">
  <i class="bi bi-info-circle"></i> About
</button>
```

---


Bootstrap **button groups** let you **group multiple buttons together** on a single line—great for toolbars, toggles, or grouped actions. Here’s the essentials 👇

---

## 1. Basic Button Group

```html
<div class="btn-group" role="group" aria-label="Basic example">
  <button type="button" class="btn btn-primary">Left</button>
  <button type="button" class="btn btn-primary">Middle</button>
  <button type="button" class="btn btn-primary">Right</button>
</div>
```

---

## 2. Button Group Sizes

```html
<div class="btn-group btn-group-lg">
  <button class="btn btn-secondary">Large</button>
  <button class="btn btn-secondary">Large</button>
</div>

<div class="btn-group btn-group-sm">
  <button class="btn btn-secondary">Small</button>
  <button class="btn btn-secondary">Small</button>
</div>
```

---

## 3. Vertical Button Group

```html
<div class="btn-group-vertical" role="group">
  <button class="btn btn-primary">Top</button>
  <button class="btn btn-primary">Middle</button>
  <button class="btn btn-primary">Bottom</button>
</div>
```

---

## 4. Button Group with Links

```html
<div class="btn-group" role="group">
  <a href="#" class="btn btn-outline-primary">Home</a>
  <a href="#" class="btn btn-outline-primary">About</a>
  <a href="#" class="btn btn-outline-primary">Contact</a>
</div>
```

---

## 5. Button Group with Checkboxes / Radio Buttons (Toggle Buttons)

Useful for filters & settings 👌

### Radio Toggle

```html
<div class="btn-group" role="group">
  <input type="radio" class="btn-check" name="options" id="option1" checked>
  <label class="btn btn-outline-primary" for="option1">Option 1</label>

  <input type="radio" class="btn-check" name="options" id="option2">
  <label class="btn btn-outline-primary" for="option2">Option 2</label>
</div>
```

### Checkbox Toggle

```html
<div class="btn-group" role="group">
  <input type="checkbox" class="btn-check" id="check1">
  <label class="btn btn-outline-success" for="check1">Bold</label>

  <input type="checkbox" class="btn-check" id="check2">
  <label class="btn btn-outline-success" for="check2">Italic</label>
</div>
```

---

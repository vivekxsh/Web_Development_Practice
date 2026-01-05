**Inheritance in CSS** means that some CSS property values applied to a parent element are automatically passed down to its child elements.

---

## 1. How CSS Inheritance Works

When you style a parent element, certain properties **cascade down** to its children unless overridden.

### Example

```css
div {
  color: blue;
}
```

```html
<div>
  <p>This text will be blue</p>
  <span>This text will also be blue</span>
</div>
```

Both `<p>` and `<span>` inherit the `color` from the `<div>`.

---

## 2. Properties That Are Inherited by Default

Common inherited properties include:

### Text & Font

* `color`
* `font-family`
* `font-size`
* `font-style`
* `font-weight`
* `letter-spacing`
* `line-height`
* `text-align`
* `text-transform`
* `visibility`

---

## 3. Properties That Are NOT Inherited

Most layout and box-model properties **do not inherit**:

* `margin`
* `padding`
* `border`
* `width`
* `height`
* `background`
* `display`
* `position`

Example:

```css
div {
  background-color: yellow;
}
```

The child elements **will not** inherit the background color.

---

## 4. Forcing Inheritance

You can force inheritance using the `inherit` keyword.

```css
p {
  border: inherit;
}
```

If the parent has a border, the `<p>` will inherit it.

---

## 5. Preventing Inheritance

You can stop inheritance by using:

### `initial`

Resets to the default browser value.

```css
p {
  color: initial;
}
```

### `unset`

* Acts as `inherit` if the property is normally inherited
* Acts as `initial` if it is not

```css
p {
  color: unset;
}
```

---

## 6. Inheritance vs Cascade vs Specificity

* **Inheritance**: values passed from parent to child
* **Cascade**: decides which rule applies when multiple rules target the same element
* **Specificity**: determines priority among selectors

---

## 7. Quick Summary

| Concept     | Meaning                      |
| ----------- | ---------------------------- |
| Inheritance | Child gets value from parent |
| `inherit`   | Force inheritance            |
| `initial`   | Default browser value        |
| `unset`     | Smart reset                  |

---

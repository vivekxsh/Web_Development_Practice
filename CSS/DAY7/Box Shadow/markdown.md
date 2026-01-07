In CSS, **`box-shadow`** adds shadow effects around elements like cards, buttons, and modals.

---

## 1. Basic syntax

```css
box-shadow: offset-x offset-y blur-radius spread-radius color;
```

Example:

```css
.box {
  box-shadow: 10px 10px 20px rgba(0, 0, 0, 0.3);
}
```

---

## 2. Shadow parameters explained

| Value           | Meaning                              |
| --------------- | ------------------------------------ |
| `offset-x`      | Horizontal shadow (right = positive) |
| `offset-y`      | Vertical shadow (down = positive)    |
| `blur-radius`   | How soft the shadow is               |
| `spread-radius` | Size expansion/shrink                |
| `color`         | Shadow color                         |

---

## 3. Simple shadows

```css
.card {
  box-shadow: 0 4px 8px #00000033;
}
```

---

## 4. Multiple shadows

You can stack shadows using commas:

```css
.box {
  box-shadow:
    0 2px 5px rgba(0,0,0,0.2),
    0 10px 20px rgba(0,0,0,0.15);
}
```

---

## 5. Inset shadows

Creates a shadow **inside** the element.

```css
.box {
  box-shadow: inset 0 2px 5px rgba(0, 0, 0, 0.3);
}
```

---

## 6. Box-shadow vs drop-shadow

### `box-shadow`

* Applies to the element’s box
* Respects `border-radius`
* Works on block elements

### `filter: drop-shadow()`

```css
img {
  filter: drop-shadow(0 5px 10px rgba(0,0,0,0.4));
}
```

* Works on transparent images
* Follows the shape of the image

---

## 7. Hover shadow effect

```css
.card {
  transition: box-shadow 0.3s ease, transform 0.3s ease;
  box-shadow: 0 2px 5px rgba(0,0,0,0.2);
}

.card:hover {
  box-shadow: 0 10px 25px rgba(0,0,0,0.3);
  transform: translateY(-5px);
}
```

---

## 8. Material-style shadow levels

```css
.shadow-sm {
  box-shadow: 0 1px 3px rgba(0,0,0,0.12);
}

.shadow-md {
  box-shadow: 0 4px 6px rgba(0,0,0,0.16);
}

.shadow-lg {
  box-shadow: 0 10px 20px rgba(0,0,0,0.25);
}
```

---

## 9. Common mistakes

❌ Too much blur → muddy UI
❌ Pure black shadows → look unnatural
✅ Use **rgba** or alpha hex
✅ Combine with `transform` for depth

---

### Quick tip

For modern UI:

```css
box-shadow: 0 8px 30px rgba(0,0,0,0.12);
```


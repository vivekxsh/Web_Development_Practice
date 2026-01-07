In CSS, **alpha** and **opacity** both control transparency, but they’re used in slightly different ways.

---

## 1. `opacity` (element-level transparency)

The `opacity` property sets the transparency of an **entire element**, including all its children.

```css
.box {
  opacity: 0.5; /* 0 = fully transparent, 1 = fully opaque */
}
```

### Key points

* Range: `0` to `1`
* Affects **everything inside** the element (text, images, children)
* Common values:

  * `0` → invisible
  * `0.5` → 50% transparent
  * `1` → fully visible

⚠️ If you want only the background to be transparent (not the text), don’t use `opacity`.

---

## 2. Alpha channel (color-level transparency)

The **alpha channel** controls transparency of a **specific color**, not the whole element.

### a) `rgba()`

```css
.box {
  background-color: rgba(255, 0, 0, 0.5); /* red at 50% opacity */
}
```

Format:

```css
rgba(red, green, blue, alpha)
```

---

### b) `hsla()`

```css
.box {
  background-color: hsla(120, 100%, 50%, 0.3);
}
```

---

### c) Modern `rgb()` with alpha (recommended)

```css
.box {
  background-color: rgb(255 0 0 / 50%);
}
```

or

```css
.box {
  background-color: rgb(255 0 0 / 0.5);
}
```

---

### d) Hex with alpha

```css
.box {
  background-color: #ff000080;
}
```

* Last two hex digits = alpha
* `80` ≈ 50% opacity

---

## 3. Opacity vs Alpha (important difference)

| Feature                      | `opacity`     | Alpha (RGBA/HSLA/etc.) |
| ---------------------------- | ------------- | ---------------------- |
| Affects children             | ✅ Yes         | ❌ No                   |
| Affects whole element        | ✅ Yes         | ❌ No                   |
| Background-only transparency | ❌ No          | ✅ Yes                  |
| Common use                   | Fade elements | Transparent colors     |

---

## 4. Example comparison

```css
/* Fades everything */
.card {
  opacity: 0.5;
}

/* Only background is transparent */
.card {
  background-color: rgba(0, 0, 0, 0.5);
  color: white;
}
```

---

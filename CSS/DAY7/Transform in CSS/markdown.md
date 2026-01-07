In CSS, **`transform`** lets you visually change an element’s shape, position, or orientation **without affecting document layout**. It’s commonly used for animations, hover effects, and UI interactions.

---

## 1. Basic syntax

```css
transform: function(value);
```

Example:

```css
.box {
  transform: rotate(45deg);
}
```

---

## 2. Common transform functions

### a) `translate()` – move element

```css
transform: translate(50px, 20px);
```

* `translateX(50px)`
* `translateY(20px)`
* `translate3d(x, y, z)`

---

### b) `scale()` – resize element

```css
transform: scale(1.2);
```

* `scaleX(1.5)`
* `scaleY(0.8)`

---

### c) `rotate()` – rotate element

```css
transform: rotate(30deg);
```

* `rotateX(45deg)`
* `rotateY(45deg)` (3D)

---

### d) `skew()` – tilt element

```css
transform: skew(20deg, 10deg);
```

* `skewX(20deg)`
* `skewY(10deg)`

---

## 3. Multiple transforms

Transforms are applied **from right to left**.

```css
transform: translateX(50px) rotate(45deg) scale(1.2);
```

Order matters!

---

## 4. Transform + transition (very common)

```css
.card {
  transition: transform 0.3s ease;
}

.card:hover {
  transform: scale(1.05) translateY(-10px);
}
```

---

## 5. `transform-origin`

Controls the point around which the transform happens.

```css
transform-origin: center;
```

Examples:

```css
transform-origin: top left;
transform-origin: 50% 50%;
```

---

## 6. 3D transforms

```css
.container {
  perspective: 800px;
}

.box {
  transform: rotateY(45deg);
}
```

Other 3D functions:

* `translateZ(50px)`
* `scaleZ(1.2)`

---

## 7. Performance benefits

✅ Fast and smooth
✅ Does NOT cause reflow
✅ Best used with `transition` or `animation`

**Best properties to animate:**

* `transform`
* `opacity`

---

## 8. Common real-world examples

### Button hover effect

```css
.btn:hover {
  transform: translateY(-3px);
}
```

### Image zoom on hover

```css
img:hover {
  transform: scale(1.1);
}
```

### Center element perfectly

```css
.box {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```

---


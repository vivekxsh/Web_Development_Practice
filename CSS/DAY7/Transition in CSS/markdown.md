In CSS, **`transition`** lets you smoothly animate changes between property values (instead of instant jumps).

---

## 1. Basic syntax

```css
transition: property duration timing-function delay;
```

Example:

```css
.box {
  width: 100px;
  transition: width 0.3s ease;
}

.box:hover {
  width: 200px;
}
```

---

## 2. Common transition properties

### a) `transition-property`

Which CSS property should animate.

```css
transition-property: background-color;
```

### b) `transition-duration`

How long the transition takes.

```css
transition-duration: 0.5s;
```

### c) `transition-timing-function`

Controls animation speed curve.

```css
transition-timing-function: ease;
```

Common values:

* `ease` (default)
* `linear`
* `ease-in`
* `ease-out`
* `ease-in-out`
* `cubic-bezier(...)`

---

### d) `transition-delay`

Wait time before animation starts.

```css
transition-delay: 0.2s;
```

---

## 3. Shorthand example

```css
.button {
  background-color: blue;
  color: white;
  transition: background-color 0.3s ease, transform 0.2s ease;
}

.button:hover {
  background-color: red;
  transform: scale(1.1);
}
```

---

## 4. Transition all properties

```css
.box {
  transition: all 0.4s ease;
}
```

⚠️ Not recommended for performance—better to specify exact properties.

---

## 5. Properties that CAN be transitioned

✅ Good (performance-friendly):

* `opacity`
* `transform`
* `color`
* `background-color`

⚠️ Less optimal:

* `width`
* `height`
* `margin`
* `padding`

❌ Cannot transition:

* `display`
* `position`
* `float`

---

## 6. Hover fade example (opacity)

```css
.card {
  opacity: 0.5;
  transition: opacity 0.3s ease;
}

.card:hover {
  opacity: 1;
}
```

---

## 7. Multiple transitions

```css
.box {
  transition:
    background-color 0.3s ease,
    box-shadow 0.3s ease,
    transform 0.2s ease;
}
```

---

## 8. Best practices

* Define `transition` on the **base state**, not `:hover`
* Prefer `transform` & `opacity` for smooth animations
* Avoid `transition: all` in production
* Use short durations (0.2s–0.4s) for UI interactions

---

### Quick example (real-world button)

```css
.btn {
  padding: 10px 20px;
  background: #007bff;
  transition: background 0.3s ease, transform 0.2s ease;
}

.btn:hover {
  background: #0056b3;
  transform: translateY(-2px);
}
```


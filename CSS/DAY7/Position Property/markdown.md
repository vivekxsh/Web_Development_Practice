
---

## The 5 Position Values (that actually matter)

### 1️⃣ `static` (default)

```css
div {
  position: static;
}
```

* Normal document flow
* **Top/left/right/bottom do nothing**
* You almost never set this explicitly

🧠 Think: *“Just behave normally.”*

---

### 2️⃣ `relative`

```css
.box {
  position: relative;
  top: 10px;
  left: 20px;
}
```

* Element stays in the normal flow
* Moves **relative to its original position**
* Creates a **positioning context for absolute children**

🧠 Think: *“Move myself a bit, but keep my space.”*

✅ Very commonly used as a parent for `absolute`

---

### 3️⃣ `absolute`

```css
.child {
  position: absolute;
  top: 0;
  right: 0;
}
```

* Removed from normal document flow
* Positioned **relative to the nearest positioned ancestor**
* If no ancestor has `position: relative | absolute | fixed`, it uses `<body>`

🧠 Think: *“Stick me exactly here.”*

📌 Usually paired with:

```css
.parent {
  position: relative;
}
```

---

### 4️⃣ `fixed`

```css
.header {
  position: fixed;
  top: 0;
}
```

* Removed from normal flow
* Positioned **relative to the viewport**
* Stays in place when scrolling

🧠 Think: *“Glue me to the screen.”*

📌 Used for navbars, chat buttons, cookies banners

---

### 5️⃣ `sticky`

```css
.nav {
  position: sticky;
  top: 0;
}
```

* Hybrid of `relative` + `fixed`
* Scrolls normally, then **sticks** at a point
* Requires a `top`, `left`, etc.

🧠 Think: *“Scroll… scroll… okay I’m stuck now.”*

⚠️ Won’t work if parent has `overflow: hidden`

---

## Quick Comparison Table

| Position | In flow | Moves with scroll | Relative to               |
| -------- | ------- | ----------------- | ------------------------- |
| static   | ✅       | ✅                 | normal flow               |
| relative | ✅       | ✅                 | itself                    |
| absolute | ❌       | ✅                 | nearest positioned parent |
| fixed    | ❌       | ❌                 | viewport                  |
| sticky   | ✅       | ❌ (after stick)   | parent + viewport         |

---

## Most Common Real-World Pattern

```css
.card {
  position: relative;
}

.badge {
  position: absolute;
  top: 8px;
  right: 8px;
}
```

📍 Result: badge sticks to the corner of the card.

---

## Bonus: `z-index`

Only works on **positioned elements** (`relative`, `absolute`, `fixed`, `sticky`)

```css
.modal {
  position: fixed;
  z-index: 999;
}
```

Higher number = closer to the user.

---

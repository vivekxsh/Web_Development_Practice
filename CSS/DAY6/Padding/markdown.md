In CSS, **padding** is the space **inside an element**, between its **content** and its **border**.

Think of it like this:

```
[ border ]
  [ padding ]
    content
```

---

## Basic padding

```css
.box {
  padding: 20px;
}
```

➡ Adds **20px space on all sides** inside the element.

---

## Padding on each side

```css
.box {
  padding-top: 10px;
  padding-right: 20px;
  padding-bottom: 30px;
  padding-left: 40px;
}
```

---

## Shorthand padding (most common)

### 1 value

```css
padding: 20px;
```

All sides = 20px

---

### 2 values

```css
padding: 10px 20px;
```

* Top & Bottom = 10px
* Left & Right = 20px

---

### 3 values

```css
padding: 10px 20px 30px;
```

* Top = 10px
* Left & Right = 20px
* Bottom = 30px

---

### 4 values

```css
padding: 10px 20px 30px 40px;
```

**Order:** top → right → bottom → left (TRBL)

---

## Visual example

```html
<div class="box">Hello</div>
```

```css
.box {
  background: #4caf50;
  padding: 20px;
  color: white;
}
```

**Looks like:**
A green box where the word **Hello** is **not touching the edges** — it has breathing room 🫁

---

## Padding vs Margin (important!)

| Padding               | Margin                     |
| --------------------- | -------------------------- |
| Inside space          | Outside space              |
| Affects background    | Does NOT affect background |
| Pushes content inward | Pushes elements apart      |

```css
padding: 20px; /* inside */
margin: 20px;  /* outside */
```

---

## Padding and width (box model)

```css
.box {
  width: 200px;
  padding: 20px;
}
```

👉 Actual size becomes **240px** (200 + 20 + 20)

### Fix with `box-sizing`

```css
.box {
  box-sizing: border-box;
}
```

Now padding is included **inside** the width 👍

---

## Padding with percentages

```css
.box {
  padding: 10%;
}
```

📌 Percentage padding is based on the **width of the parent**, not height (common confusion).

---

## Common beginner mistakes ❌

* Forgetting units: `padding: 10;` ❌
* Using padding instead of margin
* Not understanding box size changes

---

In CSS, **margin** is the space **outside an element**, used to create distance **between elements**.

Think of it like this:

```
content
  padding
    border
      margin   ← outside space
```

---

## Basic margin

```css
.box {
  margin: 20px;
}
```

➡ Adds **20px space on all sides** outside the element.

---

## Margin on each side

```css
.box {
  margin-top: 10px;
  margin-right: 20px;
  margin-bottom: 30px;
  margin-left: 40px;
}
```

---

## Shorthand margin

### 1 value

```css
margin: 20px;
```

All sides = 20px

---

### 2 values

```css
margin: 10px 20px;
```

* Top & Bottom = 10px
* Left & Right = 20px

---

### 3 values

```css
margin: 10px 20px 30px;
```

* Top = 10px
* Left & Right = 20px
* Bottom = 30px

---

### 4 values (TRBL rule)

```css
margin: 10px 20px 30px 40px;
```

Top → Right → Bottom → Left

---

## Visual example

```html
<div class="box"></div>
<div class="box"></div>
```

```css
.box {
  width: 100px;
  height: 60px;
  background: #2196f3;
  margin: 20px;
}
```

**Looks like:**
Two blue boxes with **space between them**

---

## Auto margin (centering)

```css
.box {
  width: 200px;
  margin: 0 auto;
}
```

➡ Centers the element **horizontally**

---

## Negative margin

```css
.box {
  margin-top: -20px;
}
```

⚠️ Pulls elements **closer or overlapping**
Use carefully!

---

## Margin collapsing (important concept)

Vertical margins can **collapse**:

```css
h1 {
  margin-bottom: 20px;
}

p {
  margin-top: 30px;
}
```

👉 Space between them is **30px**, not 50px.

📌 Happens with **top & bottom margins**, not left/right.

---

## Margin vs Padding (quick recap)

| Margin                | Padding               |
| --------------------- | --------------------- |
| Outside space         | Inside space          |
| Transparent           | Affects background    |
| Pushes elements apart | Pushes content inward |

---

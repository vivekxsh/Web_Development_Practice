

---

## **1. Absolute Units** 📏

Absolute units are **fixed** and **don’t change** based on screen size.

| Unit | Description                             | Example            |
| ---- | --------------------------------------- | ------------------ |
| `px` | Pixels – 1px = 1 screen pixel           | `font-size: 16px;` |
| `pt` | Points – mostly for print, 1pt ≈ 1.33px | `font-size: 12pt;` |
| `cm` | Centimeters                             | `width: 5cm;`      |
| `mm` | Millimeters                             | `height: 30mm;`    |
| `in` | Inches                                  | `width: 2in;`      |
| `pc` | Picas – mostly print, 1pc = 12pt        | `margin: 2pc;`     |

💡 **Tip:** For web design, **`px`** is the most commonly used.

---

## **2. Relative Units** 🔄

Relative units **adapt to other sizes**, like parent elements or the viewport.

| Unit   | Description                           | Example                                     |
| ------ | ------------------------------------- | ------------------------------------------- |
| `%`    | Percentage of parent element          | `width: 50%;`                               |
| `em`   | Relative to **current font size**     | `font-size: 2em;` → 2 × parent font size    |
| `rem`  | Relative to **root (html) font size** | `font-size: 1.5rem;` → 1.5 × root font size |
| `vw`   | 1% of **viewport width**              | `width: 50vw;`                              |
| `vh`   | 1% of **viewport height**             | `height: 50vh;`                             |
| `vmin` | 1% of **smaller viewport dimension**  | `font-size: 5vmin;`                         |
| `vmax` | 1% of **larger viewport dimension**   | `font-size: 5vmax;`                         |

💡 **Tip:** Use `em`/`rem` for **responsive fonts**, and `vw`/`vh` for **full-page layouts**.

---

## **3. Keywords**

Some CSS properties accept keywords instead of numbers.

| Property       | Example                               |
| -------------- | ------------------------------------- |
| `font-size`    | `small`, `medium`, `large`, `x-large` |
| `width/height` | `auto`, `max-content`, `min-content`  |

---

## **Absolute vs Relative**

| Type     | Pros            | Cons                         |
| -------- | --------------- | ---------------------------- |
| Absolute | Precise control | Doesn’t adapt to screen size |
| Relative | Responsive      | Slightly less precise        |

---

## **Example Using Different Units**

```css
div {
  width: 50%;           /* 50% of parent */
  height: 30vh;         /* 30% of viewport height */
  padding: 2rem;        /* 2 × root font size */
  font-size: 16px;      /* fixed font size */
}
```

✅ **Effect:** The `div` adapts to screen size, but text stays readable.

---

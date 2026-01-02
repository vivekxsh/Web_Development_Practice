## 🔽 Subscript and 🔼 Superscript tags in HTML

HTML provides **two special inline tags** to display text **below or above the normal text line**.

---

## 🔽 `<sub>` — Subscript

### What it does

* Displays text **slightly below** the normal line
* Commonly used in **chemical formulas** and **mathematics**

### Syntax

```html
<sub>text</sub>
```

### Example

```html
H<sub>2</sub>O
```

**Output:** H₂O

---

## 🔼 `<sup>` — Superscript

### What it does

* Displays text **slightly above** the normal line
* Used for **powers, exponents, footnotes, and math**

### Syntax

```html
<sup>text</sup>
```

### Example

```html
x<sup>2</sup>
```

**Output:** x²

---

## 🧪 More examples

```html
<p>
  CO<sub>2</sub> <br>
  10<sup>th</sup> Class <br>
  a<sup>2</sup> + b<sup>2</sup>
</p>
```

---

## ⚖️ Comparison table

| Feature    | `<sub>`           | `<sup>`           |
| ---------- | ----------------- | ----------------- |
| Position   | Below text        | Above text        |
| Type       | Inline            | Inline            |
| Common use | Chemical formulas | Powers, footnotes |

---

## 🔹 Important notes

* Both are **inline elements**
* Should be used **only when meaning requires it**
* Do not use CSS positioning instead of these tags for semantics

---

### 📌 Exam-ready definitions

* **`<sub>`**: Displays subscript text below the baseline.
* **`<sup>`**: Displays superscript text above the baseline.

---


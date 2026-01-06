The **CSS Box Model** explains how every HTML element is structured and how space is calculated around it. Think of each element as a rectangular box made of **four layers**, from inside to outside:

---

## 1️⃣ Content

* The actual text, image, or content inside the element.
* Controlled by `width` and `height`.

```css
width: 200px;
height: 100px;
```

---

## 2️⃣ Padding

* Space **inside** the element, between content and border.
* Increases the visible size of the element.

```css
padding: 20px;
```

---

## 3️⃣ Border

* Surrounds padding and content.
* Has thickness, style, and color.

```css
border: 2px solid black;
```

---

## 4️⃣ Margin

* Space **outside** the element, separating it from other elements.
* Transparent and does not affect element size itself.

```css
margin: 15px;
```

---

## 📦 Visual Representation

```
+---------------------------+
|        Margin             |
|  +---------------------+ |
|  |      Border         | |
|  |  +---------------+ | |
|  |  |   Padding     | | |
|  |  | +-----------+ | | |
|  |  | | Content   | | | |
|  |  | +-----------+ | | |
|  |  +---------------+ | |
|  +---------------------+ |
+---------------------------+
```

---

## 🧠 box-sizing Property

### Default behavior

```css
box-sizing: content-box;
```

* `width` and `height` apply **only to content**
* Padding and border add extra size

### Recommended

```css
box-sizing: border-box;
```

* `width` includes **content + padding + border**
* Easier for layouts

```css
* {
  box-sizing: border-box;
}
```

---

## 🧪 Example

```css
div {
  width: 200px;
  padding: 20px;
  border: 5px solid blue;
  margin: 10px;
}
```

### Actual width:

* Content: 200px
* Padding: 40px (20 × 2)
* Border: 10px (5 × 2)
  👉 **Total width = 250px**

---

## ✅ Summary

* **Content** → actual data
* **Padding** → space inside
* **Border** → outline
* **Margin** → space outside
* `box-sizing: border-box` makes layouts easier


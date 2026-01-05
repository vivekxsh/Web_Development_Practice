## **Color Property in CSS** 🎨

The **`color` property** in CSS is used to set the **text color** of an HTML element.

---

## **Basic Syntax**

```css
selector {
  color: value;
}
```

### **Example**

```css
p {
  color: red;
}
```

This makes all paragraph text red.

---

## **Ways to Define Colors in CSS**

### **1. Color Names**

CSS supports predefined color names.

```css
h1 {
  color: blue;
}
```

✔ Easy to use
✘ Limited choices

---

### **2. HEX Colors**

Hexadecimal values represent colors using **#RRGGBB** format.

```css
p {
  color: #ff0000; /* red */
}
```

✔ Most commonly used
✔ Wide color range

---

### **3. RGB Colors**

RGB stands for **Red, Green, Blue**.

```css
p {
  color: rgb(255, 0, 0);
}
```

✔ More control over color
✔ Good for dynamic styling

---

### **4. RGBA Colors**

RGBA adds **alpha (opacity)** to RGB.

```css
p {
  color: rgba(255, 0, 0, 0.5);
}
```

✔ Supports transparency

---

### **5. HSL Colors**

HSL stands for **Hue, Saturation, Lightness**.

```css
p {
  color: hsl(0, 100%, 50%);
}
```

✔ Easier to adjust brightness and saturation

---

### **6. HSLA Colors**

HSL with alpha (transparency).

```css
p {
  color: hsla(240, 100%, 50%, 0.7);
}
```

---

## **Common Elements Using `color`**

```css
p, h1, h2, span, a {
  color: green;
}
```

✔ Applies only to **text**, not backgrounds

---

## **Color vs Background Color**

| Property           | Purpose          |
| ------------------ | ---------------- |
| `color`            | Text color       |
| `background-color` | Background color |

```css
div {
  color: white;
  background-color: black;
}
```

---

## **Inheritance**

The `color` property is **inherited** by child elements.

```css
div {
  color: blue;
}
```

All text inside `<div>` becomes blue unless overridden.

---

## **Best Practices**

✅ Use readable color contrast
✅ Prefer HEX, RGB, or HSL for precision
❌ Avoid low contrast colors

---

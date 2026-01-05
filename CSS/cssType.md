### **Types of CSS in Web Development** 🎨

CSS can be applied to a webpage in **three main ways**. Each type has its own use case, advantages, and disadvantages.

---

## **1. Inline CSS**

Inline CSS is written **directly inside an HTML element** using the `style` attribute.

### **Example**

```html
<p style="color: blue; font-size: 18px;">Hello World</p>
```

### **Advantages**

✔ Quick for small changes
✔ Useful for testing styles

### **Disadvantages**

✘ Hard to maintain
✘ Mixes content with design
✘ Cannot reuse styles

### **When to Use**

* Very small changes
* Debugging or testing only

---

## **2. Internal CSS (Embedded CSS)**

Internal CSS is written inside a `<style>` tag in the `<head>` section of the HTML file.

### **Example**

```html
<head>
  <style>
    p {
      color: green;
      font-size: 16px;
    }
  </style>
</head>
```

### **Advantages**

✔ Styles apply to a single page
✔ Better than inline CSS

### **Disadvantages**

✘ Not reusable across multiple pages
✘ Increases page size

### **When to Use**

* Single-page websites
* Small projects

---

## **3. External CSS**

External CSS is written in a **separate `.css` file** and linked to HTML.

### **Example**

```html
<link rel="stylesheet" href="styles.css">
```

**styles.css**

```css
p {
  color: red;
  font-size: 14px;
}
```

### **Advantages**

✔ Best practice
✔ Reusable across multiple pages
✔ Easier maintenance
✔ Faster loading (browser caching)

### **Disadvantages**

✘ Requires an extra file

### **When to Use**

* Large websites
* Professional projects

---

## **Priority Order (CSS Specificity)**

When multiple CSS types affect the same element:

1. **Inline CSS** (highest priority)
2. **Internal CSS**
3. **External CSS** (lowest priority)

> Note: `!important` overrides all (but should be avoided).

---

## **Comparison Table**

| Type     | Location              | Reusable | Best Use       |
| -------- | --------------------- | -------- | -------------- |
| Inline   | Inside HTML tag       | ❌ No     | Small changes  |
| Internal | `<style>` in `<head>` | ❌ No     | Single page    |
| External | `.css` file           | ✅ Yes    | Large projects |

---

## **Best Practice**

✅ Use **External CSS** for clean, scalable, and maintainable websites
❌ Avoid excessive Inline CSS

---

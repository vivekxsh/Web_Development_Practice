

---

## **1. `line-height`** 📝

The **`line-height`** property controls the **vertical space between lines of text**. Think of it as the “line spacing” in Word or Google Docs.

### **Syntax**

```css
selector {
  line-height: value;
}
```

### **Values**

| Value          | Description                                               |
| -------------- | --------------------------------------------------------- |
| `normal`       | Default spacing, depends on font                          |
| `<number>`     | Multiplier of font size (e.g., 1.5 means 1.5 × font size) |
| `<length>`     | Fixed height in px, em, etc. (e.g., 24px)                 |
| `<percentage>` | Percentage of font size (e.g., 150%)                      |

### **Example**

```css
p {
  font-size: 16px;
  line-height: 1.5; /* 24px spacing */
}
```

💡 **Tip:** Using a multiplier (like 1.5) is preferred because it scales automatically if you change the font size.

---

## **2. `letter-spacing`** ✨

The **`letter-spacing`** property controls **the horizontal space between letters**. It’s also called **tracking** in typography.

### **Syntax**

```css
selector {
  letter-spacing: value;
}
```

### **Values**

| Value      | Description                                                             |
| ---------- | ----------------------------------------------------------------------- |
| `normal`   | Default spacing                                                         |
| `<length>` | Adds extra space (positive) or reduces space (negative) between letters |

### **Example**

```css
h1 {
  letter-spacing: 2px; /* more space between letters */
}

p.tight {
  letter-spacing: -1px; /* letters closer together */
}
```

💡 **Tip:** Don’t overdo it—too much spacing can make text hard to read. Small adjustments (1–3px) usually look best.

---

## **Example Combining Both**

```css
p {
  font-size: 16px;
  line-height: 1.6;       /* more readable spacing */
  letter-spacing: 1px;    /* slight gap between letters */
}
```

✅ **Effect:** Text becomes **easier to read** and looks more professional.

---

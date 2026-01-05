
---

## **1. `font-weight`** 🖋️

The **`font-weight`** property controls **how thick or thin the text appears**.

### **Syntax**

```css
selector {
  font-weight: value;
}
```

### **Common Values**

| Value     | Description                                    |
| --------- | ---------------------------------------------- |
| `normal`  | Default weight (usually 400)                   |
| `bold`    | Bold text (usually 700)                        |
| `lighter` | Lighter than parent text                       |
| `bolder`  | Bolder than parent text                        |
| 100–900   | Numeric weight (100 is thin, 900 is very bold) |

### **Example**

```css
p.normal {
  font-weight: normal;
}

p.bold {
  font-weight: bold;
}

h1 {
  font-weight: 900; /* Extra bold */
}
```

💡 **Tip:** Not all fonts support all numeric weights. Usually, only `400` (normal) and `700` (bold) are reliable.

---

## **2. `text-decoration`** ✨

The **`text-decoration`** property adds **decorative lines to text**. It’s often used for links or emphasis.

### **Syntax**

```css
selector {
  text-decoration: value;
}
```

### **Common Values**

| Value                | Effect                           |
| -------------------- | -------------------------------- |
| `none`               | Removes decoration               |
| `underline`          | Adds underline                   |
| `overline`           | Adds line above text             |
| `line-through`       | Adds a strike-through line       |
| `underline overline` | Adds both underline and overline |

### **Example**

```css
a {
  text-decoration: none; /* Removes default underline */
}

h2 {
  text-decoration: underline;
}

p {
  text-decoration: line-through;
}
```

### **Modern Note**

CSS3 allows more control with **`text-decoration-color`**, **`text-decoration-style`**, and **`text-decoration-thickness`**:

```css
h1 {
  text-decoration: underline;
  text-decoration-color: red;
  text-decoration-style: wavy;
  text-decoration-thickness: 2px;
}
```

---

## **Example Combining Both**

```css
p {
  font-weight: bold;
  text-decoration: underline;
}
```

This will make the paragraph **bold and underlined**.

---

✅ **Key Takeaways**

* `font-weight` → thickness of text
* `text-decoration` → decorative lines on text
* Both are often combined for styling headings, links, or emphasis

---


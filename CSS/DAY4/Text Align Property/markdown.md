## **Text Properties in CSS** ✍️

**Text properties in CSS** are used to control the **appearance, alignment, spacing, and decoration of text** on a web page.

---

## **1. `color`**

Sets the text color.

```css
p {
  color: blue;
}
```

---

## **2. `text-align`**

Controls horizontal alignment of text.

```css
h1 {
  text-align: center;
}
```

**Values:** `left`, `right`, `center`, `justify`

---

## **3. `text-decoration`**

Adds or removes decorative lines.

```css
a {
  text-decoration: none;
}
```

**Values:** `underline`, `overline`, `line-through`, `none`

---

## **4. `text-transform`**

Changes the case of text.

```css
p {
  text-transform: uppercase;
}
```

**Values:** `uppercase`, `lowercase`, `capitalize`

---

## **5. `text-indent`**

Indents the first line of text.

```css
p {
  text-indent: 40px;
}
```

---

## **6. `letter-spacing`**

Controls space between letters.

```css
h2 {
  letter-spacing: 2px;
}
```

---

## **7. `word-spacing`**

Controls space between words.

```css
p {
  word-spacing: 5px;
}
```

---

## **8. `line-height`**

Sets the height between lines of text.

```css
p {
  line-height: 1.6;
}
```

✔ Improves readability

---

## **9. `white-space`**

Controls how whitespace is handled.

```css
p {
  white-space: nowrap;
}
```

**Values:** `normal`, `nowrap`, `pre`, `pre-wrap`

---

## **10. `text-shadow`**

Adds shadow effect to text.

```css
h1 {
  text-shadow: 2px 2px 5px gray;
}
```

---

## **11. `direction`**

Sets text direction.

```css
p {
  direction: rtl;
}
```

---

## **12. `unicode-bidi`**

Used with `direction` for bidirectional text.

```css
p {
  unicode-bidi: bidi-override;
}
```

---

## **Common Text Property Example**

```css
p {
  color: #333;
  text-align: justify;
  line-height: 1.5;
  letter-spacing: 1px;
}
```

---

## **Best Practices**

✅ Use proper line height for readability
✅ Avoid excessive letter spacing
✅ Maintain good color contrast
❌ Overusing text shadows

---


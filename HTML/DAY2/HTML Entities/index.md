## 🔣 HTML Entities

**HTML entities** are **special codes used to display characters that have a reserved meaning in HTML** or characters that are not easily typed from a keyboard.

For example, characters like `<`, `>`, `&` are **reserved in HTML** and cannot be used directly in text without being escaped.

---

## 🔹 Why we need HTML entities

1. **Reserved characters:** `<`, `>`, `&` are part of HTML syntax.

   * `<` → cannot just type `<` in text because browser reads it as a tag.
2. **Special symbols:** Like ©, ®, ±, ❤
3. **Invisible or non-typing characters:** like non-breaking space

---

## 🔹 Syntax of HTML entities

1. **Named entities**

```html
&amp;  → &
&lt;   → <
&gt;   → >
&copy; → ©
&reg;  → ®
&trade; → ™
```

2. **Numeric entities**

* Decimal: `&#number;`
* Hexadecimal: `&#xHEX;`

Examples:

```html
&#169;  → ©
&#174;  → ®
&#x2764; → ❤
```

---

## 🔹 Common HTML entities

| Character          | Named Entity | Decimal   | Hexadecimal |
| ------------------ | ------------ | --------- | ----------- |
| &                  | `&amp;`      | `&#38;`   | `&#x26;`    |
| <                  | `&lt;`       | `&#60;`   | `&#x3C;`    |
| >                  | `&gt;`       | `&#62;`   | `&#x3E;`    |
| "                  | `&quot;`     | `&#34;`   | `&#x22;`    |
| '                  | `&apos;`     | `&#39;`   | `&#x27;`    |
| ©                  | `&copy;`     | `&#169;`  | `&#xA9;`    |
| ®                  | `&reg;`      | `&#174;`  | `&#xAE;`    |
| ™                  | `&trade;`    | `&#8482;` | `&#x2122;`  |
| non-breaking space | `&nbsp;`     | `&#160;`  | `&#xA0;`    |

---

## 🔹 Example usage

```html
<p>5 &lt; 10 and 10 &gt; 5</p>
<p>Copyright &copy; 2026</p>
<p>Non-breaking space&nbsp;&nbsp;between words</p>
```

**Output:**

* `5 < 10 and 10 > 5`
* `Copyright © 2026`
* Extra space between words

---

## 🔹 Important notes

* Always use **entities for reserved characters** in HTML.
* Modern browsers handle UTF-8, so **many symbols like ❤ or © can also be typed directly**, but using entities is safer for **cross-browser compatibility**.
* Entities are **inline elements**, used within text.

---

### 📌 Exam-ready definition

> **HTML entities are special codes that represent reserved or special characters in HTML so that they can be displayed correctly in the browser.**

---

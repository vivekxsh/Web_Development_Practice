
---

````md
## 🔗 Anchor Tag (`<a>`) in HTML

The anchor tag is used to **create hyperlinks** that connect web pages, files, email addresses, or locations within the same page.

---

## 🧱 Basic Syntax
```html
<a href="URL">Link Text</a>
````

* `href` → Specifies the destination of the link
* `Link Text` → Clickable text shown to users

---

## 🌐 Linking to Another Website

```html
<a href="https://www.google.com">Visit Google</a>
```

---

## 📄 Linking to a Page in the Same Project

```html
<a href="about.html">About Us</a>
```

---

## 📍 Linking to a Section on the Same Page

```html
<a href="#contact">Go to Contact Section</a>

<section id="contact">
  Contact details here
</section>
```

---

## 🖼️ Image as a Link

```html
<a href="https://example.com">
  <img src="logo.png" alt="Website Logo">
</a>
```

---

## 📨 Email Link

```html
<a href="mailto:example@email.com">Send Email</a>
```

---

## 📞 Phone Call Link

```html
<a href="tel:+1234567890">Call Now</a>
```

---

## 🧭 Target Attribute

Controls how the link opens.

| Value     | Description                     |
| --------- | ------------------------------- |
| `_self`   | Opens in the same tab (default) |
| `_blank`  | Opens in a new tab              |
| `_parent` | Opens in parent frame           |
| `_top`    | Opens in full window            |

```html
<a href="https://example.com" target="_blank">Open in New Tab</a>
```

---

## ⬇️ Download Attribute

```html
<a href="file.pdf" download>Download PDF</a>
```

---

## 🎨 Styling Anchor Tags

```css
a {
  text-decoration: none;
  color: blue;
}
```

---

## 🧠 Best Practices

* Always use meaningful link text
* Use `target="_blank"` carefully
* Add `rel="noopener noreferrer"` with `_blank`
* Use `alt` text for linked images

```html
<a href="https://example.com" target="_blank" rel="noopener noreferrer">
  Secure Link
</a>
```

---

✨ **The anchor tag connects the web together.**



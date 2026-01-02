## 🧠 Semantic Markup in HTML

**Semantic markup** means using HTML tags that **clearly describe the meaning and purpose of the content**, not just how it looks.

👉 In simple words:
**Semantic tags tell both the browser and humans what the content is.**

---

## 🔹 Why semantic markup is important

* ✅ Improves **readability of code**
* ♿ Better **accessibility** (screen readers)
* 🔍 Better **SEO** (search engines understand content)
* 🛠️ Easier **maintenance**

---

## 🔹 Semantic vs Non-semantic tags

| Semantic             | Non-semantic         |
| -------------------- | -------------------- |
| Have meaning         | No meaning           |
| Describe content     | Used only for layout |
| Example: `<article>` | Example: `<div>`     |

---

## 🔹 Common semantic HTML5 tags

| Tag            | Meaning                   |
| -------------- | ------------------------- |
| `<header>`     | Header of page or section |
| `<nav>`        | Navigation links          |
| `<main>`       | Main content              |
| `<section>`    | Thematic section          |
| `<article>`    | Independent content       |
| `<aside>`      | Side content              |
| `<footer>`     | Footer                    |
| `<figure>`     | Media content             |
| `<figcaption>` | Caption                   |
| `<strong>`     | Important text            |
| `<em>`         | Emphasized text           |
| `<mark>`       | Highlighted text          |
| `<time>`       | Date or time              |

---

## 🔹 Example: Non-semantic vs Semantic

### ❌ Non-semantic

```html
<div class="header">
  <div class="menu">Home | About</div>
</div>
```

### ✅ Semantic

```html
<header>
  <nav>
    Home | About
  </nav>
</header>
```

---

## 🔹 Semantic page structure example

```html
<header>
  <h1>My Website</h1>
</header>

<nav>
  Menu
</nav>

<main>
  <article>
    <h2>Blog Post</h2>
    <p>Content here...</p>
  </article>

  <aside>
    Related links
  </aside>
</main>

<footer>
  © 2026
</footer>
```

---

## 🔹 Important notes

* Semantic tags **do not add style by default**
* Styling is done with **CSS**
* Use `<div>` only when **no semantic tag fits**

---

### 📌 Exam-ready definition

> **Semantic markup is the use of HTML tags that convey the meaning and structure of content clearly.**

---




---

## 1️⃣ The basic way (most common)

### Step 1: Pick a font

Go to **fonts.google.com**, choose a font (say, *Roboto*), and select the styles you want.

### Step 2: Add the `<link>` in your HTML

Put this inside your `<head>`:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap" rel="stylesheet">
```

### Step 3: Use it in your CSS

```css
body {
  font-family: 'Roboto', sans-serif;
}
```

That’s it. Your site now speaks Roboto.

---

## 2️⃣ Importing Google Fonts directly in CSS

You *can* do this, but it’s slightly less performant:

```css
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@400;700&display=swap');

body {
  font-family: 'Roboto', sans-serif;
}
```

⚠️ Use this only if you can’t edit the HTML.

---

## 3️⃣ Font weights & styles

If you load multiple weights, you can switch them like this:

```css
h1 {
  font-weight: 700;
}

p {
  font-weight: 400;
}
```

If you didn’t load a weight, the browser can’t magically invent it—so only request what you need.

---

## 4️⃣ Best practices (worth knowing)

* **Limit font families** (1–2 max)
* **Limit weights** (e.g. 400, 600, 700)
* Always add a **fallback**:

  ```css
  font-family: 'Roboto', Arial, sans-serif;
  ```
* `display=swap` avoids invisible text while loading (good UX)

---

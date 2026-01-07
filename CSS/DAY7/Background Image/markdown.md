In CSS, **`background-image`** is used to set an image as the background of an element.

---

## 1. Basic syntax

```css
.element {
  background-image: url("image.jpg");
}
```

---

## 2. Common background properties (very important)

### a) `background-repeat`

```css
background-repeat: no-repeat;
```

Values:

* `repeat` (default)
* `no-repeat`
* `repeat-x`
* `repeat-y`

---

### b) `background-size`

```css
background-size: cover;
```

Values:

* `cover` → fills the element, may crop image
* `contain` → fits entire image inside
* Custom:

```css
background-size: 100% 100%;
```

---

### c) `background-position`

```css
background-position: center;
```

Examples:

```css
background-position: top right;
background-position: 50% 50%;
```

---

### d) `background-attachment`

```css
background-attachment: fixed;
```

* `scroll` (default)
* `fixed` → parallax-like effect

---

## 3. Shorthand property

```css
.element {
  background: url("image.jpg") no-repeat center / cover;
}
```

Order:

```
background: image repeat position / size attachment color;
```

---

## 4. Full background image (hero section)

```css
body {
  background: url("bg.jpg") no-repeat center center / cover;
  height: 100vh;
}
```

---

## 5. Background image with overlay (very common)

```css
.hero {
  background:
    linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)),
    url("hero.jpg");
  background-size: cover;
  background-position: center;
}
```

Overlay makes text readable.

---

## 6. Multiple background images

```css
.box {
  background-image: 
    url("pattern.png"),
    url("main.jpg");
}
```

First image is on top.

---

## 7. Responsive background image

```css
.section {
  min-height: 100vh;
  background: url("img.jpg") center / cover no-repeat;
}
```

---

## 8. Common mistakes

❌ Forgetting `background-size: cover`
❌ Using large images (performance issue)
❌ Not setting height → image won’t show

---

## 9. Background image vs `<img>`

| Background Image | `<img>`        |
| ---------------- | -------------- |
| Decorative       | Content        |
| No alt text      | Supports alt   |
| Easy overlays    | Better for SEO |

---

### Quick example

```css
.card {
  width: 300px;
  height: 200px;
  background: url("photo.jpg") center / cover no-repeat;
  border-radius: 10px;
}
```

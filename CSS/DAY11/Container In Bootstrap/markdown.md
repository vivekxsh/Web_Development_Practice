In **Bootstrap**, a **container** is the basic layout element used to **wrap, center, and pad** your website’s content. It is usually the **first Bootstrap class** you use inside the `<body>`.

---

## What Is a Container in Bootstrap?

A container:

* Centers content horizontally
* Adds left and right padding
* Controls the maximum width of the page
* Holds the **grid system** (`row` and `col`)

---

## Types of Containers in Bootstrap

### 1. `.container` (Fixed-width, responsive)

* Has a **different max-width at each screen size**
* Most commonly used

```html
<div class="container">
  Content here
</div>
```

**Max-widths (Bootstrap 5):**

| Screen Size           | Max Width |
| --------------------- | --------- |
| Extra small           | 100%      |
| Small (≥576px)        | 540px     |
| Medium (≥768px)       | 720px     |
| Large (≥992px)        | 960px     |
| Extra large (≥1200px) | 1140px    |
| XXL (≥1400px)         | 1320px    |

---

### 2. `.container-fluid` (Full-width)

* Always **100% width**
* Stretches across the entire screen

```html
<div class="container-fluid">
  Full width content
</div>
```

**Used for:**

* Full-width banners
* Background sections
* Dashboards

---

### 3. Responsive Containers

You can choose **when** the container becomes fixed-width.

```html
<div class="container-md">
  Fixed width from medium screens and up
</div>
```

| Class           | Behavior           |
| --------------- | ------------------ |
| `container-sm`  | 100% until ≥576px  |
| `container-md`  | 100% until ≥768px  |
| `container-lg`  | 100% until ≥992px  |
| `container-xl`  | 100% until ≥1200px |
| `container-xxl` | 100% until ≥1400px |

---

## Container Structure (Very Important)

Containers should contain **rows**, and rows should contain **columns**.

✅ Correct structure:

```html
<div class="container">
  <div class="row">
    <div class="col">Column</div>
  </div>
</div>
```

❌ Incorrect:

```html
<div class="container">
  <div class="col">Wrong usage</div>
</div>
```

---

## Padding in Containers

Bootstrap containers have **built-in horizontal padding** (called *gutters*).

* Default padding: `1rem` (16px)
* You can control it using utilities:

```html
<div class="container px-0">No horizontal padding</div>
```

---

## When to Use Which Container?

| Situation             | Container Type       |
| --------------------- | -------------------- |
| Normal website layout | `.container`         |
| Full-width layout     | `.container-fluid`   |
| Responsive control    | `.container-md` etc. |

---

## Example Layout

```html
<body>
  <div class="container">
    <h1 class="text-center">Welcome</h1>
    <div class="row">
      <div class="col-md-8">Main Content</div>
      <div class="col-md-4">Sidebar</div>
    </div>
  </div>
</body>
```

---

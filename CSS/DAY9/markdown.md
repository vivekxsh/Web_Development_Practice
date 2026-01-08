
---

## 1. The Big Idea

Flexbox is **one-dimensional** layout:

* It works **in a row OR a column** (not both at once — that’s Grid’s job).

You have:

* a **flex container** (the parent)
* **flex items** (the children)

```css
.container {
  display: flex;
}
```

Once you do this, the children become flex items and obey flex rules.

---

## 2. Axes: The Key Mental Model

Everything in Flexbox revolves around **two axes**:

### Main Axis

* Defined by `flex-direction`
* Default: **horizontal (row)**

### Cross Axis

* Perpendicular to the main axis

| flex-direction | Main axis    | Cross axis   |
| -------------- | ------------ | ------------ |
| row (default)  | left → right | top → bottom |
| column         | top → bottom | left → right |

This matters because:

* `justify-content` → **main axis**
* `align-items` → **cross axis**

---

## 3. Container Properties (Most Important)

### 1. `flex-direction`

Sets the direction of items.

```css
flex-direction: row;        /* default */
flex-direction: row-reverse;
flex-direction: column;
flex-direction: column-reverse;
```

---

### 2. `justify-content` (main axis alignment)

Controls **how items are spaced along the main axis**.

```css
justify-content: flex-start; /* default */
justify-content: center;
justify-content: flex-end;
justify-content: space-between;
justify-content: space-around;
justify-content: space-evenly;
```

Think:

> “How do items line up **in the direction they flow**?”

---

### 3. `align-items` (cross axis alignment)

Controls **alignment perpendicular to the main axis**.

```css
align-items: stretch; /* default */
align-items: center;
align-items: flex-start;
align-items: flex-end;
align-items: baseline;
```

---

### 4. `flex-wrap`

By default, flex items try to fit on **one line**.

```css
flex-wrap: nowrap; /* default */
flex-wrap: wrap;
flex-wrap: wrap-reverse;
```

Often used with:

```css
flex-flow: row wrap; /* shorthand */
```

---

### 5. `align-content` (multi-line only)

Used **only when items wrap onto multiple lines**.

```css
align-content: flex-start;
align-content: center;
align-content: space-between;
align-content: stretch;
```

🚨 Common mistake:

> `align-content` does **nothing** unless `flex-wrap: wrap` is on.

---

## 4. Item Properties (Children)

### 1. `flex-grow`

How much an item can grow relative to others.

```css
.item {
  flex-grow: 1;
}
```

If all items have `flex-grow: 1`, they share space equally.

---

### 2. `flex-shrink`

How much an item shrinks when space is tight.

```css
flex-shrink: 1; /* default */
```

Set to `0` to prevent shrinking.

---

### 3. `flex-basis`

The item’s **starting size** before grow/shrink.

```css
flex-basis: 200px;
```

---

### 4. `flex` (shorthand — very common)

```css
flex: grow shrink basis;
```

Examples:

```css
flex: 1;          /* = 1 1 0 */
flex: 0 0 auto;   /* no grow, no shrink */
flex: 1 0 200px;
```

📌 **Most common pattern**:

```css
flex: 1;
```

---

### 5. `align-self`

Overrides `align-items` for one item.

```css
align-self: center;
```

---

### 6. `order`

Changes visual order without changing HTML.

```css
order: 1;
```

Default is `0`.

---

## 5. Common Flexbox Patterns

### Center Anything (Classic Use Case)

```css
.container {
  display: flex;
  justify-content: center;
  align-items: center;
}
```

---

### Navigation Bar

```css
nav {
  display: flex;
  justify-content: space-between;
  align-items: center;
}
```

---

### Equal-Width Columns

```css
.column {
  flex: 1;
}
```

---

### Sidebar + Content Layout

```css
.sidebar {
  flex: 0 0 250px;
}

.main {
  flex: 1;
}
```

---

### Responsive Wrapping Cards

```css
.cards {
  display: flex;
  flex-wrap: wrap;
  gap: 1rem;
}

.card {
  flex: 1 1 250px;
}
```

---

## 6. Flexbox vs Grid (Quick Rule)

Use **Flexbox** when:

* You’re laying out items in **one direction**
* You care about **alignment & spacing**
* Navigation bars, toolbars, lists, components

Use **Grid** when:

* You need **rows AND columns**
* Page-level layouts
* Complex placement

They’re not competitors — they’re teammates.

---

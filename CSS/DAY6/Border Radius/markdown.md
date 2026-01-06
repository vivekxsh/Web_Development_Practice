In CSS, **border radius** controls how rounded the corners of an element are. It’s done with the `border-radius` property.

---

## Basic usage

```css
.box {
  border-radius: 10px;
}
```

🔹 This rounds **all four corners** by 10 pixels.

---

## Different values for each corner

You can control each corner individually, in this order:

**top-left → top-right → bottom-right → bottom-left**

```css
.box {
  border-radius: 10px 20px 30px 40px;
}
```

---

## Two or three values

```css
border-radius: 10px 20px;
```

* Top-left & bottom-right: `10px`
* Top-right & bottom-left: `20px`

```css
border-radius: 10px 20px 30px;
```

* Top-left: `10px`
* Top-right & bottom-left: `20px`
* Bottom-right: `30px`

---

## Individual corner properties

```css
.box {
  border-top-left-radius: 15px;
  border-top-right-radius: 5px;
  border-bottom-right-radius: 25px;
  border-bottom-left-radius: 10px;
}
```

---

## Making a circle or pill shape

### Circle (perfect)

```css
.circle {
  width: 100px;
  height: 100px;
  border-radius: 50%;
}
```

### Pill / rounded button

```css
.button {
  border-radius: 999px;
}
```

---

## Elliptical corners

You can create **oval corners** using `/`:

```css
.box {
  border-radius: 20px / 40px;
}
```

Or per corner:

```css
border-radius: 10px 20px / 30px 40px;
```

---

## Works with more than just borders

Even if there’s **no border**, `border-radius` still affects:

* backgrounds
* images
* shadows (`box-shadow`)
* overflow content (with `overflow: hidden`)

---

## Common beginner mistakes

* ❌ Forgetting units (`border-radius: 10;`) → needs `px`, `%`, etc.
* ❌ Expecting rounding when element has `width` but no `height`
* ❌ Not using `overflow: hidden` when rounding images inside divs

---

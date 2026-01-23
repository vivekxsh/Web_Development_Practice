Bootstrap **badges** are small count/label components—perfect for things like *notifications, status, or “new” tags*.

---

## 1. Basic Badge

```html
<span class="badge bg-primary">New</span>
```

In **Bootstrap 5**, badges use `bg-*` (not `badge-*`).

---

## 2. Badge Colors

```html
<span class="badge bg-secondary">Secondary</span>
<span class="badge bg-success">Success</span>
<span class="badge bg-danger">Danger</span>
<span class="badge bg-warning text-dark">Warning</span>
<span class="badge bg-info text-dark">Info</span>
<span class="badge bg-light text-dark">Light</span>
<span class="badge bg-dark">Dark</span>
```

---

## 3. Badges with Headings

Great for counts next to titles:

```html
<h3>
  Notifications <span class="badge bg-danger">5</span>
</h3>
```

---

## 4. Pill Badges

Rounded, modern look:

```html
<span class="badge rounded-pill bg-primary">New</span>
```

---

## 5. Badges Inside Buttons

Common for message counts 🔔

```html
<button class="btn btn-primary">
  Inbox <span class="badge bg-light text-dark">4</span>
</button>
```

---

## 6. Positioned Badges (Notification Dot)

For floating count indicators:

```html
<button class="btn btn-primary position-relative">
  Messages
  <span class="position-absolute top-0 start-100 translate-middle badge rounded-pill bg-danger">
    9+
  </span>
</button>
```

---

## 7. Accessibility Tip (Important!)

For screen readers:

```html
<span class="visually-hidden">unread messages</span>
```

Example:

```html
<span class="badge bg-danger">
  5
  <span class="visually-hidden">unread notifications</span>
</span>
```

---


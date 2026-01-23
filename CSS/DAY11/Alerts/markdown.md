Bootstrap **alerts** are used to show **important messages** like success, errors, warnings, or info to users.
---

## 1. Basic Alert

```html
<div class="alert alert-primary" role="alert">
  This is a primary alert!
</div>
```

---

## 2. Alert Colors (Contextual Classes)

```html
<div class="alert alert-success">Success! Action completed.</div>
<div class="alert alert-danger">Error! Something went wrong.</div>
<div class="alert alert-warning">Warning! Check your input.</div>
<div class="alert alert-info">Info! Please read this.</div>
<div class="alert alert-secondary">Secondary alert.</div>
<div class="alert alert-light">Light alert.</div>
<div class="alert alert-dark">Dark alert.</div>
```

---

## 3. Dismissible Alerts (Close Button)

Very common UX pattern 👌

```html
<div class="alert alert-warning alert-dismissible fade show" role="alert">
  <strong>Warning!</strong> You should check this.
  <button type="button" class="btn-close" data-bs-dismiss="alert"></button>
</div>
```

👉 Requires **Bootstrap JS**

---

## 4. Alerts with Links

```html
<div class="alert alert-info">
  Learn more <a href="#" class="alert-link">here</a>.
</div>
```

---

## 5. Alerts with Extra Content

You can put headings, text, lists, etc.

```html
<div class="alert alert-success" role="alert">
  <h4 class="alert-heading">Well done!</h4>
  <p>You successfully read this important message.</p>
  <hr>
  <p class="mb-0">Keep it up 👍</p>
</div>
```

---

## 6. Icons in Alerts (Optional)

Using Bootstrap Icons:

```html
<div class="alert alert-danger d-flex align-items-center" role="alert">
  <i class="bi bi-exclamation-triangle-fill me-2"></i>
  <div>Error occurred while saving.</div>
</div>
```

---

## 7. Alerts via JavaScript

Manually close or trigger alerts:

```html
<script>
  const alert = document.querySelector('.alert');
  const bsAlert = new bootstrap.Alert(alert);
  bsAlert.close();
</script>
```

---


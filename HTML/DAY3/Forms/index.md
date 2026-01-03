
---

## 1. What is an HTML form?

A form is created using the `<form>` tag and contains **input elements** such as text boxes, buttons, checkboxes, etc.

```html
<form>
  <!-- form elements go here -->
</form>
```

---

## 2. Basic Form Structure

```html
<form action="submit.php" method="post">
  <label>Name:</label>
  <input type="text" name="username">

  <input type="submit" value="Submit">
</form>
```

### Important attributes:

* **action** → where the form data is sent
* **method**

  * `get` → data appears in URL
  * `post` → data sent securely (commonly used)

---

## 3. Common Form Elements

### Text Input

```html
<input type="text" name="name">
```

### Password

```html
<input type="password" name="password">
```

### Email

```html
<input type="email" name="email">
```

### Radio Buttons

```html
<input type="radio" name="gender" value="male"> Male
<input type="radio" name="gender" value="female"> Female
```

### Checkbox

```html
<input type="checkbox" name="hobby" value="sports"> Sports
```

### Textarea

```html
<textarea name="message"></textarea>
```

### Dropdown (Select)

```html
<select name="country">
  <option>India</option>
  <option>USA</option>
</select>
```

### Submit Button

```html
<input type="submit" value="Send">
```

---

## 4. Labels (Important for accessibility)

```html
<label for="email">Email:</label>
<input type="email" id="email">
```

---

## 5. Required & Validation

```html
<input type="text" required>
<input type="number" min="1" max="10">
```

---

## 6. Complete Example

```html
<form>
  <label>Name:</label>
  <input type="text" required><br><br>

  <label>Email:</label>
  <input type="email" required><br><br>

  <input type="submit">
</form>
```

---

## 7. What happens after submission?

* Sent to a **server** (PHP, Node.js, etc.)
* Or handled using **JavaScript**

---


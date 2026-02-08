In JavaScript, **variables** are how you store data so you can use it later. There are **three main ways** to declare them 👇

---

### `let`

* **Most commonly used**
* Block-scoped (only exists inside `{ }`)
* Can be reassigned

```js
let age = 25;
age = 26;
```

Use this for values that **will change**.

---

### `const`

* Block-scoped
* **Cannot be reassigned**
* Must be initialized when declared

```js
const name = "Alex";
// name = "Sam"; ❌ error
```

Use this by default, especially for values that **shouldn’t change**.

⚠️ Note: Objects and arrays declared with `const` can still be modified:

```js
const nums = [1, 2];
nums.push(3); // allowed
```

---

### `var`

* **Old-school** (avoid in modern JS)
* Function-scoped, not block-scoped
* Can cause bugs due to hoisting

```js
var x = 10;
```

You’ll still see it in older code, but `let` and `const` are preferred now.

---

### Quick comparison

| Keyword | Scope    | Reassign | Use it?     |
| ------- | -------- | -------- | ----------- |
| `let`   | Block    | ✅        | ✅           |
| `const` | Block    | ❌        | ✅ (default) |
| `var`   | Function | ✅        | ❌           |

---

### Example in action

```js
const pi = 3.14;
let radius = 5;

let area = pi * radius * radius;
console.log(area);
```

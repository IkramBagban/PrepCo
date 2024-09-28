# JavaScript Interview Questions

## Basic Questions

<details>
<summary>What is JavaScript?</summary>

JavaScript is a high-level, interpreted programming language that is widely used for web development. It enables dynamic and interactive behavior on websites, allowing developers to create features such as animations, form validations, and real-time content updates. JavaScript can be executed on both the client side (in web browsers) and the server side (using environments like Node.js).

</details>

<details>
<summary>What is syntax in JavaScript?</summary>

Syntax in JavaScript refers to the set of rules that define how JavaScript code should be written and structured. These rules dictate how statements, expressions, operators, keywords, and punctuation (like semicolons, curly braces, parentheses, etc.) are used to create valid code. For example:

```javascript
let message = "Hello, World!"; // Correct syntax
console.log(message); // Correct syntax
```

</details>

<details>
<summary>What are the data types supported by JavaScript?</summary>

JavaScript supports the following data types:

- **Primitive Data Types:**

  - **String**: Represents textual data (`"hello"`, `'world'`).
  - **Number**: Represents both integer and floating-point numbers (`42`, `3.14`).
  - **Boolean**: Represents logical values (`true` or `false`).
  - **Undefined**: A variable declared but not assigned a value.
  - **Null**: Represents the intentional absence of any object value.
  - **Symbol**: Represents a unique, immutable identifier (introduced in ES6).
  - **BigInt**: Represents integers beyond the safe integer limit (introduced in ES11).

- **Non-Primitive Data Types:**

  - **Object**: Used to store collections of data or more complex entities (e.g., arrays, functions, objects).

</details>

<details>
<summary>What is the difference between `null` and `undefined`?</summary>

- **`undefined`**: Indicates that a variable has been declared but has not been assigned a value. It is the default value of uninitialized variables.

  ```javascript
  let a;
  console.log(a); // Output: undefined
  ```

- **`null`**: Represents the intentional absence of any object value. It is often used to signify that a variable is empty or has no value.

  ```js
  let b = null;
  console.log(b); // Output: null
  ```

**Key Difference:** `undefined` is automatically assigned by JavaScript to uninitialized variables, while `null` is an assignment value indicating "no value."

</details>

<details>
<summary>Explain the difference between `==` and `===` in JavaScript.</summary>

- **`==` (Loose Equality)**: Compares two values for equality after performing type conversion (coercion) if necessary. It attempts to convert the values to a common type before comparison.

  ```js
  console.log(5 == "5");
  // Output: true (because '5' is converted to 5)
  ```

- **`===` (Strict Equality)**: Compares two values for equality without performing any type conversion. The values must be of the same type and value to be considered equal.

```
 console.log(5 === '5');
 // Output: false (different types: number vs. string)
```

**Recommendation:** Always use `===` for comparisons to avoid unexpected results caused by type coercion.

</details>

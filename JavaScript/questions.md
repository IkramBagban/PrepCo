<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JavaScript Interview Questions</title>
</head>
<body style="font-family: Arial, sans-serif; background-color: #f9f9f9; color: #333; padding: 20px; margin: 0;">
    <div style="max-width: 800px; margin: 0 auto; background-color: #fff; padding: 20px; box-shadow: 0 0 10px rgba(0, 0, 0, 0.1); border-radius: 8px;">
        <h1 style="text-align: center; color: red;">JavaScript Interview Questions</h1>
        <h2 style="border-bottom: 2px solid #007bff; padding-bottom: 5px; margin-bottom: 10px; color: #007bff;">Basic Questions</h2>
        
        <details style="margin: 10px 0; border: 1px solid #ddd; padding: 10px; border-radius: 5px; background-color: #f1f1f1; cursor: pointer; transition: background-color 0.3s;">
            <summary style="font-size: 1.1em; font-weight: bold; outline: none;">What is JavaScript?</summary>
            <p style="margin: 10px 0; line-height: 1.6;">JavaScript is a high-level, interpreted programming language that is widely used for web development. It enables dynamic and interactive behavior on websites, allowing developers to create features such as animations, form validations, and real-time content updates. JavaScript can be executed on both the client side (in web browsers) and the server side (using environments like Node.js).</p>
        </details>

        <details style="margin: 10px 0; border: 1px solid #ddd; padding: 10px; border-radius: 5px; background-color: #f1f1f1; cursor: pointer; transition: background-color 0.3s;">
            <summary style="font-size: 1.1em; font-weight: bold; outline: none;">What is syntax in JavaScript?</summary>
            <p style="margin: 10px 0; line-height: 1.6;">Syntax in JavaScript refers to the set of rules that define how JavaScript code should be written and structured. These rules dictate how statements, expressions, operators, keywords, and punctuation (like semicolons, curly braces, parentheses, etc.) are used to create valid code. For example:</p>
            <pre style="background-color: #f7f7f7; padding: 10px; border: 1px solid #ddd; border-radius: 5px; overflow-x: auto;">
<code>let message = "Hello, World!"; // Correct syntax
console.log(message); // Correct syntax</code></pre>
        </details>

        <details style="margin: 10px 0; border: 1px solid #ddd; padding: 10px; border-radius: 5px; background-color: #f1f1f1; cursor: pointer; transition: background-color 0.3s;">
            <summary style="font-size: 1.1em; font-weight: bold; outline: none;">What are the data types supported by JavaScript?</summary>
            <p style="margin: 10px 0; line-height: 1.6;">JavaScript supports the following data types:</p>
            <ul style="margin: 10px 0 10px 20px;">
                <li><strong>Primitive Data Types:</strong></li>
                <ul style="margin: 10px 0 10px 20px;">
                    <li><strong>String:</strong> Represents textual data (<code>"hello"</code>, <code>'world'</code>).</li>
                    <li><strong>Number:</strong> Represents both integer and floating-point numbers (<code>42</code>, <code>3.14</code>).</li>
                    <li><strong>Boolean:</strong> Represents logical values (<code>true</code> or <code>false</code>).</li>
                    <li><strong>Undefined:</strong> A variable declared but not assigned a value.</li>
                    <li><strong>Null:</strong> Represents the intentional absence of any object value.</li>
                    <li><strong>Symbol:</strong> Represents a unique, immutable identifier (introduced in ES6).</li>
                    <li><strong>BigInt:</strong> Represents integers beyond the safe integer limit (introduced in ES11).</li>
                </ul>
                <li><strong>Non-Primitive Data Types:</strong></li>
                <ul style="margin: 10px 0 10px 20px;">
                    <li><strong>Object:</strong> Used to store collections of data or more complex entities (e.g., arrays, functions, objects).</li>
                </ul>
            </ul>
        </details>

        <details style="margin: 10px 0; border: 1px solid #ddd; padding: 10px; border-radius: 5px; background-color: #f1f1f1; cursor: pointer; transition: background-color 0.3s;">
            <summary style="font-size: 1.1em; font-weight: bold; outline: none;">What is the difference between `null` and `undefined`?</summary>
            <p style="margin: 10px 0; line-height: 1.6;"><strong>`undefined`:</strong> Indicates that a variable has been declared but has not been assigned a value. It is the default value of uninitialized variables.</p>
            <pre style="background-color: #f7f7f7; padding: 10px; border: 1px solid #ddd; border-radius: 5px; overflow-x: auto;">
<code>let a;
console.log(a); // Output: undefined</code></pre>
            <p style="margin: 10px 0; line-height: 1.6;"><strong>`null`:</strong> Represents the intentional absence of any object value. It is often used to signify that a variable is empty or has no value.</p>
            <pre style="background-color: #f7f7f7; padding: 10px; border: 1px solid #ddd; border-radius: 5px; overflow-x: auto;">
<code>let b = null;
console.log(b); // Output: null</code></pre>
            <p style="margin: 10px 0; line-height: 1.6;"><strong>Key Difference:</strong> `undefined` is automatically assigned by JavaScript to uninitialized variables, while `null` is an assignment value indicating "no value."</p>
        </details>

        <details style="margin: 10px 0; border: 1px solid #ddd; padding: 10px; border-radius: 5px; background-color: #f1f1f1; cursor: pointer; transition: background-color 0.3s;">
            <summary style="font-size: 1.1em; font-weight: bold; outline: none;">Explain the difference between `==` and `===` in JavaScript.</summary>
            <p style="margin: 10px 0; line-height: 1.6;"><strong>`==` (Loose Equality):</strong> Compares two values for equality after performing type conversion (coercion) if necessary. It attempts to convert the values to a common type before comparison.</p>
            <pre style="background-color: #f7f7f7; padding: 10px; border: 1px solid #ddd; border-radius: 5px; overflow-x: auto;">
<code>console.log(5 == "5"); // Output: true (because '5' is converted to 5)</code></pre>
            <p style="margin: 10px 0; line-height: 1.6;"><strong>`===` (Strict Equality):</strong> Compares two values for equality without performing any type conversion. The values must be of the same type and value to be considered equal.</p>
            <pre style="background-color: #f7f7f7; padding: 10px; border: 1px solid #ddd; border-radius: 5px; overflow-x: auto;">
<code>console.log(5 === '5'); // Output: false (different types: number vs. string)</code></pre>
            <p style="margin: 10px 0; line-height: 1.6;"><strong>Recommendation:</strong> Always use `===` for comparisons to avoid unexpected results caused by type coercion.</p>
        </details>
    </div>
    
    <script>
        document.querySelectorAll('details').forEach(detail => {
            detail.addEventListener('toggle', function() {
                if (this.open) {
                    document.querySelectorAll('details').forEach(otherDetail => {
                        if (otherDetail !== this) otherDetail.removeAttribute('open');
                    });
                }
            });
        });
    </script>
</body>
</html>

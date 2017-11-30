## You Don't Know JS: Up & Going

by Kyle Simpson

Link to this amazing
[book](https://github.com/getify/You-Dont-Know-JS/tree/master/up%20%26%20going)

### Chapter 1: Into Programming

* Easy way to get input from the user:

```js
age = prompt('Please tell me your age:');

console.log(age);
```

* Equality operators: `==` (loose-equals), `===` (strict-equals), `!=` (loose not-equals) and `!==` (strict non-equals).
* Lexical scope rules say that code in one scope can access variables of either that scope or any scope outside of it.
* **Practice is the key to learning code**.

### Chapter 2: Into Javascript
* Javascript has **typed values, not typed variables**.
* The following built-in types are available: `string`, `number`, `boolean`, `null` and `undefined`, `object` and `symbol` (new to ES6).
* The `typeof` operator can examine a value and tell you what type it is.
* `typeof null` errantly returns `"object"` when you'd expet it to return `"null"`.
* **Coercion** is the conversion from one type of value into another.
* Javascript has *explicit* and *implicit* coercion.
* Explicit coercion:
```js
var a = "42";

var b = Number(a);

a;    // "42" -- string
b;    // 42 -- number
```
* Implicit coercion:
```js
var a = "42";

var b = a * 1; // implicitly coerced to number

a;    // "42" -- string
b;    // 42 -- number
```
* "truthy" and "falsy" nature of values: when a non-`boolean` value is coerced to a `boolean`.
* List of "falsy" values in Js: `""` (empty string), `0`, `-0`, `NaN` (invalid `number`), `null`, `undefined`, `false`.
* Any value that's not "falsy" is "truthy".
* The difference between `==` (loose-equals) and `===` (strict-equals) is that `==` checks for **value equality with coercion allowed**, and `===` checks for **value equality without allowing coercion**.
* An identifier must start with `a`-`z`, `A`-`Z`, `$`, or `_`. It can then contain any of those characters plus the numerals `0`-`9`.
* **Hoisting**: when a `var` declaration is conceptually "moved" to the top of its enclosing scope.
* **Note** only the declaration is hoisted, the asignment is not "moved" to the top.
```js
console.log(a); // undefined
var a = 2;
console.log(a); // 2
```
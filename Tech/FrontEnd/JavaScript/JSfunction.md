# JavaScript function
JavaScript functions are somewhat peculiar. They are used in different ways to achieve different architecture.
Here are some ways to use those function in different ways.

# Declarations
### Using Function Constructor
```js
    function square(n) {
    return n * n;
    }
```
### Using Expression
* declaring variables is an example of expression. Anything LHS assigned with RHS using operator `=` is an expression.
* or `var t = 4;` is an expression in easy way.
```js
    const square = function (n) {
    return n * n;
    };
```
# Difference
### Hoisting
*  In JavaScript like in Hosting the flag goes from bottom to top, the variables and function are moved to the top before execution.
* JavaScript is the only language that uses Hoisting. JS Transpiler (one high level language to another) languages like TS, CoffeeScript also use those.
* Declaring function using constructor and expression behaves differently on hoisting.

Case 1:
```js
    console.log(square(5));
    function square(n) {
    return n * n;
    }
    // >> 25
```
Case 2:
```js
    console.log(square(5)); 
    var square = function (n) {
    return n * n;
    };
    // TypeError: square is not a function
```
* In second case, you will get `// TypeError: square is not a function` error. If all variables and functions moves to the top why case 2 doesn't work while 1st one works correctly?  Because the hoisting is just an abstracted term. But in real time the function and variables doesn't move physically in the code; Instead first the memory of those variables are allocated with value as undefined, in case of function the function is copied and memory is allocated first.
* Since the `square` variable have undefined and the function is yet to be appended, `not a function` error is thrown.

### let / const vs var
* Here is the same hoisting with different declarations.
```js
console.log(n);
var n =6
// >> undefined
console.log(n);
let n =6
// or const>>Uncaught ReferenceError: n is not defined
```
* That's how JavaScript works. `let` and `const` are block-scoped local variables and `var` are function or global scoped. So `let` and `const` is non-hoisted.
* When `let` or `const` are used in Case 2, we get `ReferenceError: square is not defined` error.
* If you need more confusing stuff check [this medium post](https://medium.com/@oguzhancelikkaya/function-declarations-vs-function-expressions-hoisting-ace84399a172) JFF.

* In simple **Conclusion** the function declaration using expression doesn't follow hoisting and can be considered as same place as physical position in the code.

## Types
### IIFE


# Ref
* [Function MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Functions)
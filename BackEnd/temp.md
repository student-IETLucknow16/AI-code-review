Your current function has a small issue: **`a` and `b` are not defined as parameters.**

Unless `a` and `b` are already defined globally outside of the function, calling this function will throw a
`ReferenceError: a is not defined`.

Here is the correct and most common way to write this function by passing `a` and `b` as **parameters**:

### 1. Standard Way (Passed as arguments)
```javascript
function sum(a, b) {
return a + b;
}

// How to use it:
console.log(sum(5, 10)); // Output: 15
```

### 2. Modern ES6 Way (Arrow Function)
If you are using modern JavaScript, you can write this in a single, clean line:
```javascript
const sum = (a, b) => a + b;

// How to use it:
console.log(sum(5, 10)); // Output: 15
```

### Why is this better?
By passing `a` and `b` inside the parentheses `(a, b)`, the function becomes "pure" and reusable. You can pass any two
numbers into it, and it will return their sum.
---
title: 'Default parameters in Javascript functions'
description: 'Default parameters are a feature of JavaScript that allows you to define a default value for a parameter in a function. Usually used as a fallback if nothing is passed to the function'
---

# Default parameters in Javascript functions
Default parameters are a feature of JavaScript that allows you to define a default value for a parameter in a function. Usually used as a fallback if nothing is passed to the function.

```js
function greet(name = 'John') {
    console.log(`Hello ${name}!`);
}
```

If a the function greet is invoked/ called without passing a parameter, it will print out `Hello John` since the function has a default parameter of John. 

If the function is invoked with a parameter, the default parameter will be ignored and the passed parameter will be used instead.

```javascript
    greet('Jane'); // Hello Jane
```

In this case `Hello Jane` is printed out instead of `Hello John`.

### More examples

**Example 1**
   
```js
function printMyNames(firstName = 'John', lastName = 'Doe') {
    console.log(`${firstName} ${lastName}`);
}

printMyNames() // John Doe
```

**Example 2**
 
```js
const addNumbers = (num1 = 1, num2 = 2) => num1 + num2;

console.log(addNumbers(10, 20)) // 30
console.log(addNumbers()) // 3
console.log(addNumbers(10)) // 12
```

**Example 3**

```js
const multiplyNumbers = (num1 = 1, num2 = 2) => {
    const num3 = num1 * num2
    return num3
}

console.log(multiplyNumbers(10, 20)) // 200
console.log(multiplyNumbers(10)) // 20
console.log(multiplyNumbers()) // 2
```
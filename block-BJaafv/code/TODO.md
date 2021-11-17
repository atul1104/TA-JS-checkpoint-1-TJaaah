1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}
//Here in above the return keyword gives the value which can be stored in a variable. Here function always returns a value.
// second
function sum(a, b) {
  console.log(a + b);
}
// Here in above the console.log keyword logs the value in console. Here function does not contain return therefore the value of sum is undefined.
```

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.
   Ans. Value of 'first' will be the result of sum of two numbers But value of 'second' will be 'undefined' datatype.

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?
   Ans.Output will be 36. And third number that is 35 will not be summed in because there are only two parameters are used in function declaration.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?
   Ans. Yes we can store the first 'sum' function in variable named 'add' because we used 'return' in this function.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

```js
function sayHello(name) {
  return `Hello ${name}`;
}
sayHello("Arya");
```

6. What will be the output of the function below and why?

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

showMessage();
```

//Output is uncaught referrence error, because username is not defined inside the function. The username defined outside the function is not come into play when function is getting executed. 7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

alert(userName); // Undefined

showMessage(); // Uncaught referrence error, username is not defined at showMessage.

alert(userName); // Undefined
```

8. What is a Anonymous Function give example of three functions.
   Ans.Anonymous function is a function with no name but it's name is defined already as a variable

```js
let showMessage = function () {
  let message = "Hello, " + userName;
  return message;
};

const addNumbers = function (numA, numB) {
  return numA + numB;
};

let sayHello = function (name) {
  return `Hello ${name}`;
};
sayHello("Arya");
```

9. Can function declaration be a Anonymous Function? Explain
   Ans. Function declaration can be an anonymous function untill it is defined in a variable.

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.
```

```js
function getSquare() {}

function calcAge() {}
function createBox() {}
function checkValue() {}
```

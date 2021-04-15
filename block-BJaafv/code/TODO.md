1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```
// The first function returns the value of sum of a and b when called whereas the second function does not have a return keyword hence it will just log the value of sum of a and b but it will not return the value. It will just return undefined.

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

// The value of the variable `first` will be undefined and the value in variable `second` will be the sum value of a and b. 

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?

// If we call the first sum function with 3 parameters the output will be undefined because the function does not have a return keyword so cannot return any value passed as arguments.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?

// We can store the first function in a variable named add but when add is called it will return undefined as it is the output of the first sum function.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

```js
function sayHello(name){
  return `Hello ${name}`;
}
sayHello("Arya");
```

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
// The output of the function above will be "Hello, John". Since userName is a outer variable it will be accessed by the function showMessage() and the variable message will have "Hello, John" which will be returned to the function. 

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // John

showMessage(); // "Hello, John"

alert(userName); // John
```

8. What is a Anonymous Function give example of three functions.

An anonymous function is a function which is not named. For example:
```js
let anonymousFunctn = function(a,b){
  return a+b;
}
```
The above function type is function expression.
```js
let anonymousFunctn2 = (a,b) => {
  return a+b;
};
```
The above function type is Arrow function with curly braces.
```js
let anonymousFunctn3 = (a,b) => return a+b;
```
The above function type is Arrow function with Implicit return.

9. Can function declaration be a Anonymous Function? Explain

// In a function declaration we need to provide a function name otherwise it'll throw a Syntax error. If we want to make the function anonymous then we can use the function expression type of function and declare a variable which stores that function. Then we would not need to name that function.

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
// Some good naming conventions are:
checkAgeGroup();
getFullName();
calcSumOfNumbers();
sayHello();
addTwoNumbers();
createSpaceBetween();

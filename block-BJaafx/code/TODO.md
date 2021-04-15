1. Using loops take 10 inputs from user and find the average of all the numbers.

```js
function calcAverage(n1,n2,n3,n4,n5,n6,n7,n8,n9,n10){
  return (n1+n2+n3+n4+n5+n6+n7+n8+n9+n10) / 10;
}
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
```
The above code when executed will give a Reference Error since println is not a valid syntax. If we use alert instead it would alert `hi` 3 times. 


3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.

```js
function getEvenSum(max = 10){
  let sum = 0;
  for(let i = 0; i<=max;i++){
    if(i%2==0){
      sum = sum + i;
    }
  }
  return sum;
}
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.

```js
function getOddSum(max = 10){
  let sum = 0;
  for(let i = 0; i<=max;i++){
    if(i%2!==0){
      sum = sum + i;
    }
  }
  return sum;
}
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

```js
function getProductOfDigits(num){
  if(num < 0){
    return `not a valid input`;
  }else{
    let prod = 1;
    let str = String(num);
    for(let i=0;i<str.length;i++){
      prod = prod * Number(str[i]);
    }
    return prod;
  }
}
```

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return 'Bigger than 5';
  }

  if (num < 5) {
    return 'Smaller than 5';
  }

  return num;
}

check(10); // "Bigger than 5"
check(1); // "Smaller than 5"
check(5); // 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // "You are arya"
getOutput('John'); // "You are john"
getOutput(); // "Who are you"
```
Since there is a return statement for each condition it will return the value if the condition matches and if there is no argument passed then the default return value will be passed.

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // "Who are you"
getOutput('John'); // "Who are you"
getOutput(); // "Who are you"
```
Since there is no return keyword used in either if statements, therefore even if the value of the condition is matched it will not return anything. It will just log the value in console.log but will not return. It will return Who are you for all cases.


9. Can a function have multiple return statement? Give one example if possible and explain the reason.

A function can have multiple return statements. Whenever any one of the return statement is executed, the function is executed. But it can have multiple return statements.
```js
function sum(a,b){
  return a+b;
  return a-b;
}
sum(10,6);
```
The output will be 16 since the first return statement got executed and the function execution finished.


10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

The `for` loop contains an initialization of variable, the condition and what to do in each iteration. Whereas the `while` loop contains only a condition if that is true it executes the piece of code within it else it breaks out of the loop.

A `for` loop can be used when you are given an initial value, a final value and what to do after each iteration. For instance to find the sum of number from 1 to 10:
```js
let sum = 0;
for(let i = 0; i<=100;i++){
    sum = sum + i;
}
alert(sum);
```

A `while` loop when all you have is a condition. For instance:
```js
let i = 0;
while (i < 3){
  alert('hi');
  i++;
}
```
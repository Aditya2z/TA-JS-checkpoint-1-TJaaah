1. Using loops take 10 inputs from user and find the average of all the numbers.
```js
let average;
let number;
let sum = 0;
for(i = 1; i <= 10; i++) {
  number = +prompt(`Enter a number`);
  sum = sum + number;
  averge = sum / i;
}
```

2. What will be the output of the code below

```js
let i = 0;
while (i < 3) {
  println('hi');
  i++;
} // output it will throw error because println is not defined
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
```js
function getEvenSum(max = 10) {
  let evenSum = 0; 
  if(max % 2 === 0) {
    evenSum = evenSum + max;
  }
  return evenSum;
}
```

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
```js
function getOddSum(max = 10) {
  let oddSum = 0; 
  if(max % 2 !== 0 && typeof max === 'number') {
    oddSum = oddSum + max;
  }
  return oddSum;
}
```

5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.
```js
function getProductOfDigits(num) {
  if (num < 0) {
    return "not a valid input";
  }

  let product = 1;
  num = String(num);
  let numberOfDigits = num.length;
  num = Number(num);
  for (let i = 0; i < numberOfDigits ; i++) {
    product *= num % 10;
    num = (num - num % 10) / 10;
  }
  return product;
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

check(10); // output 'Bigger than 5'
check(1); // output 'Smaller than 5'
check(5); // output 5
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') return 'You are arya';
  if (name === 'John') return 'You are john';
  return 'Who are you';
}

getOutput('Arya'); // what will be the output 'You are arya'
getOutput('John'); // what will be the output 'You are john'
getOutput(); // what will be the output 'Who are you'
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === 'Arya') console.log('You are arya');
  if (name === 'John') console.log('You are john');
  return 'Who are you';
}

getOutput('Arya'); // what will be the output 'Who are you'
getOutput('John'); // what will be the output 'Who are you'
getOutput(); // what will be the output 'Who are you'
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
Yes, a function in JavaScript can have multiple return statements but only one of them will be executed at one time. Example:
```js
function getSign(num) {
  if (num > 0) {
    return "positive";
  } else if (num < 0) {
    return "negative";
  } else {
    return "zero";
  }
}
```
The reason for having multiple return statements is that the function is checking for different conditions, and returning different values based on the input number.

10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.
A for loop is typically used when you know the number of iterations that the loop needs to run for. The for loop has three parts: the initialization, the condition, and the increment/decrement.E.g.
```js
for (let i = 0; i < 10; i++) {
  console.log(i);
}
```
A while loop is typically used when you don't know the number of iterations that the loop needs to run for. A while loop will continue to execute as long as the specified condition is true. E.g.
```js
let i = 0;
while (i < 10) {
  console.log(i);
  i++;
}
```

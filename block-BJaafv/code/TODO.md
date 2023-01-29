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
Answer : the first fuction will return a number equivalent to the added arguments passing through the function  while the second function will lod the value of added numbers but will return undefined.

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

first = a + b;
second = undefined;

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?

It will add the first two arguments and ignore the last argument 35 as there is no parameter defined to store the argument.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?

yes we can stroe a function into a variable as fuctions are objects and objects are values and values are expressions and we can write expression on right hand side of =.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

function sayHello(name) { 
  return `Hello ${name}`;
  }

6. What will be the output of the function below and why?

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

showMessage();
```
It will return 'Hello, John' because global variables can be accessed in the function as well.

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = 'John';

function showMessage() {
  let message = 'Hello, ' + userName;
  return message;
}

alert(userName); // Output 1 
'John'

showMessage(); // Output 2
'Hello, John'

alert(userName); // Output 3
'John'
```

8. What is a Anonymous Function give example of three functions.
An anonymous function is a function without a name. Ex: 
```js
let square = x => x * x;
```
```js
let double = x => x + x;
```
```js
let add = function(x, y) {
    return x + y;
}
```

9. Can function declaration be a Anonymous Function? Explain

No, function declaration cannot be anonymous in JavaScript. A function declaration is a statement that declares a named function. The function name is required, and it must be unique within the scope in which it is declared.

```javascript
function add(x, y) {
    return x + y;
}
```

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.
```js
getCustomerName() //return a value of customer's name.
calculateTotalCost() //calculate something, in this case, the total cost of something.
createNewAccount() //create something, in this case, a new account.
checkPasswordStrength() //check something and return a Boolean, in this case, check the strength of a password.
getAverageRating() //return a value, in this case, the average rating of something.
```

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

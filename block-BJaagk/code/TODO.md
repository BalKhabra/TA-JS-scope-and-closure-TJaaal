1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
let amount = function percentage (marks, total) {
  return (${marks} * 100) / ${total};
}

let amount = (marks, total) => {
  return (${marks} * 100) / ${total};
}

let amount = function percentage(marks, total) {
  return (${marks} * 100) / ${total};
}
let amount = (marks, total) => (marks * 100) / total;
```

2. Write Function Declaration or Function Expression next to the function.

```js
let finalPercentage = function percentage(marks, total) {
  return (marks * 100) / total;
}
// Function Declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
```
<!-- Function Expression -->


```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
```
<!-- Function Expression -->


```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};

// Function Expression

```

```js
let percentage = (marks, total) => (marks * 100) / total;

// Function Expression

```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
allows us to create an anonymous function which doesn't have any function name which is the main difference between Function Expression and Function Declaration.
function myFunction(a, b) {
  return a * b;
}

4. Why is a function call an expression in JavaScript?
to execute a specified function with the provided arguments. If the function being called is overloaded, the compiler will attempt to match the argument types with the function parameter types. If there are no matching function declarations, a compile-time error will be raised.


5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // VALID 5
five = add; // VALID
five = five(10, 11); // VALID
five = function () {
  return 'Hello';
}; // VALID
```

6. What is the difference between function definition and function call? Explain with an example.
declare and define are the same, and they mean when you write all the code for your function. At that point the function just sits there doing nothing. call is when you tell the JavaScript interpreter to run the code in your function.

7. What is the similarities between function definition and function call?
A function is a piece of code which enhanced the reusability and modularity of your program. It means that piece of code need not be written again. A function call means invoking or calling that function.
8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid because function is internally an object so this works
```

9. What is higher order function explain with an example.
 A Higher-Order function is a function that receives a function as an argument or returns the function as output. For example, Array. prototype. map , Array.
 
10. Explain what is callback function. Why you can pass a function inside a function?
A callback function is a function passed into another function as an argument, which is then invoked inside the outer function to complete some kind of routine or action
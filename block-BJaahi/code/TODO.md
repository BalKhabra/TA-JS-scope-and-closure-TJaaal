For the given code below:

- re-write the code in ways that system will understand

For Example:

1.
                                                                                   
```js
var username = 'Arya';
let brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// Declaration Phase
var username = undefined;
let brothers;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMessage = undefined;

// Execution Phase

username = 'Arya';
brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

message = sayHello(username);
nextMessage = sayHello('Test');
```

2.

```js
console.log(username, numbers);

var username = 'Arya';
let number = 21;

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

<!-- //declaration phase -->
```js
var username = undefined;
let number;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMessage = undefined;

//execution phase
username = 'Arya';
number = 21;

console.log(username, number);

message = sayHello(username);
nextMessage = sayHello('Test');
```



3.

```js
console.log(username, numbers);
let username = 'Arya';
let number = 21;

let sayHello = function (name) {
  return `Hello ${name}`;
};

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// declaration phase
let username;
let number;
let sayHello;
let message;
var nextMessage = undefined;

//execution phase
console.log(username, numbers);
username= 'Arya';
number = 21;
sayHello = function (name) {
  return `Hello ${name}`;
};
message = sayHello(username);
nextMessage = sayHello('Test');
```

4.

```js
let username = 'Arya';
console.log(username, numbers);

let number = 21;
let message = sayHello(username);

let sayHello = function (name) {
  return `Hello ${name}`;
};

var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// declaration phase
let username;
let number;
let sayHello;
var nextMessage = undefined;


//execution phase
username = 'Arya'
console.log(username, numbers);
number = 21;
message = sayHello(username);
sayHello = function (name) {
  return `Hello ${name}`;
};

nextMessage = sayHello('Test');
```

5.

```js
console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;
```

<!-- Answer -->

```js
var name = undefined;
let age;

//execution phase
console.log(name);
console.log(age);
name = 'Lydia';
age = 21;
```

6.

```js
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

sayHi();
```

<!-- Answer -->

```js
//declaration phase
function sayHi(name) {
  var name = undefined;
  let age;
}

sayHi();

//execution phase
console.log(name);
  console.log(age);
  name = 'Lydia';
  age = 21;
```

7.

```js
sayHi();
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}
```

<!-- Answer -->

```js
//declaration phase
function sayHi(name) {
  var name = undefined;
  let age;
//executio phase
  console.log(name);
  console.log(age);
  name = 'Lydia';
  age = 21;
}
sayHi();

```

8.

```js
sayHi();
let sayHi = function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
};
```

<!-- Answer -->

```js
let sayHi
sayHi();
sayHi = function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
};```

9.

```js
let num1 = 21;
console.log(sum);
var sum = num1 + num2;
let num2 = 30;
```

<!-- Answer -->

```js
let num1;
var sum = undefined;
let num2 = udefined


console.log(sum)
num1 = 21;
sum = num1 + num2;
num2 = 30;
```

10.

```js
var num1 = 21;

let sum2 = addAgain(num1, num2, 4, 5, 6);

let add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgian(a, b) {
  return a + b;
}
let num2 = 200;

let sum = add(num1, num2, 4, 5, 6);
```

<!-- Answer -->

```js
var num1 = undefined;
let sum2;
let add;
function addAgian(a, b) {
  return a + b;
}
let num2 ;
let sum;

//execution phase
num1 = 21;
sum2 = addAgain(num1, num2, 4, 5, 6);
add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgian(a, b) {
  return a + b;
}
num2 = 200;
sum = add(num1, num2, 4, 5, 6);
```

11.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

let add = (a, b) => {
  return a + b;
};
```

<!-- Answer -->

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}
let sum;
let add;

//execution
function test(a) {
  num1 = 21;
  return add(a, num1);
}

sum = test(100);

add = (a, b) => {
  return a + b;
};
};```

12.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

function add(a, b) {
  return a + b;
}
```

<!-- Answer -->

```js
function test(a) {
  let num1;
  return add(a, num1);
}

let sum;

function add(a, b) {
  return a + b;

//execution phase
function test(a) {
  num1 = 21;
  return add(a, num1);
}

sum = test(100);

function add(a, b) {
  return a + b;
}
}```

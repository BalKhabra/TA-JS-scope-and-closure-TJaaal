1. What does thread of execution means in JavaScript?
It goes through it line by line, and does each of the line of code, they call this the thread of execution

2. Where the JavaScript code gets executed?
Whenever the JavaScript engine receives a script file, it first creates a default Execution Context known as the Global Execution Context (GEC) . The GEC is the base/default Execution Context where all JavaScript code that is not inside of a function gets executed. For every JavaScript file, there can only be one GEC

3. What does context means in Global Execution Context?
The Execution Context contains the code that's currently running, and everything that aids in its execution. During the Execution Context run-time, the specific code gets parsed by a parser, the variables and functions are stored in memory, executable byte-code gets generated, and the code gets executed

4. When do you create a global execution context.
When scripts load in the browser, the Global context is created as the default context where the JS engine starts executing code and is placed at the bottom of the execution stack. The JS engine then searches for function calls in the code.

5. Execution context consists of what all things?
The Execution Context contains the code that's currently running, and everything that aids in its execution.

6. What are the different types of execution context?
Global Execution Context (GEC)
Function Execution Context (FEC)

7. When global and function execution context gets created?
Whenever the JavaScript engine receives a script file for GEC
created when JS engine whenever it finds any function call FEC

8. Function execution gets created during function execution or while declaring a function.
 Every time a function is invoked, a brand new execution context is created for that function. Each function has its own execution context, but it's created when the function is invoked or called. There can be any number of function execution contexts

9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->


![](./code/GEC.jpeg)



```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](./img/image-name.jpg)



```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](./img/image-name.jpg)gec.jpg
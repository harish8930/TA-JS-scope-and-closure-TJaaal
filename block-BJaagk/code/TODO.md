1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let marksPercentage = function(marks,total){
  return(marks*100)/total;
}

let marksPercentage = (marks,total) => {
  return(marks*100)/total;
}


2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Your answer
percentage(400,500);

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
```
let percentage = function (marks,total){
return(marks*100)/total;
}
```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};


```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
```

```js
let percentage = (marks, total) => (marks * 100) / total;
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.
it is because fnction is an object in javascript, that's why  function definition is an expression .

5. Why is a function call an expression in JavaScript?

6. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // valid
five = add; // invalid
five = five(10, 11); // invalid
five = function () {
  return 'Hello';
}; // Valid
```

6. What is the difference between function definition and function call? Explain with an example.
answer// function definition is the step where we define that what will be the steps to be executed and function call is the execution of function.
7. What is the similarities between function definition and function call?
answer// Parameters: Both function calls and function definitions can accept parameters. Parameters allow you to pass values to a function for processing. The same parameter names should be used in both the function call and the function definition to ensure proper data transfer.
8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam'; // valid or invalid
```

9. What is higher order function explain with an example.
answer// A higher-order function is a function that accepts functions as parameters and/or returns a function.

11. Explain what is callback function. Why you can pass a function inside a function?
answer// A callback is a function passed as an argument to another function. This technique allows a function to call another function. A callback function can run after another function has finished.

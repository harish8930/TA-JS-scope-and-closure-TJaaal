Create the execution context diagram for the following code snippets:

```js
function outer() {
  let b = 10;
  function inner() {
    let a = 20;
    console.log(a + b);
  }
  return inner;
}
let getSum = outer();
let num = getSum();
```
![WhatsApp Image 2023-06-23 at 5 02 30 PM](https://github.com/harish8930/TA-JS-scope-and-closure-TJaaal/assets/129581462/cb50b77a-9e67-4799-888c-28837432e99a)

2.

Create the execution context diagram for following code. Also write the output of the code below.

```js
function getCounter() {
  let count = 0;

  return () => {
    return count++;
  };
}

let counter = getCounter();

counter(); 0
counter(); 1
counter(); 2
counter(); 3
![WhatsApp Image 2023-06-23 at 5 02 29 PM (1)](https://github.com/harish8930/TA-JS-scope-and-closure-TJaaal/assets/129581462/35a96406-77c6-4647-9ad7-befd1514cb88)


3. Create the execution context diagram

```js
function makeColorChanger(color) {
  return function () {
    document.body.style.backgroundColor = color;
  };
}

let blue = makeColorChanger('blue');
let tomato = makeColorChanger('tomato');

blue();
tomato();

// What will be the background color after the execution of last line
```

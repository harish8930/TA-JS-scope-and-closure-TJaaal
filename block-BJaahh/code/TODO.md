## Getting to understand closure properly

1. Write a function called `multiplyBy` that takes a `number` as an argument and returns a function. Returned function takes another `number` as an argument and returns the multiplication of both the numbers.

function multiplyBy(number) {
  return function (anotherNumber) {
    return number * anotherNumber;
  };
}

// Usage
const multiplyByTwo = multiplyBy(2);
console.log(multiplyByTwo(4)); // Output: 8

const multiplyByFive = multiplyBy(5);
console.log(multiplyByFive(3)); // Output: 15


2. Write a function called `fullName` that takes a string `firstName` as an argument and returns a function. Returned function takes another string `lastName` as an argument and returns full name.

```js
function fullname(fn){
return function (ln){
    return `${fn}  ${ln}`
}

}
const firstname = fullname("dwayne")
 console.log(firstname("johnson"));
 //output dwayne johnson

3. Write a function called `isInBetween` which takes two parameter `a` and `b` and returns a function. When you call the returned function with any number it returns `true` if the value is in between `a` and `b`.

function isInbetween(a,b){
    return function(value){
if(value > a && value <  b){
    console.log(true);
}else{
    console.log(false);
}
    }
}


const isChild = isInbetween(10,100);
isChild(16); //output true;
isChild(109);// output false;


4. Write a function call `letsWishThem` that take one parameter `string` called `greeting` and returns a function that takes another argument called `message`.

```js
function letsWishThem(greeting){
return function (message){
    return `${greeting} ${message}`
}
}

const hello = letsWishThem("Hey");
hello(" How are you ?");
console.log(hello("How are you ? "));
```

5. Write a function called `addGame` which takes a string (name of the game) and the current score. It returns a function calling that will increment the score by one and print something like `Score of Basketball is 1`.

```js
function addGame(gameName,score){
return function(){
 score++
console.log(`score of ${gameName} is ${score} `)

}

}

const gamescore = addGame('cricket',0);
gamescore();

// Output
const hockey = addGame('Hockey', 0);
hockey(); // Your score of Hockey is 1
hockey(); // Your score of Hockey is 2
const cricket = addGame('Cricket', 1);
cricket(); // Your score of Cricket is 2
cricket(); // Your score of Cricket is 2
```

6. Write a function called `getCard` which takes one of these options (club, spade, heart, diamond) returns a function calling that function returns random card (2,3,4,5,6,7,8,9,10,J, Q, K, A) of that suit.

```js
function getCard(suit) {
  // your code goes here
}

// Output
const randomClub = getCard('Club');
randomClub(); // Card is: 6 Club
randomClub(); // Card is: A Club
const randomSpade = getCard('Spade');
randomSpade(); // Card is: 6 Spade
randomSpade(); // Card is: A Spade
```

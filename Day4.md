

# Day 4: Basic JavaScripts

## Lesson Summary

### Event Handlers
Event handlers allow us to detect and respond to events on the DOM. Here are the key points covered in this lesson:<br>

- We can use the .addEventListener method to attach event listeners to DOM elements.<br>
- Event listeners take in two parameters: the name of the event to listen for, and a handler function to run when the event occurs.<br>
- The event object provides information about the event, such as the target element and event type.<br>
```javascript
// Example 1: Event Handlers
const button = document.querySelector("#myButton");

button.addEventListener("click", () => {
  console.log("Button clicked!");
});
```

### Conditionals
Conditionals allow us to execute code based on certain conditions. Here are the key points covered in this lesson:<br>

- Conditional statements, such as if and else, allow us to run different blocks of code based on specific conditions.<br>
- Logical operators like && (and), || (or), and ! (not) can be used to create complex conditional expressions.<br>
- Loops, such as for and while, allow us to repeat code execution based on a specified condition.<br>

```javascript
// Example 2: Conditionals
const age = 21;
const name = "Aya AbuAli";

if (age >= 18) {
  console.log("You are an adult.");
} else {
  console.log("You are a minor.");
}

if (name.length > 10) {
  console.log("Your name is long.");
} else {
  console.log("Your name is short.");
}

```

### Map and Filter
The map and filter methods provide powerful tools for array manipulation. Here are the key points covered in this lesson:<br>

- The map method iterates over an array and calls a function on each item, creating a new array with the results.<br>
- The filter method processes an array and returns a new array containing only the items that meet a specified condition.<br>
- The spread operator (...) can be used to insert all items from one array into another.<br>
```javascript
// Example 3: Map and Filter
const numbers = [1, 2, 3, 4, 5];

const multipliedNumbers = numbers.map((num) => num * 2);
console.log(multipliedNumbers); // Output: [2, 4, 6, 8, 10]

const evenNumbers = numbers.filter((num) => num % 2 === 0);
console.log(evenNumbers); // Output: [2, 4]
// Example: Using the Spread Operator
const array1 = [1, 2, 3];
const array2 = [4, 5, 6];

const combinedArray = [...array1, ...array2];

console.log(combinedArray);
// Output: [1, 2, 3, 4, 5, 6]
```


## Coding Exercises

[Use Multiple Conditional (Ternary) Operators](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/use-multiple-conditional-ternary-operators)
#### My Solution
```javascript
function checkSign(num) {
return num===0?"zero":num>0?"positive":"negative";
}

checkSign(10);
```

[Golf Code](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/golf-code)

#### My Solution
```javascript
const names = ["Hole-in-one!", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"];

function golfScore(par, strokes) {
  // Only change code below this line


  return strokes===1?names[0]:strokes<=par-2?names[1]:strokes===par-1?names[2]:strokes===par?names[3]:strokes===par+1?names[4]:strokes===par+2?names[5]:"Go Home!";
  // Only change code above this line
}

golfScore(5, 4);
```


[Use the map Method to Extract Data from an Array](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/use-the-map-method-to-extract-data-from-an-array)

#### My Solution
```javascript
// Only change code below this line

const ratings = watchList.map((movie) => {
  return {
    title: movie.Title,
    rating: movie.imdbRating,
  };
});


// Only change code above this line

console.log(JSON.stringify(ratings));


```
[Use the filter Method to Extract Data from an Array](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/functional-programming/use-the-filter-method-to-extract-data-from-an-array)
#### My Solution
```javascript
// Only change code below this line
const notFilteredList = watchList.map((movie) => {
  return {
    title: movie.Title,
    rating: movie.imdbRating,
  };
});
const filteredList = notFilteredList
.filter(e=>e.rating > 8)
// Only change code above this line
```



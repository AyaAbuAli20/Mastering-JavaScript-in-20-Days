
# Day 3: Basic JavaScripts

## Lesson Summary

### Functions 
Functions are one of the fundamental building blocks in JavaScript. A function in JavaScript is similar to a procedure—a set of statements that performs a task or calculates a value, but for a procedure to qualify as a function, it should take some input and return an output where there is some obvious relationship between the input and the output. To use a function, you must define it somewhere in the scope from which you wish to call it.
```javascript
function half(x){
return x/2;}
const one = helf(2);
```
#### Coding Examples
```javascript
funtion multiply(a,b){
return a*b;
}
```
```javascript
funtion yell(saying){
return saying.toUperCase();
}
```
```javascript
funtion longerThan(a,b){
return a.length() > b.length();
}
```


### Arrow Functions
The => "fat arrow" let us create an unnamed function without much code
```javascript
(x,y) => x+y
```
aka an arrow function
#### Coding Examples
```javascript
const divide= (x,y) => x/y
divide(9/3)
```
```javascript
const whisper= (text) => text.lowerCase()
whisper(OMG)
```
```javascript
const shourterThan= (x,y) => x<y
shourterThan([1,2],[1,2,3])
```
### Scope
scope:determines where varibles are "in play"
-the widest scope is the global scope.
-each function gets its own scope within the scope where it was declared.



## Coding Exercises

[Return a Value from a Function with Return](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/return-a-value-from-a-function-with-return)
#### My Solution
```javascript
function timesFive(num) {
  return num *5;
}

const answer = timesFive(5);
```

[Global Scope and Functions](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/global-scope-and-function)

#### My Solution
```javascript
// Declare the myGlobal variable below this line
let myGlobal=10;

function fun1() {
  // Assign 5 to oopsGlobal here
 oopsGlobal=5;
}

// Only change code above this line

function fun2() {
  let output = "";
  if (typeof myGlobal != "undefined") {
    output += "myGlobal: " + myGlobal;
  }
  if (typeof oopsGlobal != "undefined") {
    output += " oopsGlobal: " + oopsGlobal;
  }
  console.log(output);
}
```


[Local Scope and Functions](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/local-scope-and-functions)

#### My Solution
```javascript
function myLocalScope() {
  // Only change code below this line
let myVar=5;
  console.log('inside myLocalScope', myVar);
}
myLocalScope();

// Run and check the console
// myVar is not defined outside of myLocalScope
console.log('outside myLocalScope', myVar);

```
[Stand in Line](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/stand-in-line)
#### My Solution
```javascript
function nextInLine(arr, item) {
  // Only change code below this line
  arr.push(item);
  let x = arr.shift();
  return x;
  
  // Only change code above this line
}

// Setup
let testArr = [1, 2, 3, 4, 5];

// Display code
console.log("Before: " + JSON.stringify(testArr));
console.log(nextInLine(testArr, 6));
console.log("After: " + JSON.stringify(testArr));
```



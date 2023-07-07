
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

- [Return a Value from a Function with Return](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-javascript/return-a-value-from-a-function-with-return)
#### My Solution
```javascript
function timesFive(num) {
  return num *5;
}

const answer = timesFive(5);
```

 [Copy Array Items Using Slice](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-data-structures/copy-array-items-using-slice)

#### My Solution
```javascript
function forecast(arr) {


arr= arr.slice(2, 4);
  return arr;
}


console.log(forecast(['cold', 'rainy', 'warm', 'sunny', 'cool', 'thunderstorms']));
```


[Combine Arrays with the Spread Operator](https://www.freecodecamp.org/learn/javascript-algorithms-and-data-structures/basic-data-structures/combine-arrays-with-the-spread-operator)

#### My Solution
```javascript
function spreadOut() {
  let fragment = ['to', 'code'];
  let sentence=['learning',...fragment,'is', 'fun']; // Change this line
  return sentence;
}

console.log(spreadOut());

```



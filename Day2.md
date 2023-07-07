# Day 2: Basic JavaScripts

## Lesson Summary

### Expressions 
Regular expressions are patterns used to match character combinations in strings. In JavaScript, regular expressions are also objects. These patterns are used with the exec() and test() methods of RegExp, and with the match(), matchAll(), replace(), replaceAll(), search(), and split() methods of String. This chapter describes JavaScript regular expressions.


### Arrays
The Array object, as with arrays in other programming languages, enables storing a collection of multiple items under a single variable name, and has members for performing common array operations.
let us keep mutiple value togather.
```javascript
let number = [100,2,50];
```
-it have length, index
-arrays can do lots of useful tricks! like:sort()/join()/concat().
```javascript
 number.sort(); 
```
-mutability
```javascript
 number[1]=150; 
```

### Objects
 It is used to store various keyed collections and more complex entities.
 ```javascript
 const person={
name:"Aya",
age: 21,
gender: "Female"}
person.name
```
-object Methodes
 .dog.speak();
 .Nested object
 .objects in array and object
-Built_in objects
 .document
 .Math
 .String



## Coding Exercises

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



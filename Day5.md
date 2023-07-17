


# Day 5: Basic JavaScripts

## Lesson Summary

###  Data Fetching & Promises
In this lesson, we explore fetching data from an API endpoint using the fetch function and working with promises. Here are the key points covered in this lesson:<br>

- Using the fetch function to load data from an API endpoint.<br>
- Understanding the states of a promise: pending, fulfilled, and rejected.<br>
- Using the await operator to wait for a promise and obtain its resulting value.<br>
```javascript
async function fetchData(url) {
  const response = await fetch(url);
  const data = await response.json();
  return data;
}

const apiUrl = "https://api.example.com/data";
const result = await fetchData(apiUrl);
console.log(result);
});
```

###  Destructuring Data
Destructuring allows us to declare multiple variables at once by extracting values from objects or arrays. Here are the key points covered in this lesson:<br>

- Destructuring objects to retrieve values from properties.<br>
- Destructuring arrays using square brackets.<br>
- Applying destructuring in various scenarios to simplify code.<br>
```javascript
const person = {
  name: "Aya Abu Ali",
  age: 21,
  city: "Bethlehem",
};

const { name, age } = person;
console.log(name); // Output: "Aya Abu Ali"
console.log(age); // Output: 21

```

### Async Functions
Async functions provide a cleaner syntax for writing asynchronous code. Here are the key points covered in this lesson:<br>

- Combining async fetching and parsing into a single function.<br>
- Using the await keyword to retrieve the contents of a returned promise.<br>
- Handling errors and exceptions in async functions.<br>
```javascript
async function fetchData(url) {
  try {
    const response = await fetch(url);
    const data = await response.json();
    return data;
  } catch (error) {
    console.error(error);
    throw new Error("An error occurred while fetching data.");
  }
}

const apiUrl = "https://api.example.com/data";
try {
  const result = await fetchData(apiUrl);
  console.log(result);
} catch (error) {
  console.error(error);
}
```

### Modules
Modules allow us to split large codebases into smaller files for better organization and reusability. Here are the key points covered in this lesson:<br>

- Understanding the differences between JavaScript and module JavaScript.<br>
- Importing and exporting modules using the import and export keywords.<br>
- Debugging and error handling techniques.<br>
```javascript
// Module 1: math.js
export function add(a, b) {
  return a + b;
}

// Module 2: utils.js
export function capitalize(str) {
  return str.charAt(0).toUpperCase() + str.slice(1);
}

// Main file: main.js
import { add } from "./math.js";
import { capitalize } from "./utils.js";

console.log(add(2, 3)); // Output: 5
console.log(capitalize("hello")); // Output: "Hello"
```
## Coding Exercises




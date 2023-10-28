# my-javascript-references
This is the js reference repo
[AVidhanR](github.com/AVidhanR)

*************************************************************************

### Map method
The map() method in JavaScript is a higher-order function used to transform elements of an array. 
It takes a callback function as an argument and applies that function to each item in the array, creating a new array with the results.

> The syntax is
```javascript
const newArray = array.map(callback(element, index, array) => {
  // return transformed element
});
```
> The callback function is executed for every element, and the transformed values are collected in a new array.
  This is a powerful tool for efficiently manipulating data within arrays, making it a fundamental part of modern JavaScript programming, 
  often used for tasks like data transformation, filtering, and rendering lists in web applications.

--------------------------------------------------------------------------

### Set
In JavaScript, a Set is a built-in data structure that allows you to store unique values, which means it automatically eliminates duplicates. Sets are useful for efficiently managing collections of data with no repeated elements. You can add, delete, or check for the existence of elements in a Set. Here's the syntax and a brief explanation:

>The Syntax is
```javascript
const mySet = new Set(); // Create a new Set
mySet.add(value); // Add a value to the Set
mySet.delete(value); // Remove a value from the Set
mySet.has(value); // Check if a value exists in the Set
mySet.size; // Get the number of unique values in the Set
```
> Sets are commonly used when you need to maintain a unique list of items or check for the presence of specific values within a collection.

--------------------------------------------------------------------------

### Dynamic Object Keys
In JavaScript, dynamic object keys refer to the ability to create objects with keys (property names) that are determined at runtime, rather than having them hardcoded. This is often achieved using square brackets [] to define keys. Here's an explanation and the syntax for creating objects with dynamic keys:

> Example (alike Syntax)
```javascript
const dynamicKey = "someKey"; // The dynamic key determined at runtime
const dynamicValue = "someValue"; // The corresponding value
const myObject = {
  [dynamicKey]: dynamicValue, // Using square brackets to create an object with dynamic keys
};
// Accessing the value using the dynamic key
const retrievedValue = myObject[dynamicKey];
```
> In this example, dynamicKey is a variable that holds the key, and dynamicValue is the corresponding value. We use square brackets to create an object with the key-value pair, and you can also use the same dynamic key to access the value from the object. Dynamic object keys are useful when you need flexibility in defining object properties based on runtime conditions.

--------------------------------------------------------------------------

### Array Destructing
Array destructuring in JavaScript is a technique that allows you to extract values from arrays and assign them to variables in a concise and readable way. Here's an explanation with syntax:

**Syntax:**
```javascript
const [var1, var2, ...rest] = myArray;
```

- `var1`, `var2`: Variables that will receive values from the array.
- `...rest`: The rest operator (`...`) collects the remaining elements of the array into a new array.

Example:
```javascript
const fruits = ['apple', 'banana', 'cherry'];
const [first, second] = fruits;

console.log(first); // Output: 'apple'
console.log(second); // Output: 'banana'
```

You can also use default values:
```javascript
const [x = 1, y = 2] = [10];
console.log(x); // Output: 10
console.log(y); // Output: 2
```

> Array destructuring is a powerful feature that simplifies code when working with arrays and is commonly used in various JavaScript applications.

--------------------------------------------------------------------------

### Filter and Find 
In JavaScript, the `filter()` method is used to create a new array by filtering elements from an existing array based on a provided condition. It returns an array containing only the elements for which the condition is true.

Syntax:
```javascript
const newArray = array.filter(function(element, index, array) {
  // Return true to keep the element, or false to exclude it
});
```

Example:
```javascript
const numbers = [1, 2, 3, 4, 5];
const evenNumbers = numbers.filter(function(number) {
  return number % 2 === 0;
});
// evenNumbers will contain [2, 4]
```

The `find()` method is used to retrieve the first element in an array that matches a specified condition. It returns the first matching element or `undefined` if no match is found.

Syntax:
```javascript
const result = array.find(function(element, index, array) {
  // Return true to indicate a match
});
```

Example:
```javascript
const people = [
  { name: "Alice", age: 25 },
  { name: "Bob", age: 30 },
  { name: "Charlie", age: 35 }
];
const person = people.find(function(person) {
  return person.age === 30;
});
// person will contain { name: "Bob", age: 30 }
```

> In both methods, the callback function is called for each element in the array, and the result is based on the condition specified in the function. `filter()` returns an array of all matching elements, while `find()` returns the first matching element.

--------------------------------------------------------------------------

### Reduce
In JavaScript, the `reduce()` method is used to iterate through an array and accumulate its elements into a single value. It applies a specified function to each element of the array, taking an accumulator and the current element as arguments, and returns the final accumulated result. 

Syntax:
```javascript
array.reduce(callback(accumulator, currentValue, currentIndex, array), initialValue);
```

- `array`: The array to be reduced.
- `callback`: A function that is called for each element in the array, which takes four parameters:
  - `accumulator`: A value that accumulates the results.
  - `currentValue`: The current element being processed.
  - `currentIndex` (optional): The index of the current element.
  - `array` (optional): The original array being iterated.
- `initialValue` (optional): An initial value for the accumulator. If not provided, the first element of the array is used as the initial accumulator value.

Here's a simple example:
```javascript
const numbers = [1, 2, 3, 4, 5];
const sum = numbers.reduce((accumulator, currentValue) => accumulator + currentValue, 0);
console.log(sum); // Output: 15
```

> In this example, the `reduce()` method adds up all the elements in the `numbers` array, starting with an initial accumulator value of 0.

--------------------------------------------------------------------------


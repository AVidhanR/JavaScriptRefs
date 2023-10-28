# my-javascript-references
This is the js reference repo
[AVidhanR](github.com/AVidhanR)
--------------------------------------------------------------------------
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

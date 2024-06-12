
# JavaScript Array Challenges

## Challenge 1: Sum of Array Elements
**Difficulty**: Beginner

Write a function `sumArray` that takes an array of numbers as input and returns the sum of all the elements in the array.

```javascript
function sumArray(numbers) {
  // Your code here
}

// Example usage:
console.log(sumArray([1, 2, 3, 4])); // Output: 10
console.log(sumArray([10, -10, 10, -10])); // Output: 0
```

## Challenge 2: Find the Maximum Element
**Difficulty**: Easy

Write a function `findMax` that takes an array of numbers as input and returns the maximum element in the array.

```javascript
function findMax(numbers) {
  // Your code here
}

// Example usage:
console.log(findMax([1, 2, 3, 4, 5])); // Output: 5
console.log(findMax([-10, -20, -30, -1])); // Output: -1
```

## Challenge 3: Remove Duplicates from Array
**Difficulty**: Intermediate

Write a function `removeDuplicates` that takes an array as input and returns a new array with all duplicate elements removed.

```javascript
function removeDuplicates(arr) {
  // Your code here
}

// Example usage:
console.log(removeDuplicates([1, 2, 2, 3, 4, 4, 5])); // Output: [1, 2, 3, 4, 5]
console.log(removeDuplicates(['a', 'b', 'a', 'c', 'b'])); // Output: ['a', 'b', 'c']
```

## Challenge 4: Flatten a Nested Array
**Difficulty**: Advanced

Write a function `flattenArray` that takes a nested array (array of arrays) as input and returns a new array with all the elements flattened to a single level.

```javascript
function flattenArray(nestedArray) {
  // Your code here
}

// Example usage:
console.log(flattenArray([1, [2, 3], [4, [5, 6]], 7])); // Output: [1, 2, 3, 4, 5, 6, 7]
console.log(flattenArray([['a', 'b'], ['c', ['d', 'e']], 'f'])); // Output: ['a', 'b', 'c', 'd', 'e', 'f']
```

## Challenge 5: Group Elements by Frequency
**Difficulty**: Expert

Write a function `groupByFrequency` that takes an array as input and returns an object where the keys are the elements and the values are the number of times each element appears in the array.

```javascript
function groupByFrequency(arr) {
  // Your code here
}

// Example usage:
console.log(groupByFrequency([1, 2, 2, 3, 3, 3, 4])); // Output: { '1': 1, '2': 2, '3': 3, '4': 1 }
console.log(groupByFrequency(['apple', 'banana', 'apple', 'orange', 'banana', 'apple'])); // Output: { 'apple': 3, 'banana': 2, 'orange': 1 }
```

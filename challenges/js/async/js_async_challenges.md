# JavaScript Async Challenges

## Theoretical Questions

### 1. What are JavaScript Promises and how do they work?

Describe what JavaScript Promises are, how they work, and how they are used to manage asynchronous operations.

### 2. What is the difference between synchronous and asynchronous code in JavaScript?

Explain the difference between synchronous and asynchronous code execution in JavaScript, including the impact on performance and user experience.

### 3. What is the difference between async/await, try-catch, promises, and callbacks?

Explain the differences between `async/await`, `try-catch`, promises, and callbacks in JavaScript, including how they are used for handling asynchronous operations and error handling.

### 4. How do functions behave differently in ES6+ compared to ES5?

Describe the differences in function behavior between ES6+ and ES5, including syntax differences such as arrow functions, default parameters, and the use of `this`.

### 5. What is the event loop and how does it work?

Explain the concept of the event loop in JavaScript, detailing how it handles asynchronous operations and the execution of code in a non-blocking manner.


## Challenge 1: Fetch Data from an API
**Difficulty**: Beginner

Write an asynchronous function `fetchData` that fetches data from a given URL and returns the data as a JavaScript object.

```javascript
// parameter url is a string. ex: url = 'https://jsonplaceholder.typicode.com/posts/1'
async function fetchData(url) {
  // Your code here
}

// Example usage:
fetchData('https://jsonplaceholder.typicode.com/posts/1')
  .then(data => console.log(data)) 
  .catch(error => console.error(error)); 
// Output: {userId: 1, id: 1, title: '...', body: '...'}
```

## Challenge 2: Delay Execution
**Difficulty**: Easy

Write an asynchronous function `delay` that takes a number of milliseconds as input and returns a promise that resolves after that number of milliseconds.

```javascript
// parameter ms is a number. ex: ms = 1000
function delay(ms) {
  // Your code here
}

// Example usage:
delay(1000).then(() => console.log('Executed after 1 second'));
// Output: Executed after 1 second (after 1 second delay)
```

## Challenge 3: Fetch Multiple APIs Concurrently
**Difficulty**: Intermediate

Write an asynchronous function `fetchMultiple` that takes an array of URLs, fetches data from all the URLs concurrently, and returns an array of the results.

```javascript
// parameter urls is an array of strings. ex: urls = ['https://jsonplaceholder.typicode.com/posts/1', 'https://jsonplaceholder.typicode.com/posts/2']
async function fetchMultiple(urls) {
  // Your code here
}

// Example usage:
fetchMultiple(['https://jsonplaceholder.typicode.com/posts/1', 'https://jsonplaceholder.typicode.com/posts/2'])
  .then(data => console.log(data)) 
  .catch(error => console.error(error)); 
// Output: [{userId: 1, id: 1, title: '...', body: '...'}, {userId: 1, id: 2, title: '...', body: '...'}]
```

## Challenge 4: Retry Fetch on Failure
**Difficulty**: Advanced

Write an asynchronous function `retryFetch` that takes a URL and a number of retries. It should attempt to fetch the data from the URL, retrying up to the specified number of times if it fails.

```javascript
// parameter url is a string. ex: url = 'https://jsonplaceholder.typicode.com/posts/1'
// parameter retries is a number. ex: retries = 3
async function retryFetch(url, retries) {
  // Your code here
}

// Example usage:
retryFetch('https://jsonplaceholder.typicode.com/posts/1', 3)
  .then(data => console.log(data)) 
  .catch(error => console.error('Failed to fetch after 3 retries', error));
// Output: {userId: 1, id: 1, title: '...', body: '...'} or 'Failed to fetch after 3 retries' error message
```

## Challenge 5: Throttle Function Execution
**Difficulty**: Expert

Write an asynchronous function `throttle` that takes a function and a delay as input. It should return a new function that, when invoked repeatedly, will only call the original function at most once per specified delay.

```javascript
// parameter fn is a function. ex: fn = () => console.log('Throttled function executed')
// parameter delay is a number. ex: delay = 2000
function throttle(fn, delay) {
  // Your code here
}

// Example usage:
const throttledFunction = throttle(() => console.log('Throttled function executed'), 2000);
setInterval(throttledFunction, 500);
// Output: 'Throttled function executed' (only once every 2 seconds, despite being called every 0.5 seconds)
```

These challenges will help you improve your understanding and mastery of JavaScript asynchronous programming, from basic fetch operations to advanced throttling and retry mechanisms.
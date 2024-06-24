# JavaScript Async Challenges

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
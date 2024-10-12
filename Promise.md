## Promise.all

`Promise.all()` is frequently used when there are multiple concurrent API requests, and we want to wait for all of them to have 
completed before continuing with code execution. This is usually necessary because we depend on data from all the responses.

```javascript
const [userData, postsData, tagsData] = await Promise.all([
  fetch('/api/user'),
  fetch('/api/posts'),
  fetch('/api/tags'),
]);
```

Let's implement our own version of Promise.all(), a promiseAll function, with the difference being the function takes in an array 
instead of an iterable.Be sure to read the description carefully and implement accordingly!

### Example 
```javascript
// Rejection example.
const p0 = Promise.resolve(30);
const p1 = new Promise((resolve, reject) => {
  setTimeout(() => {
    reject('An error occurred!');
  }, 100);
});

try {
  await promiseAll([p0, p1]);
} catch (err) {
  console.log(err); // 'An error occurred!'
}
```

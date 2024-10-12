## MakeCounter

### Description
`makeCounter` is a function that accepts an optional integer value and returns a new function. The returned function, when called, behaves as a counter. On the first call, it returns the initial value (if provided), otherwise it returns 0. Each subsequent call increases the returned value by 1.

**Parameters**
- `initialValue` (optional): A starting integer value for the counter. Defaults to `0` if not provided.

**Returns**
- A function that, when called, returns the next value in the counting sequence, starting from `initialValue` (or 0 by default).

### Example

```javascript
const counter = makeCounter();
console.log(counter()); // 0
console.log(counter()); // 1
console.log(counter()); // 2
```

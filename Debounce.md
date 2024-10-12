## Debounce

**Debouncing** is a technique used to control how frequently a function is executed over time. When a JavaScript function is debounced with a wait time of `X` milliseconds, 
it will only be executed after `X` milliseconds have passed since the last invocation of the debounced function. A common example of debouncing in everyday life is when 
you are in an elevator: the door will only close after a certain time has passed without pressing the "Door open" button.

### Implementation
The `debounce` function takes two parameters:
1. **Callback function**: The function to be debounced.
2. **Wait duration**: The delay (in milliseconds) between the last call and the actual invocation.

### Example Code:
```javascript
let i = 0;
function increment() {
  i++;
}
const debouncedIncrement = debounce(increment, 100);

// t = 0: Call debouncedIncrement().
debouncedIncrement(); // i = 0

// t = 50: i is still 0 because 100ms have not passed.

// t = 100: increment() was invoked and i is now 1.
```

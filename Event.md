## Event Emitter

Implement an `EventEmitter` class similar to the one in Node.js that follows the observer pattern.

### Example 

```javascript
const emitter = new EventEmitter();

function addTwoNumbers(a, b) {
  console.log(`The sum is ${a + b}`);
}

emitter.on('foo', addTwoNumbers);
emitter.emit('foo', 2, 5);
// Output: "The sum is 7"

emitter.on('foo', (a, b) => console.log(`The product is ${a * b}`));
emitter.emit('foo', 4, 5);
// Output: 
// "The sum is 9"
// "The product is 20"

emitter.off('foo', addTwoNumbers);
emitter.emit('foo', -3, 9);
// Output: "The product is -27"
```

### API

#### 1. new EventEmitter()
Creates an instance of the EventEmitter class. Events and listeners are isolated within the EventEmitter instances they're added to, 
aka listeners shouldn't react to events emitted by other EventEmitter instances.

#### 2. emitter.on(eventName, listener)
Adds a callback function (listener) that will be invoked when an event with the name eventName is emitted.

function createCounter(initialValue) {
  let counterValue = initialValue;

  function increment() {
    counterValue++;
    console.log('Incremented:', counterValue);
  }

  function decrement() {
    counterValue--;
    console.log('Decremented:', counterValue);
  }

  function getValue() {
    console.log('Current value:', counterValue);
  }

  return {
    increment,
    decrement,
    getValue
  };
}

// Create a counter with an initial value of 5
const counter = createCounter(5);

// Use the counter
counter.increment(); // Output: Incremented: 6
counter.increment(); // Output: Incremented: 7
counter.decrement(); // Output: Decremented: 6
counter.getValue();  // Output: Current value: 6

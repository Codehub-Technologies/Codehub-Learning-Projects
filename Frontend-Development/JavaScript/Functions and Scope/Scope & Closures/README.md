# Scope & Closures

### Global vs Local:
- Declare a global variable `counter = 0`. Create a function `incrementCounter` that declares a local variable `counter = 10` and increments it. What’s the `global counter` value after invocation?

### Block Scope:
- Use a for loop with let to print `numbers 1-5`. Then, try accessing the loop variable outside the loop. What happens?

### Closure:
- Create a function `createCounter` that returns a function. The returned function should `increment` and return a `counter` each time it’s called.
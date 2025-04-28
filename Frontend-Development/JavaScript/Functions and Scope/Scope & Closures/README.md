# Scope & Closures

**Instruction:**
1. Create a file `function_scope_closure.js` and complete the task below
2. Add relevant `comments` and organise your codes properly

### Global vs Local:
- Declare a global variable `counter = 0`. Create a function `incrementCounter` that declares a local variable `counter = 10` and increments it. What’s the `global counter` value after invocation?
- log a `test` on the console

### Block Scope:
- Use a for loop with let to print `numbers 1-5`. Then, try accessing the loop variable outside the loop. What happens?
- log a `test` on the console

### Closure:
- Create a function `createCounter` that returns a function. The returned function should `increment` and return a `counter` each time it’s called.
- log a `test` on the console
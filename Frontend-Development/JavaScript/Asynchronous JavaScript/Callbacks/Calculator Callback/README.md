# Exercise: Calculator with Callbacks

### Task Description:
- Create four functions: add, subtract, multiply, and divide, each taking two numbers as arguments and returning the result.
- Create a calculate function that takes three parameters: two numbers and a callback function.
- The calculate function should call the callback function with the two numbers and return the result.
- Test the calculate function with each of the four operations.

### Implementation:
- Define the operation functions:
    - add(a, b): Returns the sum of a and b.
    - subtract(a, b): Returns the difference of a and b.
    - multiply(a, b): Returns the product of a and b.
    - divide(a, b): Returns the quotient of a and b (ensure b is not zero).
- Define the calculate function:
    - calculate(a, b, operation): Calls the operation callback with a and b.
- Test the calculate function:
    - Call calculate with add, subtract, multiply, and divide as the callback functions.
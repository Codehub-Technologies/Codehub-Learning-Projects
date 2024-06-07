# Exercise: String Manipulator with Callbacks

### Task Description:
- Create four functions: `toUpperCase`, `toLowerCase`, `reverseString`, and `getStringLength`, each taking a string as an argument and returning the respective manipulated string or length.
- Create a `stringManipulator` function that takes a string and a callback function.
- The `stringManipulator` function should call the callback function with the string and return the result.
- Test the `stringManipulator` function with each of the four operations.

### Implementation:
- Define the manipulation functions:
    - `toUpperCase(str)`: Returns the string converted to uppercase.
    - `toLowerCase(str)`: Returns the string converted to lowercase.
    - `reverseString(str)`: Returns the string reversed.
    - `getStringLength(str)`: Returns the length of the string.
- Define the `stringManipulator` function:
    - `stringManipulator(str, operation)`: Calls the operation callback with str.
- Test the `stringManipulator` function:
    - Call `stringManipulator` with `toUpperCase`, `toLowerCase`, `reverseString`, and `getStringLength` as the callback functions.

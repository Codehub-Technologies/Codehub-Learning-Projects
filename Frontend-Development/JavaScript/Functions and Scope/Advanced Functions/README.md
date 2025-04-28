# Advanced Function Exercises

### Prime Checker:
Write a function `isPrime` that uses a `loop` and `conditionals` to check if a number is `prime`.

### Password Validator:
Create a function `validatePassword` that checks:
- Minimum 8 characters
- At least 1 uppercase letter
- At least 1 number
- Return true/false using regex and string methods.

### Temperature Converter:
Write a function `convertTemp` that takes a temperature and a unit ("C" or "F"). Convert between Celsius and Fahrenheit using the formula:
```
F = (C * 9/5) + 32
C = (F - 32) * 5/9
```

### Array Operations:
Create a function filterEvens that takes an array of numbers and returns a new array with only even numbers. Use a for loop and conditionals.

### Closure + Loop:
Create a function createMultiplier that takes a number n and returns a function. The returned function should multiply its input by n.

```
const double = createMultiplier(2);  
console.log(double(5)); // 10  
```

### Loop + Closure Trap:
Fix this code to print 0, 1, 2 after a 1-second delay:

```
for (var i = 0; i < 3; i++) {  
  setTimeout(() => console.log(i), 1000);  
}  
```

### Private Variable:
Use a closure to create a BankAccount function with:

- Private balance variable

- Methods deposit(amount) and getBalance()


### Memoization 
Create a memoized Fibonacci function using closure.

### Currying 
Write a curry function that converts sum(a, b, c) into sum(a)(b)(c).

### Debounce 
Implement a debounce function that delays invoking a function until after a cooldown period.
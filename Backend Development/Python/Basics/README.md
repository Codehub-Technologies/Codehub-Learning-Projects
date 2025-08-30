
**Instruction:**
1. Create a file `python_basics.py` and complete the task below
2. Add relevant `comments` and organise your codes properly



### Simple Assignments

1.  **Type Conversion and Logic:**
    * Create a variable `user_input` and set it to a string, for example, `"15"`.
    * Convert this string to an integer and store it in a new variable `number`.
    * Write an `if` statement to check if `number` is an even number. (Hint: Use the modulus operator `%`).
    * Print "The number is even" if it's even, and "The number is odd" if it's odd.

2.  **Loops:**
    * Use a `for` loop to print the numbers from 1 to 5.
    * Use a `while` loop to print the first three letters of the alphabet (`A`, `B`, `C`).

---



### Complex Assignments

1.  **Type Conversion, `for` Loops, and `if` statements:**
    * Write a program that takes a list of numbers as strings: `numbers_as_strings = ["10", "25", "50", "33"]`.
    * Create a new, empty list called `even_numbers`.
    * Loop through the `numbers_as_strings` list. Inside the loop, convert each string to an integer.
    * Use an `if` statement to check if the number is even. If it is, add it to the `even_numbers` list.
    * After the loop, print the `even_numbers` list and its sum.

2.  **Conditional Logic with Multiple Conditions and `break`:**
    * Write a program that checks a list of temperatures. `temperatures = [20, 25, 30, 35, 40]`.
    * Loop through the `temperatures` list.
    * Inside the loop, use `if` statements to print a message for each temperature:
        * If the temperature is 35 or higher, print "Warning: High temperature!" and use a `break` statement to stop the loop.
        * If the temperature is 30, print "It's a warm day."
        * For all other temperatures, print "It's a comfortable day."
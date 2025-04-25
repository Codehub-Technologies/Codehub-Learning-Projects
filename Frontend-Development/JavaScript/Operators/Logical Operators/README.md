# JavaScript Logical Operators Practice

Instructions: For each question, write code that:
- Declares `variables` as described
- Uses logical operators `(&&, ||, !)` to solve the problem
- `Log` the result to the `console`

1. Basic `AND` Operator
Declare two variables: `isMember` (boolean) and `cartTotal` (number). Check if the user is a member `AND` their cart total is at least N50.

2. `OR` Operator with Strings
Declare `paymentMethod` (string) with possible values: `"credit", "debit", or "cash"`. Check if the payment method is either "credit" `OR` "debit".

3. `NOT` Operator
Declare `isLoggedIn` (boolean). Check if the user is `NOT logged in`.

4. Combined Conditions
Declare `age` (number) and `hasLicense` (boolean). Check if the user is at least 18 `AND` has a license.

5. Short-Circuit Evaluation
Declare `username` (string) and `defaultName` (string). Use the `|| operator` to assign a value to displayName such that:
- If username is `empty`, use `defaultName`
- Otherwise, use `username`

6. Range Check with `AND`
Declare `temperature` (number). Check if the temperature `is between` 20°C and 30°C (inclusive).

7. `Truthy/Falsy` Check
Declare `userInput` (string). Check if `userInput` is either `null`, `undefined`, or an `empty string`.

8. Complex Logic
Declare `isAdmin` (boolean), `accessLevel` (number), and `isBanned` (boolean). Check if:
- The user is an admin OR has accessLevel > 3
- AND is NOT banned

9. Operator Precedence
Declare `a = true`, `b = false`, and `c = true`. Evaluate:
`(a || b) && c vs a || (b && c)`
- Log both results and explain why they differ.

10. Real-World Discount Rule
Declare:
- `isSeniorCitizen` (boolean)
- `isStudent` (boolean)
- `regularPrice` (number)

Check if a customer qualifies for a discount:
- Senior citizens `OR` students
- `AND` regular price is over N100
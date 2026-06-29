# Variables Tasks
**Instruction:**
1. Create a file `variable.js` and complete the task below
2. Add relevant `comments` and organise your codes properly

---

## Part 1: Naming & Keyword Selection (Exercises 1 - 4)

### Exercise 1: Fixing the Crash

* **Task:** The code snippet below contains syntax errors and breaks your application. Rewrite the code using valid variable naming rules and modern declaration keywords (`let` or `const`). Make sure to use proper `camelCase`.
* **Broken Code:**
```javascript
let 1st_user name = "Samuel";
var total amount! = 4500;

```


* **Goal:** Eliminate all syntax errors and log the variables to the console.

### Exercise 2: Locking Down Constants

* **Task:** Declare three variables to store the configuration settings of a web app:
1. The application's name (`"Codehub Portal"`)
2. The maximum login attempts allowed (`5`)
3. The API base URL (`"https://api.codehub.tech"`)


* **Goal:** Choose the correct keyword (`let` or `const`) based on the rule that these settings should never change while the app is running.

### Exercise 3: Tracking Changing States

* **Task:** Create an application profile tracking system. Store a user's current `onlineStatus` (set to `true`) and their `accountType` (set to `"Student"`). On the next line, simulate the user logging out and upgrading their account by updating both variables to `false` and `"Premium"`.
* **Goal:** Ensure you use the correct keyword that allows variable reassignment.

### Exercise 4: The Vague Name Refactor

* **Task:** A junior developer wrote the following code, but the variable names are too vague and poor practice. Refactor this code by giving them clear, concise, descriptive `camelCase` identifiers.
* **Bad Code:**
```javascript
let d = 30; // represents the number of days in the current month
let x = "Asaba"; // represents the user's business location city
const val = 0.075; // represents the standard value-added tax (VAT) rate

```



---

## Part 2: Working with Variables (Exercises 5 - 7)

### Exercise 5: The Value Swapper

* **Task:** Declare two variables: `walletA = 1500` and `walletB = 3000`. Without simply typing out the numbers again, write a logic script that swaps their values so that `walletA` ends up with `3000` and `walletB` ends up with `1500`.
* *Hint: You might need to create a temporary "holding box" variable to achieve this.*

### Exercise 6: Dynamic Cart Update

* **Task:** Declare a variable called `cartTotal` and initialize it with a value of `12000`. The user adds a new item worth `4500` to their cart. Update the `cartTotal` variable to reflect the new price by using its own previous value.
* **Expected Output:** Log `cartTotal` to display `16500`.

### Exercise 7: Reassignment Trap

* **Task:** Write a script where you declare a user's `birthYear` using `const`. On the next line, intentionally try to reassign it to a different year. Run the code in your console and write a single-line comment below it explaining the exact name of the error you received and why it happened.

---

## 🔴 Part 3: Real-World Scenarios (Exercises 8 - 10)

### Exercise 8: The Score Tracker

* **Task:** Create a mini-game scoring system. Declare a variable `playerScore` and set it to `0`. Simulate three game events:
1. The player defeats an enemy (add `10` points).
2. The player collects a coin (add `5` points).
3. The player takes damage (subtract `3` points).


* **Goal:** Update the `playerScore` variable sequentially after each event and print the final score.

### Exercise 9: Distance Conversion Safety

* **Task:** You are building a map feature. Create a variable to store a distance value. Following the rule *"Don't get too specific with names in case formats change,"* choose an appropriate general variable identifier. Set its initial value to `150`. Write a comment explaining why your variable name choice is cleaner than naming it `milesValue`.

### Exercise 10: Private Signal Simulation

* **Task:** Declare an internal system configuration variable meant to hold a sensitive database credentials token. Use the standard developer convention to visually signal to your engineering team that this specific variable is "private" and shouldn't be altered directly from outside the file.
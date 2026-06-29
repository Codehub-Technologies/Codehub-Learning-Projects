# JavaScript Operators Exercises


---

## 🟢 Part 1: Arithmetic Operators (Exercises 1 - 4)

### Exercise 1: The Remainder Finder

* **Task:** Create a script that takes a total number of items (e.g., `27`) and packs them into boxes that hold exactly `5` items each. Use the correct operator to find out how many leftover items cannot fit into a full box.
* **Expected Output:** `2`

### Exercise 2: Exponential Power

* **Task:** Declare a variable `base` and set it to `4`. Declare another variable `exponent` and set it to `3`. Calculate the value of `4` raised to the power of `3` using the modern exponentiation operator.
* **Expected Output:** `64`

### Exercise 3: Average Score

* **Task:** A student scored `85`, `90`, and `78` on three separate tests. Store these scores in three distinct variables, then calculate the average score. Remember to mind your operator precedence!
* **Expected Output:** `84.333...`

### Exercise 4: Dynamic Greeting (String Operator)

* **Task:** Create two variables: `firstName` and `lastName`. Use the addition operator to combine them into a single variable named `fullName`, ensuring there is a space character between them.
* **Expected Output:** `"John Doe"`

---

## 🟡 Part 2: Assignment Operators (Exercises 5 - 8)

### Exercise 5: The Bank Deposit

* **Task:** Start with a variable `balance` set to `500`. A user deposits `150`. Update the `balance` variable using the **add-and-assign** operator.
* **Expected Output:** `650`

### Exercise 6: Inventory Shrinkage

* **Task:** A store has `40` laptops in stock. They sell `7` of them. Update the stock variable using the **subtract-and-assign** operator.
* **Expected Output:** `33`

### Exercise 7: Combo Math

* **Task:** Initialize a variable `points` at `10`. Multiply it by `3`, and then add `5` to it. Perform both operations using compound assignment operators (`*=`, `+=`).
* **Expected Output:** `35`

### Exercise 8: Clear the Wallet

* **Task:** A user has a variable `cash` set to `100`. They purchase an item that costs exactly all their cash. Use an assignment operator to reduce their cash to `0` based on the item price.
* **Expected Output:** `0`

---

## 🔴 Part 3: Comparison Operators (Exercises 9 - 11)

### Exercise 9: The Type Trap

* **Task:** Compare the number `10` and the string `"10"`. Write two separate comparison statements: one using loose equality (`==`) and one using strict equality (`===`). Log both results to see the difference.
* **Expected Output:** `true` for loose, `false` for strict.

### Exercise 10: Age Gate

* **Task:** Set a variable `userAge` to `18`. Write a comparison statement that checks if the user is old enough to drive (the minimum driving age is `18`). The expression must return `true` if they are exactly 18.
* **Expected Output:** `true`

### Exercise 11: Inequality Check

* **Task:** Create a variable `currentStatus` and set it to `"processing"`. Write a strict inequality comparison (`!==`) to verify that the status is **not** equal to `"completed"`.
* **Expected Output:** `true`

---

## 🔥 Part 4: Logical & Combined Operators (Exercises 12 - 15)

### Exercise 12: Login Authentication

* **Task:** To log in, a user must have their email verified **and** have a secure token. Create two boolean variables: `isEmailVerified` (set to `true`) and `hasToken` (set to `false`). Use a logical operator to determine if they can enter the dashboard.
* **Expected Output:** `false`

### Exercise 13: Delivery Fee Waiver

* **Task:** A food delivery app waives the delivery fee if a customer spends over `$50` **or** if they are a premium member. Create variables `orderTotal = 35` and `isPremium = true`. Use a logical operator to check if they qualify for free delivery.
* **Expected Output:** `true`

### Exercise 14: Toggle State

* **Task:** Create a variable `isModalOpen` and set it to `false`. Use the logical NOT operator (`!`) to toggle this variable to its exact opposite value and reassign it.
* **Expected Output:** `true`

### Exercise 15: The Ultimate Gatekeeper

* **Task:** Write a single expression to check if a user can buy a restricted ticket. The rules are: The user must be **at least 18 years old**, AND they must either **have a VIP pass (boolean)** OR **have a coupon code (boolean)**.
* Test it with: `age = 19`, `hasVIP = false`, `hasCoupon = true`.


* **Expected Output:** `true`

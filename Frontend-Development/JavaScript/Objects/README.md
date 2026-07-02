


---

## Task 1: The "Smart Device" Catalog (Literals vs. Blueprint)

**Objective:** Practice building a single standalone object literal, and then refactoring it into a re-usable Constructor Function blueprint.

### Instructions:

1. **Create an Object Literal:** Create a standalone object named `smartTV` using curly braces `{}`. Give it the properties `brand` (string), `screenSize` (number), and `is4K` (boolean). Fill it with whatever values you like.
2. **Create a Constructor Function:** Now, imagine your store expands and you need to make hundreds of TVs. Write a constructor function named `Device(brand, screenSize, is4K)`. Inside the template, use the `this` keyword to dynamically map the incoming arguments to the object properties.
3. **Instantiate the Instances:** Use your new constructor function along with the `new` operator to create two distinct TV objects:
* `tv1`: A Samsung, 55-inch, true 4K TV.
* `tv2`: An LG, 32-inch, false (not 4K) TV.



---

## Task 2: Refactoring to Modern Class Syntax

**Objective:** Take a legacy ES5 constructor function blueprint and upgrade it to a modern ES6 Class structure.

### Instructions:

Below is a legacy ES5 constructor function used to generate profiles for a gaming application. Your job is to update this code to meet modern ECMAScript standards using **Class Syntax**.

1. Convert the `Player` constructor function into an ES6 `class` named `PlayerClass`.
2. Move the internal variable assignments inside a dedicated `constructor` block.
3. Instantiate a new player instance named `player1` passing the values `"CyberKnight"` and `85` using the `new` keyword.

### Legacy Code to Refactor:

```javascript
// Upgrade this legacy template into an ES6 Class
function Player(username, level) {
    this.username = username;
    this.level = level;
}

// Convert the instantiation below to use your new class blueprint
const player1 = new Player("CyberKnight", 85);

```


---

## Task 3: The Dynamic Inventory Manager (Bracket Notation & Updates)

**Objective:** Practice modifying object properties, adding new keys dynamically, and understanding when bracket notation is mandatory.

### Instructions:

You are building a backend inventory system for a clothing store. Start with the initial object below and write the JavaScript statements to complete these operations in order:

1. A customer just purchased a pair of jeans. Update the `quantity` property by decreasing its value from `50` down to `49`.
2. The store decided to categorize items. Add a brand new property named `category` and set its value to `"Apparel"`.
3. The store has an official dynamic promotional event running, stored in a variable: `const promoKey = "discount-percentage";`. Using **bracket notation and the variable**, add this property to the `inventoryItem` object with a value of `15`.
4. Console log your updated object to verify the changes.

### Starter Code:

```javascript
const inventoryItem = {
  id: "JNS-01",
  itemName: "Slim Fit Jeans",
  quantity: 50
};

// Write your solution below:

```

---

## Task 4: Data Cleanup (The Delete Operator)

**Objective:** Use the `delete` keyword to purge sensitive or outdated keys entirely from an object collection.

### Instructions:

Before sending user account data to the frontend browser, a security dev needs to sanitize the user object by stripping out non-essential or sensitive fields.

1. Use the `delete` keyword to completely remove the `passwordHash` property from the `userAccount` object.
2. Use the `delete` keyword to completely remove the `temporaryFlag` property.
3. Print out the object using `console.log(userAccount)`. Ensure the remaining object *only* contains the `username` and `email` properties.

### Starter Code:

```javascript
const userAccount = {
  username: "DevAlex",
  email: "alex@code.com",
  passwordHash: "a9f82b3cc110e7",
  temporaryFlag: true
};

// Write your solution below:

```

---

## Task 5: The Interactive Bank Account (Methods & Execution Context)

**Objective:** Write custom object methods that modify internal state using the `this` keyword.

### Instructions:

Complete the missing functionality inside the `bankAccount` object. You will need to write two methods that directly update the account's balance.

1. Implement the `deposit(amount)` method. It should take a number as an argument, add that number directly to the object's `balance` property using `this`, and return the updated balance.
2. Implement the `withdraw(amount)` method. It should subtract the argument amount from the internal `balance` property using `this`, and return the updated balance.
3. Test your code by running the verification script at the bottom.

### Starter Code:

```javascript
const bankAccount = {
  accountHolder: "Sarah",
  balance: 250,
  
  // 1. Write the deposit method here:
  deposit(amount) {
    // Your code here
  },
  
  // 2. Write the withdraw method here:
  withdraw(amount) {
    // Your code here
  }
};

// --- Verification Script ---
console.log(bankAccount.deposit(50));   // Expected Output: 300
console.log(bankAccount.withdraw(100)); // Expected Output: 200

```
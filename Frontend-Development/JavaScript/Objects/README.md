


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

---

## Task 6: The "Profile Card" Debugging Challenge (Arrow vs. Inner Functions)

**Objective:** Spot and fix context runtime bugs caused by the improper layout of arrow functions and standard inner functions inside object definitions.

### Instructions:

A developer wrote the following profile application widget, but it is currently broken. When `profile.displayDetails()` is executed, it prints unexpected values to the console.

Copy the code below into your editor and fix the following bugs without changing the text strings:

1. The `displayDetails` method is defined as an **arrow function**, causing it to lose access to the local `name` property. Convert it into a **standard shorthand method**.
2. The nested `renderTag` function inside `displayTags` loses its `this` binding completely, crashing the script. Fix it by converting `renderTag` into an **arrow function** so that it lexically inherits the correct object instance scope from its parent method.

### Starter Code:

```javascript
const profile = {
  name: "Alex",
  tags: ["Developer", "Mentor"],
  
  // Bug 1: Fix this method's function type definition
  displayDetails: () => {
    console.log(`User Profile Name: ${this.name}`);
  },
  
  displayTags() {
    // Bug 2: Convert this inner function to fix the context binding trap
    function renderTag(tag) {
      console.log(`${this.name} is tagged as: ${tag}`);
    }
    
    this.tags.forEach(renderTag);
  }
};

// --- Test Execution ---
profile.displayDetails(); // Should log: "User Profile Name: Alex"
profile.displayTags();    // Should log: "Alex is tagged as: Developer", etc.

```

---

## Task 7: The Shared Device Engine (Explicit Context Hijacking)

**Objective:** Use `.call()` to explicitly override execution contexts and run a single unattached function across completely unique data structures.

### Instructions:

Instead of rewriting the exact same logic inside dozens of different objects, software engineers keep code dry by writing decoupled standalone functions and applying them explicitly when needed.

1. Write a standalone global function named `processOrder()`.
2. Inside `processOrder`, use the `this` keyword to calculate a new total value based on the formula:

$$\text{Total} = \text{this.basePrice} - \text{this.discount}$$


3. Have `processOrder` log a final summary string format exactly like this:
`"Order item processed. Final Total: $X"`
4. Using the `.call()` method, invoke your standalone function twice:
* First, run it explicitly binding `this` to the `order1` configuration object.
* Second, run it explicitly binding `this` to the `order2` configuration object.



### Starter Code:

```javascript
const order1 = {
  itemId: "B100",
  basePrice: 50,
  discount: 10
};

const order2 = {
  itemId: "C250",
  basePrice: 120,
  discount: 30
};

// 1. Write your standalone processOrder function here

// 4. Invoke the function explicitly using .call() on both orders below:

```

---

## Task 8: The "Classroom Average" Report (Iteration & Utilities)

**Objective:** Extract keys, values, and loop through an object to compute calculations based on structural elements.

### Instructions:

You have received a raw data report of a student's final grades. Write JavaScript code using the provided `studentGrades` object to calculate and output critical report details:

1. Use `Object.keys()` to extract a clean list of all subjects the student took. Log this array to the console.
2. Use `Object.values()` to extract a clean list of all scores the student received. Log this array to the console.
3. Using a `for...in` loop, iterate over the `studentGrades` object to compute the sum of all values, then calculate the average score. Log the final average to the console (Hint: Sum all grades up inside the loop and divide by total number of keys).

### Starter Code:

```javascript
const studentGrades = {
  history: 88,
  literature: 92,
  physics: 78,
  chemistry: 84
};

// Write your extraction and calculation logic below:

```

---

## Task 9: Preventing the "Reference Overwrite" (Object Cloning)

**Objective:** Understand how objects behave in memory when copied by reference, and fix accidental mutations using the spread operator.

### Instructions:

A junior developer attempted to build a "dark mode" settings feature for a web app. However, because they copied the object profile by reference, changing the dark mode configuration accidentally overwrote the user's primary system default profile template!

1. Look closely at the `// BUG LOCATION` line in the starter code. Fix it by using the **Spread Operator (`...`)** to make an actual independent clone instead of a shared memory link.
2. Verify that after running your fix, `defaultSettings.theme` safely stays `"light"`, while `userSettings.theme` changes to `"dark"`.

### Starter Code:

```javascript
const defaultSettings = {
  theme: "light",
  notifications: true,
  fontSize: "medium"
};

// BUG LOCATION: This line creates a shared reference link instead of a safe clone!
const userSettings = defaultSettings; 

// Mutating the new config profile
userSettings.theme = "dark";

// --- Verification Script ---
console.log(`Original Base Theme: ${defaultSettings.theme}`); // Target: "light"
console.log(`User Custom Theme: ${userSettings.theme}`);       // Target: "dark"

```

---

## Task 10: Cleaner Data Extraction (Destructuring Challenge)

**Objective:** Cleanly unpack specific values directly out of deeply nested objects into distinct variables in a single line of code.

### Instructions:

When working with third-party server responses or APIs, you'll often get heavy, deeply nested structures. Instead of writing long lines of code like `const title = response.payload.title;`, we can unpack it elegantly.

1. Use **Object Destructuring** syntax to extract the `title`, `price`, and `stock` properties directly out of the `product` object into three standalone local variables.
2. Log out the matching values using a template literal statement:
`"The item X costs $Y. Stock count: Z"`

### Starter Code:

```javascript
const product = {
  id: "PROD-902",
  title: "Wireless Mechanical Keyboard",
  price: 125,
  stock: 14,
  warehouseId: "WH-East"
};

// 1. Unpack properties using Destructuring on a single line below:


// 2. Add your console.log statement here:

```

Here are two practical exercise tasks designed to help students master the structural differences between JSON and JavaScript objects, as well as serialization workflows using `JSON.parse()` and `JSON.stringify()`.

---

## Task 11: The "Syntax Inspector" (Validating & Parsing Server Data)

**Objective:** Learn to spot syntax differences between standard JavaScript objects and raw JSON strings, and parse valid strings into operational objects.

### Instructions:

Imagine your web application just pulled a string of raw profile configurations from a network database server. However, before you can manipulate it, you need to fix a few critical formatting syntax bugs to ensure it fits the strict JSON specification rules.

1. Inspect the raw text assigned to `rawServerResponse` in the starter code. It contains **three formatting bugs** that prevent it from being valid JSON data. Fix these errors:
* JSON keys must be explicitly wrapped inside double quotes (`""`). Fix the bare keys.
* JSON string values must use strict double quotes (`""`), not single quotes (`''`). Fix the single-quoted string value.
* Trailing commas at the very end of an object layout are strictly illegal in JSON syntax. Remove the trailing comma.


2. Once the string syntax is verified and valid, use **`JSON.parse()`** to deserialize it into a operational JavaScript object literal assigned to a variable named `cleanProfile`.
3. Verify your work by running `console.log(cleanProfile.username);`.

### Starter Code:

```javascript
// BUG HUNT: Fix the syntax errors inside this string block to make it valid JSON!
const rawServerResponse = '{ username: "CodePro", status: \'Active\', credits: 450, }';

// 2. Parse the corrected string into an object below:


// 3. Test access
// console.log(cleanProfile.username); // Expected Output: "CodePro"

```

---

## Task 12: Shipping local data away (The `JSON.stringify()` serialization)

**Objective:** Safely package a local live dataset structure into a serialized transport string ready for web API payloads or storage.

### Instructions:

You are developing a feature to save a user's running shopping cart state before they close their browser tab. You have the data structured nicely as a local JavaScript Array filled with individual item objects.

1. Create a variable named `jsonPayload`.
2. Use the **`JSON.stringify()`** method to serialize the `shoppingCart` data array into a flattened transport string format.
3. Test the datatype of your resulting transformation by executing a `typeof` inspection statement:
`console.log(typeof jsonPayload);`
4. Confirm that the final logged execution prints `"string"` out to the debugger panel rather than an array or object structure.

### Starter Code:

```javascript
const shoppingCart = [
  { item: "Wireless Mouse", price: 25, qty: 1 },
  { item: "HDMI Cable", price: 12, qty: 2 },
  { item: "Sticker Pack", price: 5, qty: 3 }
];

// 1 & 2. Convert the array data layout to a JSON string format below:


// 3. Run a type check verification below:

```
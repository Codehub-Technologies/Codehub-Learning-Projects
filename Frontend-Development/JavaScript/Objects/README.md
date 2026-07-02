


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
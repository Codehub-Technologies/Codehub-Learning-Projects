# Python Object Oriented Programming

**Instruction:**
1. Create a file `python_oop.py` and complete the task below
2. Add relevant `comments` and organise your codes properly
3. These tasks cover all OOP pillars — Class, Object, Encapsulation, Inheritance, Polymorphism, Abstraction, Composition, and Magic Methods.


### **1. Class & Object Design**

Create a class `BankAccount` with:

* Attributes: `account_number`, `owner_name`, and `balance` (default `0.0`)
* Methods:

  * `deposit(amount)`
  * `withdraw(amount)`
  * `get_balance()`

* Create **three objects** from this class and perform deposits and withdrawals.
* Allow the user to enter input from the terminal
* Prevent withdrawals that would make the balance negative (show an error message instead).



### **2. Encapsulation & Property Decorators**

Modify the `BankAccount` class:

* Make `balance` **private** (`__balance`).
* Use the `@property` decorator to safely access it. (Advance)
* Add a setter for `balance` that prevents direct modification (except via deposit/withdraw) (Advance).
* Demonstrate what happens if someone tries to set the balance directly.


### **3. Inheritance**

Create a subclass called `SavingsAccount` that inherits from `BankAccount`:

* Add an attribute `interest_rate`.
* Add a method `apply_interest()` that increases the balance based on the interest rate.
* Create both `BankAccount` and `SavingsAccount` objects and demonstrate how they differ in behavior.



### **4. Polymorphism**

Create a base class `Employee` with:

* A method `calculate_pay()` (to be overridden).

Then create two subclasses:

* `FullTimeEmployee` with a fixed monthly salary.
* `PartTimeEmployee` paid hourly.
* Write a function `show_employee_pay(employee_list)` that loops through employees and calls `calculate_pay()` on each, demonstrating **runtime polymorphism**.


### **5. Abstraction**

Use the `abc` module:

* Create an abstract class `Vehicle` with abstract methods `start_engine()` and `stop_engine()`.
* Create subclasses `Car` and `Motorbike` that implement those methods differently.
* Try to instantiate `Vehicle` directly — what happens?


### **6. Composition**

* Create a class `Battery` with attributes like `capacity` and a method `get_status()`.
* Then create an `ElectricCar` class that **uses composition** — it has a `Battery` object as one of its attributes.
* Demonstrate how the `ElectricCar` delegates battery-related actions to its `Battery` object.


### **7. Dunder (Magic) Methods**

Enhance the `BankAccount` class by adding:

* `__str__` → returns a readable string representation.
* `__eq__` → compares two accounts by account number.
* `__add__` → combines two accounts’ balances and returns a new account.
* Show examples of how these methods make your objects behave like built-in types.
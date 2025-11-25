# Python List Exercise

**Instruction:**
1. Create a file `python_list.py` and complete the task below
2. Add relevant `comments` and organise your codes properly

## **Exercise 1: Deeper List Access & Validation**

Given:

```python
my_list = [10, 20, 30, 40, 50]
```

Perform:

1. Print the *third element from the end* using **negative indexing**.
2. Check if the list length is a **multiple of 5**.
3. Write an expression to check if the list is empty.

**Expected Output Example**

```
Third from end: 30
Length is a multiple of 5: True
List is not empty
```



## **Exercise 2: Advanced List Manipulation**

Given:

```python
my_list = [10, 20, 30, 40, 50]
```

Perform:
1. Replace the *second and third* items with `200` and `300` in a **single assignment**.
2. Append **two values at once** (5000 and 6000) without using two append calls.
3. Insert value `999` *at the middle of the list* (calculate the index programmatically).
4. Remove **all elements greater than 500**.
5. Remove the last element **without using pop()**.


## **Exercise 3: Compute Sum, Average & Standard Deviation**

Given:

```python
my_list = [10, 20, 30, 40, 50]
```

Compute:
1. Total sum
2. Average


## **Exercise 4: Reverse Without Built-in Tools**

Reverse:

```python
list1 = [100, 200, 300, 400, 500]
```

But **you MAY NOT use**:
* `reverse()`
* slicing (`[::-1]`)
* `reversed()`

*Hint:* Use swapping or two-pointer technique.



## **Exercise 5: Transform List Into Squares — With Constraints**

Given:

```python
numbers = [1, 2, 3, 4, 5, 6, 7]
```

Create a new list where:
* odd numbers → square them
* even numbers → **cube** them

Expected Output:

```
[1, 8, 9, 64, 25, 216, 49]
```


## **Exercise 6: Find Max, Min, and Second Max**

Without using:

* `max()`
* `min()`
* `sorted()`

Given:

```python
data = [8, 2, 15, 1, 9]
```

Find:

* largest
* smallest
* **second-largest**


## **Exercise 7: Count Occurrences + Case-Insensitive Matching**

Given:

```python
sports = ['Cricket', 'Football', 'Hockey', 'football', 'Tennis']
```

Count how many times `"football"` appears **ignoring case**.



## **Exercise 8: Sort Manually (No Built-ins)**

Given:

```python
numbers = [5, 2, 8, 1, 9]
```

Sort the list **using your own bubble-sort or selection-sort implementation**.



## **Exercise 9: Deep Copy vs Shallow Copy**

Given:

```python
original = [10, 20, [30, 40]]
```

1. Create a **shallow copy** and modify the nested list.
2. Create a **deep copy manually (no `copy` module`)**.
3. Show the difference in output.



## **Exercise 10: Combine Lists — With Zip Logic**

Combine:

```python
list_a = [1, 2, 3]
list_b = [10, 20, 30]
```

But the output should be:

```
[(1, 10), (2, 20), (3, 30)]
```



## **Exercise 11: Remove Empty Strings + Strings with Only Spaces**

Given:

```python
list1 = ["Mike", "", "Emma", "   ", "Kelly", "", "Brad"]
```

Remove:
* empty strings
* strings that contain *only whitespace*


## **Exercise 12: Remove Duplicates While Preserving Order**

Given:

```python
list_with_duplicates = [1, 2, 2, 3, 1, 4, 5, 4]
```

Expected Output:

```
[1, 2, 3, 4, 5]
```

*Constraint:*
**Do not use `set()`**.


## **Exercise 13: Remove All Occurrences — Without Using `remove()`**

Given:

```python
list1 = [5, 20, 15, 20, 25, 50, 20]
```

Remove all occurrences of 20 using:

* list comprehension OR
* manual iteration with indexes



## **Exercise 14: Extract Only Integers — But Keep Their Order**

Given:

```python
my_list = [1, 2, 3, 'Jessa', 4, 5, 'Kelly', 'Jhon', 6]
```

Output only integers using a comprehension *and* verify the type.



## **Exercise 15: Access Deeply Nested Elements**

Given:

```python
nested_list = [[10, 20, 30], [44, 55, 66], [77, 87, 99]]
```

Print:

* First element of the last list
* Middle element (55)
* Last element of the first list



## **Exercise 16: Flatten Nested List of Unknown Depth**

Given:

```python
list_of_lists = [[1, 2], [3, 4, [5, 6]], 7]
```

Expected Output:

```
[1, 2, 3, 4, 5, 6, 7]
```

*Constraint:*
Must work for **any depth**, not only 1 or 2.



## **Exercise 17: Index-Wise Concatenation — With Unequal Lengths**

Given:

```python
list1 = ["M", "na", "i", "Ke", "extra"]
list2 = ["y", "me", "s", "lly"]
```

Expected Output:

```
['My', 'name', 'is', 'Kelly', 'extra']
```



## **Exercise 18: Cartesian Concatenation — But Exclude Identical Pairs**

Given:

```python
list1 = ["A", "B", "C"]
list2 = ["A", "B", "C"]
```

Produce:

```
['AA', 'AB', 'AC', 'BA', 'BB', 'BC', 'CA', 'CB', 'CC']
```

But **remove cases where both letters are equal**:

```
['AB', 'AC', 'BA', 'BC', 'CA', 'CB']
```



## **Exercise 19: Pair Lists — Without Using `zip()`**

Given:

```python
list1 = [10, 20, 30, 40]
list2 = [100, 200, 300, 400]
```

Print:

```
10 400
20 300
30 200
40 100
```


## **Exercise 20: Insert After a Value (Nested)**

Given:

```python
list1 = [10, 20, [300, 400, [5000, 6000], 500], 30, 40]
```

Insert `7000` after `6000` **regardless of nesting depth**.



## **Exercise 21: Extend Deepest Nested List Dynamically**

Given:

```python
list1 = ["a", "b", ["c", ["d", "e", ["f", "g"], "k"], "l"], "m", "n"]
sub_list = ["h", "i", "j"]
```

Append the sublist into the **deepest nested list** (the one containing `["f", "g"]`).



## **Exercise 22: Replace First Occurrence of a Value — In a Nested Structure**

Given:

```python
list1 = [5, 10, [15, 20, 25], 20, 50]
```

Replace only the **first** `20` with `200`.
Should work whether the value appears at top level or inside nested lists.
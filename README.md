Sure! Here's the full README text that you can copy and paste:

---

# inventory\_Carmen.py

## Overview

This script is developed for Laboratory Exercise 1 of the IT2409 course. It demonstrates how Python handles mutable and immutable data types through two functions:

1. `add_to_stock(stock_list)`
2. `update_price(price)`

Each function is tested with appropriate data to illustrate Python’s behavior with lists (mutable) and floats (immutable).

---

## Files

* `inventory_Surname.py`: Python script containing the implementation of the two required functions.

---

## Instructions and Functionality

### 1. Function: `add_to_stock(stock_list)`

**Purpose**:
Simulates updating inventory by appending a new quantity (75) to the existing stock list.

**Behavior**:

* Accepts a list as input.
* Adds `75` using `append()` method.
* Prints the updated list inside the function.

**Test Case**:

```python
inventory = [100, 200, 150]
add_to_stock(inventory)
print("Outside function (stock):", inventory)
```

**Expected Output**:

```
Inside function (stock): [100, 200, 150, 75]
Outside function (stock): [100, 200, 150, 75]
```

**Explanation**:
Lists are mutable, so changes inside the function persist outside it.

---

### 2. Function: `update_price(price)`

**Purpose**:
Calculates a 10% markup on the price without modifying the original value, simulating pass-by-value.

**Behavior**:

* Accepts a float as input.
* Computes a new price: `price + (price * 0.10)`
* Prints the computed price inside the function.

**Test Case**:

```python
base_price = 250.0
update_price(base_price)
print("Outside function (price):", base_price)
```

**Expected Output**:

```
Inside function (price): 275.0
Outside function (price): 250.0
```

**Explanation**:
Floats are immutable; changes made inside the function do not affect the original variable.

---


# 🧠 Gen AI Task 3: Functions, Lambda, Map & Filter

## 📌 Overview

This notebook contains solutions for **Task 3** of the Gen AI course, focusing on Python fundamentals such as:

* User-defined functions
* Default arguments
* Recursion
* Lambda functions
* Map and Filter
* Practical mini problem implementation

---

## 🎯 Tasks Implemented

### ✅ Task 1: Discount Calculation Function

* Created a function `apply_discount()`
* Used **default argument (5%)**
* Calculates final price after discount

```python
def apply_discount(price, discount_percent=5):
    final_price = price - ((discount_percent/100) * price)
    return final_price
```

---

### ✅ Task 2: Factorial Using Recursion

* Implemented recursive function `factorial()`
* Handled negative input
* Used base condition (`0` and `1`)

```python
def factorial(n):
    if n < 0:
        print("its a -ve number")
        return
    elif n == 0 or n == 1:
        return 1
    return n * factorial(n-1)
```

---

### ✅ Task 3: Lambda Function

* Used lambda to calculate GST
* Demonstrates **anonymous function usage**

```python
gst = lambda price: price + (0.8 * price)
```

---

### ✅ Task 4: Map Function

* Applied `map()` with lambda
* Transformed list of prices by adding GST

```python
list(map(lambda p: p + (0.8 * p), prices))
```

---

### ✅ Task 5: Filter Function

* Used `filter()` to select values
* Extracted prices based on condition

```python
list(filter(lambda p: p > 500, prices))
```

---

### ✅ Task 6: Map + Filter Combined

* Combined both functions
* Applied transformation + filtering

```python
discounted_prices = list(map(lambda p: p + (p * 0.10), prices))
filtered = list(filter(lambda p: p > 300, discounted_prices))
```

---

## 🧪 Mini Project: Price Management System

### 📊 Features:

* Add price to list
* Calculate average price
* Find maximum price
* Handle empty list

### 💡 Functions Used:

* `add_price()` → adds price
* `avg_price()` → calculates average
* `max_price()` → finds max value

---

## 🧠 Key Learnings

* How to write reusable functions
* Importance of base condition in recursion
* Difference between `def` and `lambda`
* Practical use of `map()` and `filter()`
* Handling edge cases like empty lists

---

## ▶️ How to Run

1. Open the notebook
2. Run all cells sequentially
3. Test functions with different inputs

---

## 🚀 Future Improvements

* Add input validation
* Improve UI with menu system
* Store data in file
* Convert to web app

---

## 👨‍💻 Author

**Ruthvik Sukhavasi**

---

## ⭐ Note

This task is part of my **Gen AI learning journey**, focusing on building strong Python fundamentals required for data science and real-world problem solving.

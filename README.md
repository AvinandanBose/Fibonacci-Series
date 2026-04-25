# Fibonacci Series (Recursive Approach)

## 📌 Overview

This repository demonstrates the implementation of the **Fibonacci Series using recursion**.
The Fibonacci sequence is one of the most fundamental concepts in computer science and mathematics, widely used for understanding **recursion, time complexity, and algorithm design**.

---

## 🔢 What is Fibonacci Series?

The Fibonacci series is a sequence where each number is the sum of the two preceding numbers.

[
F(n) = F(n-1) + F(n-2)
]

### Example Sequence:

```
0, 1, 1, 2, 3, 5, 8, 13, 21, ...
```

---

## 💻 Implementation (Recursive)

```cpp
int fibonacci(int n)
{
    if (n == 0 || n == 1)
        return n;

    return fibonacci(n - 1) + fibonacci(n - 2);
}
```

---

## 🚀 How It Works

* Uses **recursion** to break the problem into smaller subproblems
* Each function call computes:

  * `fibonacci(n-1)`
  * `fibonacci(n-2)`
* Combines results to get the final answer

---

## ⏱️ Time Complexity

[
T(n) = T(n-1) + T(n-2) + O(1)
]

* **Time Complexity:**
  👉 Θ(φⁿ) ≈ O(2ⁿ)

* This exponential growth occurs due to repeated calculations.

---

## 📦 Space Complexity

* **Auxiliary Space:** Θ(n)
* Due to recursion stack depth

---

## ⚠️ Limitations

* Inefficient for large `n`
* Recomputes the same values multiple times
* Leads to exponential time complexity

---

## 🔄 Optimized Alternatives

To improve performance, consider:

### 1. Memoization (Top-Down)

* Stores computed values
* Time: O(n)

### 2. Tabulation (Bottom-Up)

* Iterative approach
* Space optimized

### 3. Matrix Exponentiation

* Time: O(log n)

---

## 📚 Learning Outcomes

This project helps in understanding:

* Recursion and call stack behavior
* Recurrence relations
* Time vs Space complexity
* Difference between **growth rate and actual output**

---



## 📊 Complexity Analysis

### Space Complexity: `O(n)`
- **Input Space:** `O(1)` for primitive integer variables (like `n` and `i`).
- **Auxiliary Space:** `O(n)`. This is governed by the Call Stack. The longest path in the recursion tree goes from `n` down to `1`, meaning there will be at most `n` activation records on the stack at any given time.
- **Total Space Complexity:** `O(n)`

### Time Complexity: `O(1.618^n)` 
The recurrence relation for this recursive algorithm is:
$$T(n) = T(n-1) + T(n-2) + O(1)$$

Using the **characteristic equation method** ($x^2 - x - 1 = 0$), the roots are:
- $x_1 = \\frac{1 + \\sqrt{5}}{2} \\approx 1.618$ (The Golden Ratio)
- $x_2 = \\frac{1 - \\sqrt{5}}{2} \\approx -0.618$

Solving for the coefficients using the base cases $T(0) = 1$ and $T(1) = 1$ gives the exact non-asymptotic time complexity equation:
$$T(n) = \\left(\\frac{1 + \\sqrt{5}}{\\sqrt{5}}\\right)\\left(\\frac{1 + \\sqrt{5}}{2}\\right)^n + \\left(\\frac{\\sqrt{5} - 1}{\\sqrt{5}}\\right)\\left(\\frac{1 - \\sqrt{5}}{2}\\right)^n - 1$$

Dropping the lower-order terms and coefficients yields the tight upper bound:
**Big O Notation:** `O(1.618ⁿ)` (Often generalized as `O(2ⁿ)`)

## 🛠️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/AvinandanBose/Fibonacci-Series.git
```

2. Compile:

```bash
g++ filename.cpp -o fib
```

3. Run:

```bash
./fib
```

---

   ## 🤝 Contributing

Contributions are welcome!

* Fork the repository
* Create a new branch
* Submit a pull request

---

## 📜 License

This project is open-source and available under the MIT License.

---


## 👨‍💻 Author

**Avinandan Bose**
- GitHub: [@AvinandanBose](https://github.com/AvinandanBose)

---



## ⭐ Support

If you found this useful, consider giving it a ⭐ on GitHub!

---


<br>
<br>
<br>

<h2></h2>
<h2> 👉 <a href="https://github.com/AvinandanBose/CPLUSPLUS_DataStructure"> 𝑪++ 𝑷𝒓𝒐𝒈𝒓𝒂𝒎  𝒐𝒏 𝑭𝒊𝒃𝒐𝒏𝒂𝒄𝒄𝒊 𝑺𝒆𝒓𝒊𝒆𝒔  </h2>






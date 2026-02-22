# Lesson 1.6 – NumPy for Beginners (Agenda)

Total Duration: 3 hours  
Environment: Google Colab or VS Code Jupyter

---

## Welcome & Outcomes

- Introduce the session and goals:
  - Understand what NumPy is and why it matters
  - Create and inspect basic arrays
  - See how NumPy compares to Python lists on performance
  - Learn about array indexing, slicing, and broadcasting
  - Apply universal functions and perform linear algebra operations

---

## Part 1: Performance Benchmark

Notebook: **"Part 1: Performance Benchmark"** section and code cell.

- Walk through:
  - `import numpy as np`
  - Creating a 1,000,000‑element NumPy array and Python list
  - `%timeit` comparison: NumPy vectorized multiply vs list comprehension
- Quick learner activity:
  - Learners run the timing cell and briefly describe what they observe

---

## Part 2: The ndarray (N-dimensional array)

Notebook: **"Part 2: The ndarray"** section.

- Demonstrate:
  - Creating arrays from Python sequences
  - Array attributes: `shape`, `dtype`, `ndim`
  - Data types and casting using `astype`
- **[EXERCISE 1: Creation & Casting]**
  - Create a 3x4 array of all ones using `np.ones()`
  - Cast this array to `float32`
  - Create an array of strings representing numbers and cast to `float`

---

## Part 3: Arithmetic & Broadcasting

Notebook: **"Part 3: Arithmetic & Broadcasting"** section.

- Demonstrate:
  - Element-wise arithmetic operations (addition, multiplication, etc.)
  - Broadcasting: how scalars and arrays of different shapes work together
  - Examples: `arr * arr`, `1 / arr`
- Discussion:
  - How broadcasting makes code cleaner and more efficient

---

## Part 4: Indexing and Slicing

Notebook: **"Part 4: Indexing and Slicing"** section.

- Demonstrate:
  - 1D array indexing (similar to Python lists)
  - 2D array indexing with `[row, col]` syntax
  - Array slices are views (not copies)
  - Modifying a slice affects the original array
- **[EXERCISE 3: Complex Filtering]**
  - Select all scores where the name is NOT 'Bob'
  - Select scores for 'Bob' or 'Will' using the `|` operator
  - Find all scores less than 80 and set them to 0

---

## Part 6: Universal Functions (ufuncs) and Methods

Notebook: **"Part 6: Universal Functions (ufuncs) and Methods"** section.

- Demonstrate:
  - Unary ufuncs: `sqrt`, `exp`
  - Binary ufuncs: `add`, `maximum`
  - Statistical methods: `mean`, `sum`, `std`
  - Computing statistics along axes (axis=0, axis=1)
- Discussion:
  - When to use ufuncs vs loops for performance

---

## Part 7: Linear Algebra

Notebook: **"Part 7: Linear Algebra"** section.

- Demonstrate:
  - Element-wise multiplication with `*` vs matrix multiplication
  - Matrix multiplication with `.dot()` or `@` operator
  - Example: multiplying two matrices
- **[EXERCISE 4: Reshaping & Statistics]**
  - Create an array of 15 integers using `arange(15)` and reshape it to `(3, 5)`
  - Calculate the average value of each row
  - Use `np.unique()` to find distinct elements
  - Transpose the reshaped array using `.T` and check the new shape

---

## Wrap-up & Next Steps

- Review key takeaways:
  - NumPy's performance advantages
  - Creating and manipulating ndarrays
  - Broadcasting and vectorization
  - Linear algebra basics
- Preview next lesson topics
- Q&A

# Computational Theory Tasks

This repository contains solutions for a series of tasks related to computational theory. Each task focuses on different topics such as binary representations, hash functions, SHA256 padding, prime numbers, fractional roots, proof-of-work for SHA256, Turing machines, and computational complexity using bubble sort. Each solution is provided in a Jupyter Notebook with both Markdown cells (for explanations) and Code cells (for implementations and tests).

---

## Task Overview

### Task 1: Binary Representations
- **Objective:**  
  Implement functions to perform bit rotations (`rotl`, `rotr`), bit selection (`ch`), and majority voting (`maj`) on 32-bit unsigned integers.
- **Details:**  
  - `rotl(x, n=1)`: Left rotation of bits.
  - `rotr(x, n=1)`: Right rotation of bits.
  - `ch(x, y, z)`: Chooses bits from two numbers based on a mask.
  - `maj(x, y, z)`: Computes the bitwise majority across three numbers.
- **Research Sources:**  
  - FIPS 180-4, Secure Hash Standard (SHS): [NIST FIPS 180-4](http://dx.doi.org/10.6028/NIST.FIPS.180-4)
  - W3Schools Python Tutorial: [W3Schools Python](https://www.w3schools.com/python/)

### Task 2: Hash Functions
- **Objective:**  
  Convert a C hash function (from *The C Programming Language* by Kernighan and Ritchie) to Python.
- **Details:**  
  - Original C code provided.
  - Implement as `custom_hash` in Python.
  - Explain the choice of constants 31 and 101.
- **Research Sources:**  
  - *The C Programming Language* by Kernighan and Ritchie.
  - W3Schools: [W3Schools Python Tutorial](https://www.w3schools.com/python/)

### Task 3: SHA256 Padding
- **Objective:**  
  Write a Python function that computes the SHA256 padding for a file.
- **Details:**  
  - Read file content.
  - Append a `1` bit (as `0x80`), then enough `0` bits, and finally the original length as a 64-bit big-endian integer.
  - Print the padding in hexadecimal.
- **Research Sources:**  
  - FIPS 180-4, Secure Hash Standard (padding section): [NIST FIPS 180-4](http://dx.doi.org/10.6028/NIST.FIPS.180-4)
  - W3Schools: [Python Tutorial](https://www.w3schools.com/python/)

### Task 4: Prime Numbers
- **Objective:**  
  Calculate the first 100 prime numbers using two different algorithms.
- **Details:**  
  - **Trial Division:** Check each candidate for factors up to its square root.
  - **Sieve of Eratosthenes:** Efficiently generate primes with a dynamic upper bound.
- **Research Sources:**  
  - GeeksforGeeks: [Prime Numbers](https://www.geeksforgeeks.org/prime-numbers/) and [Sieve of Eratosthenes](https://www.geeksforgeeks.org/sieve-of-eratosthenes/)
  - W3Schools: [Python Tutorial](https://www.w3schools.com/python/)

### Task 5: Roots
- **Objective:**  
  Compute the first 32 bits of the fractional part of the square roots of the first 100 prime numbers.
- **Details:**  
  - For each prime, compute `sqrt(p)`.
  - Extract the fractional part, multiply by 2^32, and convert to an 8-digit hexadecimal value.
- **Research Sources:**  
  - GeeksforGeeks: [Prime Numbers](https://www.geeksforgeeks.org/prime-numbers/)
  - W3Schools: [Python Tutorial](https://www.w3schools.com/python/)

### Task 6: Proof of Work (SHA256 Leading Zero Bits)
- **Objective:**  
  Find the English word(s) whose SHA256 hash has the maximum number of consecutive 0 bits at the beginning.
- **Details:**  
  - Load a dictionary from `dolph_dictionary.txt`.
  - Compute SHA256 for each word and count the leading zero bits.
  - Provide proof of dictionary membership.
- **Research Sources:**  
  - W3Schools: [Python Tutorial](https://www.w3schools.com/python/)
  - Tutorialspoint: [SHA256 Basics](https://www.tutorialspoint.com/cryptography/sha256.htm)

### Task 7: Turing Machines
- **Objective:**  
  Design a Turing Machine that adds 1 to a binary number on its tape.
- **Details:**  
  - The machine starts at the left-most non-blank symbol.
  - The right-most symbol is the least significant bit.
  - Example: Transform tape `100111` to `101000`.
- **Research Sources:**  
  - Tutorialspoint: [Turing Machine](https://www.tutorialspoint.com/theory_of_computation/theory_of_computation_turing_machines.htm)
  - W3Schools: [Python Tutorial](https://www.w3schools.com/python/)

### Task 8: Computational Complexity (Bubble Sort Comparisons)
- **Objective:**  
  Implement bubble sort in Python, modified to count the number of comparisons, and use it to sort all permutations of the list `[1, 2, 3, 4, 5]`.
- **Details:**  
  - For each permutation, print the permutation and the number of comparisons.
- **Research Sources:**  
  - W3Schools: [Sorting Algorithms](https://www.w3schools.com/howto/howto_js_sort_array.asp)
  - GeeksforGeeks: [Bubble Sort](https://www.geeksforgeeks.org/bubble-sort/)
  - W3Schools: [Python Tutorial](https://www.w3schools.com/python/)

---

## How to Use This Repository

1. **Notebook Structure:**  
   Each task is implemented in a Jupyter Notebook with Markdown cells (for explanations) and Code cells (for implementations and tests).
2. **Version Control:**  
   Commits should reflect incremental development and include clear documentation for each task.
3. **Execution:**  
   Run the notebook cells sequentially to test and verify the solutions for each task.
4. **References:**  
   Research sources are provided above for further reading and to understand the background of each task.

---

## References

- **FIPS 180-4, Secure Hash Standard (SHS):**  
  [NIST FIPS 180-4](http://dx.doi.org/10.6028/NIST.FIPS.180-4)
- **The C Programming Language** by Brian Kernighan and Dennis Ritchie.
- **W3Schools:**  
  - [Python Tutorial](https://www.w3schools.com/python/)  
  - [Sorting Algorithms](https://www.w3schools.com/howto/howto_js_sort_array.asp)
- **Tutorialspoint:**  
  - [Turing Machines](https://www.tutorialspoint.com/theory_of_computation/theory_of_computation_turing_machines.htm)
  - [SHA256 Basics](https://www.tutorialspoint.com/cryptography/sha256.htm)
- **GeeksforGeeks:**  
  - [Prime Numbers](https://www.geeksforgeeks.org/prime-numbers/)  
  - [Sieve of Eratosthenes](https://www.geeksforgeeks.org/sieve-of-eratosthenes/)  
  - [Bubble Sort](https://www.geeksforgeeks.org/bubble-sort/)

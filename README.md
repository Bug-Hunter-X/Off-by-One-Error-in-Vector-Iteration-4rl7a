# Off-by-One Error in Vector Iteration

This repository demonstrates a common off-by-one error when iterating over a `std::vector` in C++.  The error arises from attempting to access an element at the index equal to the vector's size, which is one element beyond the last valid index.

## Bug Description
The code iterates through a vector using a `for` loop, but the loop condition `i <= vec.size()` is incorrect. The correct condition should be `i < vec.size()`, as vector indices are zero-based.

## Bug Solution
The solution corrects the loop condition to `i < vec.size()` ensuring that only valid indices are accessed.
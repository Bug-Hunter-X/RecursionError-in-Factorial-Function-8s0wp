# RecursionError in Python Factorial Function

This repository demonstrates a common error in recursive functions: the lack of base case handling for invalid input, leading to a RecursionError.  The `bug.py` file contains the faulty implementation, and `bugSolution.py` provides a corrected version.

## The Problem

The `factorial` function in `bug.py` correctly calculates the factorial for non-negative integers. However, if you call it with a negative number, it recursively calls itself infinitely, eventually causing a `RecursionError` because Python has a limit on the maximum recursion depth.

## The Solution

The `bugSolution.py` file addresses this problem by adding a check for negative input.  If `n` is negative, it raises a `ValueError` indicating that the factorial is not defined for negative numbers. This prevents infinite recursion and provides a more informative error message.
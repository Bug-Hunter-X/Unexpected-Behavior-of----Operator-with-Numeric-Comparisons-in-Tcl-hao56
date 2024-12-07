# Tcl == Operator Bug

This repository demonstrates a common error in Tcl programming related to the unexpected behavior of the `==` operator when comparing numbers.  The `==` operator in Tcl performs string comparison by default, which can lead to incorrect results when comparing numeric values.

## Bug Description
The provided Tcl code defines a procedure `badproc` that attempts to check if its input `x` is equal to 0 and return 1 if true, and 0 otherwise. However, due to the use of the `==` operator, the comparison is performed as a string comparison instead of a numerical comparison.

## Solution
The solution uses the `eq` operator, which performs strict numerical comparison. This ensures that the function correctly identifies when the input is numerically equal to 0.
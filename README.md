# Ada Integer Overflow Bug

This repository demonstrates a potential integer overflow bug in Ada code. The function `Check_Range` checks if a given integer is within the range [10, 20]. However, this function does not properly handle integer overflow.  If the input number is very large or very small, this will lead to incorrect results. The provided code includes a test case to demonstrate this behavior.  A solution to address the integer overflow is provided in `bugSolution.ada`.

## Bug Description

The `Check_Range` function in `bug.ada` does not handle cases where the integer input might exceed the maximum or minimum representable value for the `Integer` type.  This can result in unexpected and incorrect Boolean return values.
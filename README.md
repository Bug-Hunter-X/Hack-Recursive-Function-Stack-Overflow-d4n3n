# Hack Recursive Function Stack Overflow

This repository demonstrates a common error in recursive functions written in Hack: stack overflow. The `foo()` function calculates the factorial, but without a base case that properly handles inputs effectively.  The `main()` function calls `foo()` with 5 as input. For small inputs, this works correctly. However, if you increase the input significantly, it will cause a stack overflow error. This is because each recursive call adds a new frame to the call stack, and eventually the stack space is exhausted.

The solution involves modifying the function to use iteration or tail recursion to avoid excessive stack usage.
# Dangling Pointer and Incorrect free() Usage

This repository demonstrates a common C programming error: attempting to free memory allocated on the stack using the `free()` function.  The `free()` function is intended for dynamically allocated memory (using `malloc`, `calloc`, etc.). Attempting to use it with stack-allocated memory is undefined behavior and can lead to crashes or unpredictable results.

The `bug.c` file shows the incorrect code, and the `bugSolution.c` file shows the corrected version.
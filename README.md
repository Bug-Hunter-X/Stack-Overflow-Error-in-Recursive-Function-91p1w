# Stack Overflow Bug in JavaScript

This repository demonstrates a common error in JavaScript: a stack overflow error caused by uncontrolled recursion. The `foo` function recursively calls itself without a proper base case, leading to excessive function calls and eventually exceeding the call stack limit.

## Bug

The `bug.js` file contains the buggy code. When the function `foo` is called with a large value for the first argument ('a'), it recursively calls itself until the call stack is full, resulting in a stack overflow error.

## Solution

The `bugSolution.js` file provides a corrected version of the code. The solution introduces a check for 'a' and if its value is less than 0, returns b. This way, the recursion is eventually stopped, preventing the stack overflow. 

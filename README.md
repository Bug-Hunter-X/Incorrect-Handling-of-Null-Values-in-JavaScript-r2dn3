# Incorrect Handling of Null Values in JavaScript

This repository demonstrates a common error in JavaScript: incorrect handling of null values. The function `foo` returns `null` if either input is `null`, even if the other input is a number. This can lead to unexpected behavior if the function is used in a larger program.

The `bug.js` file contains the buggy code, while `bugSolution.js` contains a corrected version that handles null values more gracefully.

## Bug

The `foo` function incorrectly handles null values. If either `a` or `b` is null, it returns null, regardless of the other parameter's value.  This is likely not the intended behavior.

## Solution

The solution adds a check to see if either parameter is null. If one is null, the other parameter's value is returned; otherwise, the sum is returned.  This ensures the function produces more useful outputs when one input is unexpectedly null.
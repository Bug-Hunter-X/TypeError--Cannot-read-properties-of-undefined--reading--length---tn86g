# JavaScript Bug: Handling Undefined Values

This repository demonstrates a common JavaScript error: attempting to access a property of an undefined object.  The `foo` function is designed to return the length of an array, but it fails when given `undefined` as input. This demonstrates the importance of robust error handling and input validation in JavaScript.

## Bug Description
The `foo` function doesn't explicitly handle the `undefined` case, leading to a `TypeError` when attempting to access the `length` property of `undefined`. 

## Solution
The solution adds an explicit check for `undefined` before accessing the `length` property, preventing the error and returning 0 in that case. 
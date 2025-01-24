# JavaScript Null Value Handling Bug

This repository demonstrates a common, yet subtle, bug in JavaScript related to how null values are handled during arithmetic operations. The `foo` function is designed to add two numbers, but it incorrectly returns 0 if either input is null. This occurs because of the implicit type coercion that JavaScript performs when adding null to a number.  The solution involves explicitly checking for null values and handling them appropriately. 

## Bug

The `bug.js` file contains the faulty implementation of the `foo` function. The function uses loose equality (`===`) to check for null values; however, this isn't sufficient to prevent unexpected results in arithmetic contexts. 

## Solution

The `bugSolution.js` file provides a corrected version of the function.  The solution explicitly handles null values by converting them to 0 before performing the addition. This avoids the implicit type coercion and ensures the function behaves correctly for all input values. 
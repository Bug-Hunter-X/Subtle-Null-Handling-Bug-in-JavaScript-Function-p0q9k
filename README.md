# Subtle Null Handling Bug in JavaScript Function

This repository demonstrates a common, yet subtle, error in JavaScript related to null value handling within a function.

## Description

The `foo` function is designed to add two numbers. However, it contains a logic flaw in how it deals with `null` values. While it correctly handles cases where one parameter is null, it fails if *both* parameters are null.

## Bug

The original `bug.js` file contains the erroneous code.  It returns 0 when either parameter is null, but does not consider the case where both parameters are null.  This results in a seemingly unexpected outcome.

## Solution

The solution provided in `bugSolution.js` adds a check to specifically handle the case where both parameters are null, providing a more robust and expected behavior.

## How to run

1. Clone the repository.
2. Open both `.js` files.
3. Run the Javascript code in your preferred environment (browser console, Node.js, etc.).  Observe the outputs of the console.log statements.
# JavaScript: Unexpected Addition Behavior with undefined and null

This repository demonstrates unexpected behavior in JavaScript's addition operator when dealing with `undefined` and `null` values. Specifically, it highlights the difference in how these values are treated during addition.

## Bug Description
The addition operator (+) in JavaScript handles `undefined` and `null` differently.  `undefined` results in `NaN`, while `null` is treated as 0.  This can lead to unexpected results if not carefully considered.

## How to Reproduce
1. Clone this repository.
2. Run `bug.js` using a JavaScript runtime (e.g., Node.js).
3. Observe the output, noting the discrepancies between the addition operations.

## Solution
The `bugSolution.js` file provides a solution by explicitly handling `undefined` and `null` values before performing addition to avoid unexpected results.  This ensures that any potential `undefined` or `null` values are converted to 0 before the summation is executed, making the behavior more predictable.

## Additional Notes
Understanding how JavaScript handles type coercion is crucial to prevent these types of errors. Explicit type checking and handling of potential nullish values are highly recommended when writing robust JavaScript code.
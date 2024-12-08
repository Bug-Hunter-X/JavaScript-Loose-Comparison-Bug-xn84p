# JavaScript Loose Comparison Bug

This repository demonstrates a common error in JavaScript: using loose comparison (==) instead of strict equality (===) when checking for null values. Loose comparison can lead to unexpected behavior and errors in your code.

## Bug Description

The provided code snippet demonstrates a function that performs addition. However, it incorrectly uses loose comparison to check for null values. As a result, the code produces unexpected results when handling null inputs. This is because loose comparison may implicitly convert values before comparing them, leading to unexpected matches.

## How to Reproduce

1. Clone this repository.
2. Run `node bug.js`.
3. Observe the incorrect output caused by the loose comparison.
4. Run `node bugSolution.js` to see the correct output using strict equality.

## Bug Solution

The solution involves using strict equality (===) to ensure accurate null value comparison. Strict equality does not perform implicit type conversion, ensuring that only identical values will match. This prevents the unexpected behavior seen with loose comparison. 
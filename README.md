# MongoDB $inc Operator Type Error
This example demonstrates a common error when using the `$inc` operator in MongoDB update operations.  The `$inc` operator is used to increment a numerical value.  However, if you provide a string value instead of a number, MongoDB will not throw an error but will likely produce unexpected results.

## Bug
The provided code snippet attempts to increment the `count` field by '1' (a string). This will not increment the field as expected. 

## Solution
The solution involves ensuring that the increment value is a number (integer or floating point), as demonstrated in `bugSolution.js`.
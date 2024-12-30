# MongoDB $inc Operator Error: Non-numeric Increment Value

This repository demonstrates a common error in MongoDB update operations when using the `$inc` operator.  The `$inc` operator is used to increment a numeric field by a specified value. However, if you provide a non-numeric value as the increment, MongoDB will throw an error.

The `bug.js` file showcases the incorrect usage of `$inc` with a non-numeric value.  The `bugSolution.js` demonstrates the correct usage with a numeric value.

## How to reproduce the error

1.  Make sure you have a MongoDB instance running.
2.  Create a collection named `myCollection` with a document containing a numeric field named `count`.
3.  Run the `bug.js` script.
4.  Observe the error message.

## Solution

The solution, provided in `bugSolution.js`, corrects the increment value to a number which will allow the MongoDB update operation to succeed without error.
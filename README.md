# MongoDB $inc operator error
This repository demonstrates a common error when using the `$inc` operator in MongoDB update operations. The `$inc` operator is used to increment a numerical field by a specified value.  However, if a string is provided instead of a number, it results in an error or unexpected behavior.

The `bug.js` file showcases the incorrect usage, while `bugSolution.js` provides the corrected code.

## Bug Description
The primary issue is providing a string ('1') to the $inc operator instead of a number (1).  This leads to either an error or the counter not being incremented correctly, which is usually unexpected behavior.

## Solution
The correct approach is to provide a numerical value to `$inc`.
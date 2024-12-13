# Incorrect Use of $inc Operator in MongoDB Update Query

This repository demonstrates an uncommon error in MongoDB update queries involving the `$inc` operator.  Specifically, it showcases the issue of using a string instead of a number with the `$inc` operator. This can lead to unexpected behavior and incorrect updates.

The `bug.js` file contains the erroneous code. The `bugSolution.js` file provides the corrected version.

## Bug
Using a string value with the `$inc` operator will not increment the field but will instead add a string to the value in a unexpected way.

## Solution
Ensure that you are using a number value as a parameter for the `$inc` operator.
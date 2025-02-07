# Incorrect use of $inc operator in MongoDB update
This example demonstrates an uncommon error in MongoDB update operations using the `$inc` operator.
The error arises from using a string instead of a number for the increment value, which results in unexpected behavior.

## Bug
The bug is in the `updateOne` operation in the provided code snippet. The `$inc` operator expects a numerical value for the increment, but instead, a string value ('1') is provided which does not increment the field.

## Solution
The solution corrects the error by using the numerical value 1 instead of the string value '1'.
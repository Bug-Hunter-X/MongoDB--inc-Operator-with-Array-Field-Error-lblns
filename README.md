# MongoDB $inc Operator with Array Field
This repository demonstrates a common error encountered when using the `$inc` operator in MongoDB with array fields. The error arises from incorrectly applying the `$inc` operator, leading to unexpected results.

## Bug Description
The bug involves attempting to increment a field within an array using the `$inc` operator without the correct use of the positional operator (`$[<expression>]`).  This usually results in an update not being applied or applying to the wrong document.

## Solution
The solution demonstrates how to correctly utilize the positional operator (`$[]`) to modify the specified array element.  This ensures that only the intended elements are incremented accurately. 
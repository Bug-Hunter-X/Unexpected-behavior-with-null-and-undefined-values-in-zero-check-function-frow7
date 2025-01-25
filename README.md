# Unexpected behavior with null and undefined values in zero-check function
This code demonstrates a common JavaScript issue where loose comparison (==) with 0 can lead to unexpected results when null or undefined are passed as arguments.
The function foo is intended to return 0 if either a or b is 0, otherwise it returns their sum. However, due to JavaScript's type coercion, null and undefined are treated as 0 in the loose comparison, resulting in unexpected output for the calls with null as input.  The solution below illustrates a safer way to check for these values.

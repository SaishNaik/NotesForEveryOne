# Tips

For rotating a 2D array or matrix, always transpose the matrix first. Then flip or swap the columns in case of clockwise rotation or swap the rows in case of anticlockwise rotation. One whole operation of transpose and swap flips it by 90 degrees.

To convert a numeric char to int in java, `int temp = numeric_character - '0';`

In Java, only signed integers are present. However we should not be worried about its implementation as long as we are using bit operators. The system will give the correct result in case of any bit operations while using it as a integer.

In bit manipulation problems, whenever you are asked for "difference in the corresponding bits", always think of `xor` operator. `Integer.bitCount` counts the no of 1 bits in java.
A number XOR itself will become 0. Any number XOR with 0 will stay unchanged.

In array, if told to find the sum of n nos where n > 2, try to fix nums and reduce the problem to  sum of  2 nos.

In case of duplicates not to be included in Array , try to sort if feasible. Then while traversing you can ignore elements if duplicate easily. 





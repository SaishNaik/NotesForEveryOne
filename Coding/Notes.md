# Tips

For rotating a 2D array or matrix, always transpose the matrix first. Then flip or swap the columns in case of clockwise rotation or swap the rows in case of anticlockwise rotation. One whole operation of transpose and swap flips it by 90 degrees.

To convert a numeric char to int in java, `int temp = numeric_character - '0';`

In Java, only signed integers are present. However we should not be worried about its implementation as long as we are using bit operators. The system will give the correct result in case of any bit operations while using it as a integer.

In bit manipulation problems, whenever you are asked for "difference in the corresponding bits", always think of `xor` operator. `Integer.bitCount` counts the no of 1 bits in java.
A number XOR itself will become 0. Any number XOR with 0 will stay unchanged.

In array, if told to find the sum of n nos where n > 2, try to fix nums and reduce the problem to  sum of  2 nos.

In case of duplicates not to be included in Array , try to sort if feasible. Then while traversing you can ignore elements if duplicate easily. 

In case of matrix,  rowcount = matrix.length , columncount = matrix[0].length. 

If it says found cycle in the list or other similar message in case of linkedlist problems, check if you have added null as last element of linked list. eg. if `temp` points to last node, make sure `temp.next= null`  is set. This found cycle error 
usually occurs when modifying an existing list `in place`.

If you encounter `The order of your output does not matter.`, it is likely that the problem solution might involve sorting or other order changing method.

If you are finding index of a character for a 0 based aplhabetic array use `c - 'a'` where c is the character whose position you want to find.

To convert int to char `char c = (char)(int_value)`

To convert int to character in a to z, `char c = (char)(a+int_value)` where int_value is between 0 and 25 both inclusive.

Always implement min heap with a array.It makes it easier to add the element at the bottom.

Decimal value of a is 97 and A is 65

Permutations means order matters. Combination order does not matter.

Binary tree representation as a array is left child = 2*parentindex + 1, right child = 2*parentindex + 2

//todo check if it is correct. If not needs to be deleted 
Whenever a variation of a given problem is given such as finding the length of the longest palindromic substring in a substring, try to solve the smaller problem ( in this case palindrome) in a way that would help you in getting the final solution as palindrome check can be done in many ways.   
//todo check if it is correct. If not needs to be deleted

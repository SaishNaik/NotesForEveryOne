# Tips 

Note: `There are certain tips only specific to java`

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

Given a problem to find max or min where the data set may contain Max integer and Min integer, use the Integer class. Because
it will allow to define the start/initial value as null.

We can use == operators for reference comparison (address comparison) and .equals() method for content comparison. In simple words, == checks if both objects point to the same memory location whereas .equals() evaluates to the comparison of values in the objects.

In bit manipulation, mask is a no that you will compare the given number against for a particular operation to get the desired result.

Arrays.binarySearch() returns the index of the search key, if it is contained in the array; otherwise, (-(insertion point) – 1).  
The insertion point is defined as the point at which the key would be inserted into the array: The index of the first element greater than the key, or array.length if all elements in the array are less than the specified key.

Use Greedy Algorithms only if there is a single path from the current state.

In Java, primitive types and even Integers  wont be updated in function calls, So either use a array or list.


//todo check if it is correct. If not needs to be deleted 
Whenever a variation of a given problem is given such as finding the length of the longest palindromic substring in a substring, try to solve the smaller problem ( in this case palindrome) in a way that would help you in getting the final solution as palindrome check can be done in many ways.   
//todo check if it is correct. If not needs to be deleted

Strings.replace("old","new") will replace characters or char sequence .
Strings.replaceAll("regexold","new") will replace it with regex.
Strings.replaceAll("\\.","new") to replace . with new  

Cycle sort is an in-place sorting Algorithm, unstable sorting algorithm, a comparison sort that is theoretically optimal in terms of the total number of writes to the original array. This sorting algorithm is best suited for situations where memory write or swap operations are costly.

(1<<32) -1 gives you a bit mask for 32 bit integer.

 If last bit is set then the number is odd, otherwise even. 
 
 to convert Integer list to int[] , use  `l.stream().mapToInt(i->i).toArray();`
 
Iterate through map
 ```
 for (Map.Entry<String, Integer> entry : map.entrySet()) {
            System.out.println(entry.getKey() + "/" + entry.getValue());
}
```

If there is something common to find, many times hashmaps can be used.

to go through all characters of string
```str.chars().forEach(c->{});```


Removing characters from array,use 2 pointer approach

String.valueOf()  This method returns the string representation of the passed argument.

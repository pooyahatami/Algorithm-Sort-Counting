[![Build Status](https://secure.travis-ci.org/soldair/node-binarysearch.png)](https://github.com/pooyahatami/Algorithm-Sort-Counting/)
# Algorithm-Sort-Counting
Counting sort is a sorting technique based on keys between a specific range. It works by counting the number of objects having distinct key values (kind of hashing). Then doing some arithmetic to calculate the position of each object in the output sequence.

```javascript
 * Counting sort algorithm !
 * Class	Sorting algorithm
 * Data structure	Array
 * Worst-case performance	О(n+k) comparisons, swaps
 * Best-case performance	O(n+k) comparisons, O(1) swaps
 * Average performance	О(n+k) comparisons, swaps
 * Worst-case space complexity
 ```
 
Let us understand it with the help of an example.

```javascript
For simplicity, consider the data in the range 0 to 9. 
Input data: 1, 4, 1, 2, 7, 5, 2
  1) Take a count array to store the count of each unique object.
  Index:     0  1  2  3  4  5  6  7  8  9
  Count:     0  2  2  0   1  1  0  1  0  0

  2) Modify the count array such that each element at each index 
  stores the sum of previous counts. 
  Index:     0  1  2  3  4  5  6  7  8  9
  Count:     0  2  4  4  5  6  6  7  7  7

The modified count array indicates the position of each object in 
the output sequence.
 
  3) Output each object from the input sequence followed by 
  decreasing its count by 1.
  Process the input data: 1, 4, 1, 2, 7, 5, 2. Position of 1 is 2.
  Put data 1 at index 2 in output. Decrease count by 1 to place 
  next data 1 at an index 1 smaller than this index.
```

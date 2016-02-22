# What is Big-O Notation? 

Big-O Notation refers to the time it takes to compute an algorithm in relation to the number of inputs given 

Big-O Complexity (Best to Worst): 

1. **Constant Time** O(1): It takes the same amount of computation time regardless of the size of your input; an increase in the size of the input does not mean increase in computation time; it is constant
	* Use case: Pushing and popping elements in array 
2. **Logarithmic** O(log n): By reducing the number of elements in consideration, we reduce computation time (i.e. starting computation at the center of array instead of the beginning, thereby reducing the number of inputs in half)
	* Use case: Binary trees and binary search trees
3. **Linear** O(n): It takes an equal amount of work on *each* element in the input; an increase in the size of the input means an increase in computation time    	 
	* Use case: Iterating over every element of an array
4. <strong>Quadratic</strong> O(n^2): When the size of the input doubles, the computation time increases four-fold
	* Use case: Nested loops and sorting
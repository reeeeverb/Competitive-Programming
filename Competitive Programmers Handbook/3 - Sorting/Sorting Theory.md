## Sorting Theory
- many problems are easier to solve when dealing with sorted input so sorting is often a sub problem 

#### Algorithmns of Note
- **Bubble sort** is an $O(n^2)$ algo where upon each iteration the algo iterates through the elements and swaps any two consecutive elements that are not in the correct order 
	- after the first round the largest element will be in the correct positions and after k rounds the k largest elements will be in the correct positions 
	- Any algorithmn that relies upon swapping consecutive elements will be at least $O(n^2)$ complexity 
- **Merge Sort** is an $O(n * log(n))$ algo that is based on recursion, it spits the array into smaller subarrays, sorts the subarrays and then functions as a double pointer problem to combine the 2 sub arrays back into one large, sorted array 
	- fastest possible sorting algo under most conditions
- **Counting Sort** is capable of sorting in $O(n)$ time assuming that every element in the array is an integer between 0 and c. This allows for the creation of a *bookkeeping array* whose indices are elements of the original array. We then iterate through the original array and calculate how many time each int from 0 to c shows up within the array.
	- ie the array \[1,3,6,9,9,3,5,9\] (with the assumption that all numbers are between 0 and 9) becomes the *bookkeeping array* \[1,0,2,0,1,1,0,0,3\]
	- extremely efficent and useful algo in certain circumstances
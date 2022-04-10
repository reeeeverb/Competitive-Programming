## Binary Search
- a general method for search for an element is to use a for loop and iterate through all of the elements 
	- if the order is arbitrary this is the best approach 
- if the elements are sorted binary search is the most efficent approach 

#### C++ Functions to Implement Binary Search
- Assuming that the array is sorted 
	- lower_bound returns a pointer to the first array element whose value is at least x 
	- upper_bound return a poijnter to the first array element whose value is larger than x 
	- equal_range returns both above pointers 
``` C++
auto a=lower_bound(array, array+n, x);
auto c=upper_bound(array, array+n, x);
auto r=equal_range(array, array+n, x);
```
- if there is no such element in the array it returns the element after the last array element
	- the following code find out whether an array contains an element with value x
```C++
auto k = lower_bound(array,array+n,x)-array;
if(k<n && array[k] == x){
	//x was found at index k
}
```
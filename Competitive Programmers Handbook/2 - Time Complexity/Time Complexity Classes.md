## Complexity Classes 
Short hand | Description
:-----------|:-----------
O(1) | Constant-time(independent of input)
O(logn)| Logarithmic, halves input size at each step
O($\sqrt{n}$) | sqaure root
O(n) | linear, accesses each input element once
O(n log n) | the time complexity of most efficent sorting algos
O($n^2$) | quadratic, two nested loops
O($n^3$) | cubic, three nested loops
O($2^n$) | Often indicated the algo iterates through all subsets of the input elements
O(n!) | Indicated the algo iterates through all permuations of the input elements

- an algo is polynomial if its complexity is anything on the above table other than O($2^n$) and O(n!)
	- this is considered to be efficent 
	- most algo fall under this category 

## Estimating Efficency 
- the time complexity required by a problem can be estimated based upon input size
	- assumes limit of 1 second 
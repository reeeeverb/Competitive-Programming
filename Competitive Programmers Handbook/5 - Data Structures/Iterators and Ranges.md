## Iterators and Ranges 
- An **iterator** is a variable that points to an element in a data structure 
	- `s.begin()` points at the first element
	- `s.end()` points *after* the last element

#### Ranges 
- ranges are frequently used in C++ as the elements within a data structure
```C++
sort(v.begin(), v.end());
reverse(v.begin(), v.end());
random_shuffle(v.begin(), v.end());
```

#### Set Iterators
- iterators are often used to access elements of a set
- `auto it = s.begin();`
- the elements to which an iterator point can then be accessed by using the * symbol
- `cout << *it << "\n";`
- iterators can be moved using the operators ++(forward) and --(reverse)
```C++
for(auto it = s.begin(); it!=s.end(); it++){
	cout << *it << "\n";
}
```
- few more functions involving set iterators
```C++ 
auto it = s.find(x)
if(it == s.end){
	//x is not found
}
s.lower_bound(x); // return first element in set greater than x
s.upper_bound(x); // return lowest element in set less than than x
```
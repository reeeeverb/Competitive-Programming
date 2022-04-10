## Dynamic Array
- array whose size can be changed during the execution of a program 
- the most popular is the vector 
``` C++
for(auto x : v){ // easiest way to print all elements 
	cout << x << "\n";
}

v.back(); // returns the last element in a vector 
v.pop_back() // returns the last element and deletes it from the vector 
v.push_back(2)

vector<int> v(10); //vector size 10 all 0s
vector<int> v(10,5); //vector size 10 all 5s
```
- string structures are a type of dynamic array 

#### Other Structures 

- Deque 
	- a dynamic array whose size can be changed at both ends 
	- inlcudes push_back, pop_back, push_front and pop_front 
	- slightly slower than a vector 
- Stack 
	- can only add and remove an element from the top 
- Queue 
	- can only add and remove an element from the end
- 


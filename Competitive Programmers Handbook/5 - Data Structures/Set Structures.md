## Set Structures 
- maintains a collection of elements 
- 3 standard operations 
	- insertion 
	- search 
	- removal 
- Two standard implementations 
	- set 
		- based on a balanced binary tree 
	- unordered_set 
		- uses hashing, less functionallity but can be more efficent 
```C++
set<int> s;
s.insert(3);
s.insert(2);
s.insert(5);
cout << s.count(3) << "\n"; // 1
s.erase(3);
cout << s.count(3) << "\n"; // 0
```
- all elements are distinct 
	- count will return either a 1 or 0 
- multiset and unordered_multiset override this rule 
	- s.erase(5) will remove all instances of 5 
		- s.erase(s.find(5)) will only erase one instance

#### 
## Map Structures 
- generalized array that consists of key-value pairs 
``` C++
map<string, int> m; // creates a map where strings are key and ints are values 

m["monkey"] = 4;
m["banana"] = 3;

cout << m["banana"] << "\n"; // 3

cout << m["aybabtu"] << "\n"; // key is not in map so it is added with default value (0)

if(m.count("banana")){
	// key exists
}
```

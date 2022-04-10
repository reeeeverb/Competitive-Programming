## Bitset
- contains only 1s and 0s 
	- very small memory footprint 
```C++
bitset<10> s(string("0010011010")); // from right to left
cout << s[4] << "\n"; // 1
cout << s[5] << "\n"; // 0

s.count() // returns the number of 1's (4)
```
- very easy to execute small bitwise operations
```C++
bitset<10> a(string("0100110100"));
bitset<10> b(string("0010011010"));

cout << (a&b) << "\n"; // 0000010000
cout << (a|b) << "\n"; // 0110111110
cout << (a^b) << "\n"; // XOR 0110101110
```
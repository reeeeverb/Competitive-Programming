## Starter Template

- Basic template for a file is as follows 
``` C++
#include <String>
#include <iostream>

using namespace std;

ios::sync_with_stdio(0);
cin.tie(0);

int main(){

	freopen("input.txt", "r", stdin);
	freopen("output.txt", "w", stdout);
	//solution comes here
} 
```
- basic code compilation 
``` g++ -std=c++11 -O2 -Wall test.cpp -o test```
	- standard is c++ 11
	- -O2 optimizes the code 
	- Warning about possible errors are shown because of -Wall
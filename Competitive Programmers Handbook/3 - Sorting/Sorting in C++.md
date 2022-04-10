## Sorting in C++

 - don't use homemade sorting algos, just don't 

#### C++ Sort Function for Vectors
- to sort in increasing order
```C++
vector<int> v = {4,2,5,3,5,8,3};
sort(v.begin(),v.end()); 
```
- and decreasing order
```C++
vector<int> v = {4,2,5,3,5,8,3};
sort(v.rbegin(),v.rend()); 
```

#### C++ Sort Function for Arrays
- sorting an array 
```C++
int n = 7; // array size
int a = [4,2,5,3,5,8,3];
sort(a,a+n); 
```
- sorting a string
```C++
string s = "monkey";
sort(s.begin(), s.end()); //results in ekmnoy
```
- in sorting a pair or tuple the first element will be compared then the second if they are equal and finally third if applicable

#### User Defined Structs
- in order to a user defined struct to be able to use the sort function a comparision operator must be definied
```C++
struct P{
	int x,y;
	bool operator<(const P &p){
		if(x!= p.x) return x < p.x;
		else return y < p.y
	}
}
```

#### Comparison Functions 
- it also possible to create a custom defined sort of comparision rather than the default
- for example sorting strings by their length
```C++
bool comp(string a, string b){
	if(a.size() != b.size()) return a.size() < b.size();
	return a<b;
}

sort(v.begin(), v.end(), comp) //Sorting a vector of Strings
```

- **Complete Search** is a method used to solve problems where one generates all possible solutions to a problem and then selects the best solution 
		- is a good technique if there is enough time to go through all the solutions, as it is easy to implement and will always yeild the correct solution 
	- other techniques include greedy algos or dynamic programming may be needed if time is a restraint 

#### Generating Subsets
- the problem of generating all subsets of a set of n elements 
- **Solution 1** using recursion
```C++
void search(int k){
	if(k==n){
		// process subset
	}else{
		search(k+1);
		subset.push_back(k);
		search(k+1);
		subset.pop_back();
	}
}
```
- I would have litterally never though of this, wack as fuck 
- **Solution 2** using a bit sequence 
```C++
for(int b = 0; b < (1<<n); b++){
	vector<int> subset;
	for(int i = 0; i < n; i++){
		if(b&(1<<i)) subset.push_back(i);
	}
}
```


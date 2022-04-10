## Input and Output 
- cin and cout are the default options for input and output 
```C++
ios::sync_with_stdio(0);
cin.tie(0);
```
- optimizes the input and the output 
- **new line (\\n) is always faster than endl**
- ```scanf``` and ```printf``` are usually a bit faster but they are more difficult 
- ```printf("%d %d\n, a, b)"```
- ```scanf("%d %d\n, &a, &b)"```
- ```getline(cin,s)``` is used to get a whole line from input and set it equal to s 
```C++
while(cin >> x){
	//useful for when the amount of data is unknown 
}
```
- when a file is being used for input or output simply add these at the start of the program 
```C++
freopen("input.txt", "r", stdin);
freopen("output.txt", "w", stdout);
```

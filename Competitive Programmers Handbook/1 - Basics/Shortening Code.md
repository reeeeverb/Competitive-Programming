## Shortening Code 
#### Typedef 
- makes it possible to give a shorter name to a datatype 
```C++
typedef long long ll;
typedef vector<int> vi; 
typedef pair<int,int> pi;
```

#### Macros 
- certain strings in the code will be changed before the compilation 
```C++
#define REP(i,a,b) for (int i =a; i <= b; i++)

# define F first
# define S second
# define PB push_back
# define MP make_pair
```
- can be somewhat unpredicatable and bugs can be much harder to detect
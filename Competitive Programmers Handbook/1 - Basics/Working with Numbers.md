## Working With Numbers 
- int is a 32 bit long number 
- long long is a 64 bit long number 
- `__int28_t` is a 128 bit number

#### Floating Point Numbers
- `double` is 64 bits long
- `long double` is 80bits
-  printing required precision is specificed as 
```C++
// prints x with 9 decimal places
printf("%.9f\n, x")
```
- when comparing floating point numbers do not use ```==``` but rather 
```C++ 
if (abs(a-b) < 1e-9) { 
// a and b are equal 
}
```

#### Modulos 
- Many answers just want the modulus of a result 
	- this allows you to take the modulo prior to the end of the problem as (a mod m + b mod m) is the same as a+b mod m 
		- this also true of subtraction and multiplication
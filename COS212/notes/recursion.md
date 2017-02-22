# Recursion

Recursion involves a function repeatedly calling itself until an answer is found.
<br>

## Examples

### Factorial
#### Pseudo code
```pseudo
	factorial(n):
		if n is greather than one
			return n * factorial(n - 1)
		else
			return 1
```
#### java
```java
int factorial(int n){
    if (n > 1){
        return n*factorial(n-1);
    }
    else {
        return 1;
    }
}
```

# Recursion

Recursion involves a function repeatedly calling itself until an answer is found.
It is often associated with breaking a problem down into smaller parts
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
#### Java
```Java
int factorial(int n){
    if (n > 1){
        return n*factorial(n-1);
    }
    else {
        return 1;
    }
}
```

___

### Fibonacchi
#### Pseudo code
```pseudo
	fib(n):
	if n is smaller than or equal to 1
		return n;
	else
		return fib(n-1) + fib(n-2)
```
#### Java
```Java
public int fib(int n) {
    if(n <= 1) {
        return n;
    } else {
        return fib(n - 1) + fib(n - 2);
    }
}
```

___

## Backtracking

Backtracking involves 'going back' to solve a particular problem.
Eg If you are driving and get lost you turn back and try to find a road that you remember.

A popular problem solved with backtracking is the N-Queen problem;<br>
This is where you place N queens on a chessboard with NxN slots so that no 2 queens
can attack each other.

<br>![No internet](http://i.imgur.com/O3cGlYv.gif)

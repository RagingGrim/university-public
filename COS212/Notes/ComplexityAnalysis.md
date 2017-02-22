# Complexity Analysis

Basically covers the fact that all algorithms have tradeoffs. In the case of complexity analysis space (RAM) and time (execution time) is mainly considered.

Let f(n) be the function that describes the complexity of an algorithm. We are only concerned with asymptotic complexity ; which is to say we are only concerned with the order of complexity ( magnitude of a function ).

This means that the function f(x) has a low order of complexity compared to g(x)<br>
![No connection](https://latex.codecogs.com/gif.latex?f(x)&space;=&space;x^2)<br>
![No connection](https://latex.codecogs.com/gif.latex?g(x)&space;=&space;x^3)<br><br>

We determine the complexity of f(n) by deciding which terms contribute the most and discarding the others.

## Big O Notation
### Introduction
![No connection](https://latex.codecogs.com/gif.latex?O%28g%28n%29%29)<br>

Let g(n) be the worst case performance of f(n); Big O Notation can then be defined as the 'slowest' possible performance of a function.

### Examples

     f(n)       | Big-O
:-------------: | :----:
     2n^2       | ![No connection](https://latex.codecogs.com/gif.latex?g(x)&space;=&space;x^3)
   100000n^2    | O(n^2)
   2n + n^2     | O(n^2)
10 + n + log(n) |  O(n)
10n^3 + 364n^2  | O(n^3)

![No connection](https://upload.wikimedia.org/wikipedia/commons/thumb/7/7e/Comparison_computational_complexity.svg/1920px-Comparison_computational_complexity.svg.png)

### Common algorithms

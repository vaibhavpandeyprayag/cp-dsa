# Dynamic Programming

It is an optimization technique which is applicable to problems that have 2 properties - **_Optimal substructure_** and **_Overlapping sub-problems_**.

## Fibonacci Series

0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55...

**How the series is formed:** The first and second terms are set to 0 and 1 respectively. Now the nth term is caluculated by calculating sum of (n-1)th term and (n-2)th term.

To recursively calculate the nth term of fibonacci series, 2 things are required (required in all recursive solution obviously): recurrence relation (recursive step) and base condition (codition at which the recursion stops).  
In this case (Here F is the recursive function which returns fibonacci term):

1. Recurrence relation: F(n) = F(n - 1) + F(n - 2).
2. Base condition: F(1) = 0, F(2) = 1.

```cpp
fib(int n) {
    if (n == 1) return 0;
    if (n == 2) return 1;

    return fib(n - 1) + fib(n - 2);
}
```

# Written:
### Problem 1: (5pts) Consider the following algorithm:
1. Write a recurrence for the running time T(n) of Goo(n).
```
T(n) = Theta(1) + T(n-2)
```

2. Solve the recurrence for the asymptotic running time. Assume that addition can be done in constant time. Use theta notation.
```
T(1) = 1
T(2) = T(2-2) = 1
T(1) <= c(1) for all c>=1
T(2) <= c(2) for all c>=2
Thus T(n) => O(n)
```

### Problem 2: (5pts) Consider the following algorithm:
1. Write a recurrence for the running time T(n) of Foo(n).
```
T(n) = Theta(1) + 2T(n/4) + Theta(n^2)
```

2. Solve the recurrence for the asymptotic running time. Assume that addition can be done in constant time. Use theta notation.
```
A = 2, b = 4, f(n) = n^2
Log_b(a) = log_4(2) = 0.5
Thus T(n) = Theta(f(n)) = Theta(n^2)
```

### Problem 3: (5 pts) Consider the following cruel and unusual sorting algorithm.
1. Give a recurrence for the running time T(n) of the UNUSUAL function.
```
T(n) = Theta(1) + Theta(n) + 3T(n/2)
```

2. Solve the recurrence in part 1 to find the running time of UNUSUAL use Theta notation.
```
A = 3, b = 2, F(n) = n
Log_2(3)
T(n) = Theta(n^log_2(3)) = Theta(n^1.58)
```

### Extra Credit:
1. Give a recurrence for the running time T(n) of the CRUEL function.
```
T(n) = 2T(n/2) + Theta(n^log2(3))
```

2. Solve the recurrence in part 1 to find the running time of CRUEL use Theta notation.
```
A = 2, b = 2, f(n) = n^log_2(3)
T(n) = Theta(n^log_2(3))
```

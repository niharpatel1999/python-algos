# Recursion

Recursion is a common mathematical and programming concept. It means that a function calls itself. This has the benefit of meaning that you can loop through data to reach a result. The only problem with recursion is that without a proper exit condition, the code could got into infinite loop.


<img src="https://i.imgur.com/Myvtk0G.jpg" alt="image" width="75%" height="auto">

### Factorial using Recursion

As you can see in the below code, the function calls itself with a base case.
For example `fact(5)` would lead to `5 * fact(4)`, again the `fact(4)` will lead to `4 * fact(3)`, and similarly the final result would be `5*4*3*2*1`.

```python
def factorial(num):
  if num == 1:
    return 1
  return num * factorial(num-1)
```

### Fibonacci using Recursion

Similarly, `fibonacci(n)` would call `fibonacci(n-1) + fibonacci(n-2)` with a appropriate exit condition.
```python
def fibonacci(num):
    if num < 2:
        return num
    return fib(num-1) + fib(num-2)
```

For more reading on recursion in pytho, please refer <a href ="https://realpython.com/python-recursion/#what-is-recursion">here</a>.
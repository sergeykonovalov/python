# Functions

One should define functions before using them.

## Docstring

Everything inside triple quotes is function's docstring (funcname.__doc__)

## Named Arguments

If you send arguments and their names match those defined inside of function, no matter which order of arguments in the call.

```python
def some_func(a, b=False)

some_func(100, b=False)  # ok
some_func(a=100, b=False)  # ok
some_func(b=False, a=100)  # ok
some_func(b=False, 100)  # error, you have named argument, followed by unnamed (positional); reading arguments left to right once you have a single named argument, the rest of arguments should also be named
some_func(a=100, False)  # error; same reason as above
```

# Booleans

Booleans represent one of two values: `True` or `False`.

### Boolean Values

In programming you often need to know if an expression is `True` or `False`.

You can evaluate any expression in Python, and get one of two answers, `True` or `False`.

When you compare two values, the expression is evaluated and Python returns the Boolean answer:

```
// Some code

print(10 > 9)
print(10 == 9)
print(10 < 9)
```

#### Example

Print a message based on whether the condition is `True` or `False`:

```
// Some code
a = 200
b = 33

if b > a:
  print("b is greater than a")
else:
  print("b is not greater than a")
```

### Evaluate Values and Variables

The `bool()` function allows you to evaluate any value, and give you `True` or `False` in return,

#### Example

Evaluate two variables:

```
// Some code
x = "Hello"
y = 15

print(bool(x))
print(bool(y))
```

### Most Values are True

Almost any value is evaluated to `True` if it has some sort of content.

Any string is `True`, except empty strings.

Any number is `True`, except `0`.

Any list, tuple, set, and dictionary are `True`, except empty ones.

#### Example

The following will return True:

```
// Some code
bool("abc")
bool(123)
bool(["apple", "cherry", "banana"])
```

### Some Values are False

In fact, there are not many values that evaluate to `False`, except empty values, such as `()`, `[]`, `{}`, `""`, the number `0`, and the value `None`. And of course the value `False` evaluates to `False`.

#### Example

The following will return False:

```
//Example code
bool(False)
bool(None)
bool(0)
bool("")
bool(())
bool([])
bool({})
```


# Unpacking a Tuple
When we create a tuple, we normally assign values to it. This is called "packing" a tuple:

```
 fruits = ("apple", "banana", "cherry")
```

We can extract the tuple values back into variables, this is called "unpacking":

```
fruits = ("apple", "banana", "cherry")

(green, yellow, red) = fruits

print(green)
print(yellow)
print(red)
```

## Assing as a list
You can add * to the last variable name and the values will be assigned to it as a list
```
fruits = ("apple", "banana", "cherry", "strawberry, "raspberry"")
(green, yellow, *red) = fruits

print(green)
print(yellow)
print(red)
```

If the asterisk is added to another variable name thant the last, python will assign values to the variable until the number of values left matches the number of variables left:

```
fruits = ("apple", "mango", "papaya", "pineapple", "cherry")

(green, *tropic, red) = fruits

print(green)
print(tropic)
print(red)
```

## References
- [Tuples unpack](https://www.w3schools.com/python/python_tuples_unpack.asp)

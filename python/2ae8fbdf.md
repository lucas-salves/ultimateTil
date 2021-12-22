# Access tuple items

## Access tuple items by index:
```
thistuple = ("apple", "banana", "cherry")
print(thistuple[1])
```
## Note: the first item has index 0

## Negative indexing
Use negative indexing to start from the end of the tuple. Where -1 refers to the last item and -2 to the second last item etc.
```
thistuple = ("apple", "banana", "cherry")
print(thistuple[-1]) // cherry
```
## Range of indexes
Enter the values to where to start and end the range
```
thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
print(thistuple[2:5]) // cherry, orange, kiwi (index 2 is included and index 5 is not included)
```

## Return items from the beggining, but NOT included "kiwi":
```
thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
print(thistuple[:4]
```

## By leaving out the end value, the range will go on to the end:
```
thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
print(thistuple[2:])
```

## Range of negative indexes
Use negative indexes if you want to start the search range from the end of the tuple
```
thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
print(thistuple[-4:-1])
```

## Check if item exists
Use the in keyword to know if a specified item is present in a tuple:
```
thistuple = ("apple", "banana", "cherry", "orange", "kiwi", "melon", "mango")
if "apple" in thistuple:
	print("Yes, 'apple' is in the fruits tuple")
```

### References
- [Tuple access](https://www.w3schools.com/python/python_tuples_access.asp)

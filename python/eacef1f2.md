# Access items

by key name:
```
thisdict = { 
        "brand":"Ford",
        "model":"Mustang",
        "year":1964
}
x = thisdict["model"]

```

or, use the get() method:
```
x = thisdict.get("model")
```

## keys() method
Returns a list of keys in the dictionary:
```
x = thisdict.keys()
```

## values() medthod will return a list of all values in the dictionary:
```
x = thisdict.values()
```

## items() method
Will return each item in a dictionary, as tuples in a list:
//get a list of key:value pairs
```
x = thisdict.items()
```
## Check if Key exists
Use the in keyword:
```
thisdict =	{
  "brand": "Ford",
  "model": "Mustang",
  "year": 1964
}

if "model" in thisdict:
	print("Yes, 'model' is one of the keys in the thisdict dicionary")
```

### References
- [Dictionaries](https://www.w3schools.com/python/python_dictionaries_access.asp)

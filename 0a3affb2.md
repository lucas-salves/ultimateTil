# Variables

Variables do not need do be declared with any particular type and can even change the type after they have been set.
```
x = 4 # x is of type int
x = "Sally" # x is now of type str
print(x)
```

## Casting
Specifying the data type of a variable:
```
x = str(3) # x will be '3'
y = int(3) # y will be 3
z = float(3) # z will be 3.0
```

## Get the type of a variable
*type()* function returns the data type of a variable:
```
x = 5
y = "Lucas"
print(type(x))
print (type(y)
)
```
## Str: Single or double quotes?

String variables can be declared either by using single or double quotes.
```
x = "John"
## is the same as:
x = 'John'
```
## Case sensitive
Variable names are case sensitive.
```
a = 4
A = "Sally"
#A will not overwrite a. This will create two variables.
```
### References
- [W3 Schools](https://www.w3schools.com/python/python_variables.asp)

# Identation

Python use identation to determine blocks of code. Generally, in other programming languages this is done using "{ }".

The code below as expected:
```
if 5 > 2:
	print("Five is greater than two!")
```
The number of spaces is yp to you as a programmer, but it has to be at least one. As follows:
```
if 5 > 2:
 print("Five is greater than two!") 
if 5 > 2:
        print("Five is greater than two!") 
```

Remember that you have to use the same number of spaces in the same block of code:
```
if 5 > 2:
 print("Five is greater than two!")
        print("Five is greater than two!") 
```
Outputs:
```
IndentationError: unexpected indent
```

### References
- [W3 Schools] (https://www.w3schools.com/python/python_syntax.asp)

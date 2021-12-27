# Python while loops

Python has two primitive loop statements:
while and for loops

## While loops: execute a set of statements as logn as a condition is true
```
i = 1

while i < 6
	print(i)
	i += 1
```
## Continue statement

We can stop the current iteration and continue with the next:
```
i = 0
	while i < 6:
		i += 1
		if i==3:
			continue
		print(i)

```

## Else statement
We can run a block of code once when the condition no longer is true.
The exemple below print a message once the condition is false:

```
i = 1
while i < 6:
	print(i)
	i += 1
else:
	print("i is no longer less than 6")
```

### References
- [While loops](https://www.w3schools.com/python/python_while_loops.asp)

# Convert a long to int

For small values, Simple conversion is enough

```
long l = 1000000;
int i = (int) l;
```

Math.toIntExact converts the value to int and throws an exception if the value exceeds an integer:

```
Math.toIntExact(value);
```

This one truncates the value to fit in a int:
```
Long x = 100L;
int y = x.intValue();
```

### References

- [How can I convert a long to int in java](https://qastack.com.br/programming/4355303/how-can-i-convert-a-long-to-int-in-java)




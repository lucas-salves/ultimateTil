# Check if an object is a collection type

How to check if an obect is a collection:
```
public static boolean isColleciton(Object ob){
	return ob instanceof Collection ||;
}
```

How to check if a a class is a collection:

```
public static boolean isClassCollection(Class c){
	return Collection.class.isAssignableFrom(c);
}
```

### References
- [How to check if an object is a collection type in java](https://stackoverflow.com/questions/2651632/how-to-check-if-an-object-is-a-collection-type-in-java)

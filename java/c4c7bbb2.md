# Collections: List

A List is an ordered sequence of objects. List allows insertions, get items and remove objects.
Each element in a List has an index, that starts at 0.

## List vs. Set

- The same object can occur more than once in a List while in a java Set, each element can occur only once;
- The elements in a List has an order, and the elements can be iterated in that order. While Set does not guarantee order the elements kept internally.

## Implementations

Assuming List is an interface, you have to choose one of its implementations like:

* java.util.ArrayList
* java.util.LinkedList
* java.util.Vector
* java.util.Stack

ArrayList is the most commonly used.
In addition to these implementations, there are also concurrent List implementations.

## Creating a List

To create a List, you have to make an instance of one of the classes that implements the List interface:

```
List listA = new ArrayList();
List listB = new LinkedList();
List listC  = new Vector();
List listD = new Stack();
```

## Generic List

You can create a List of any Object, and restrict it to only one type:
```
List<MyObject> list = new ArrayList<MyObject>();
```
At the same time as you can create a List with no generic type specified:
```
List list = new ArrayList();

list.add(MyObject("First Obejct"));

MyObject yObject = (MyObject) list.get(0); //cas needed

```
It is necessary to cast the MyObject instance that retrieves from the List without a generyc type.

## Insert elements in a List

```
List<String> listA = new ArrayList<>();

listA.add("element 1");
listA.add("element 2");
listA.add("element 3");
```
These add() methods adds Strings to the end of the list.o

## Insert null values

List allows you to insert *null* values in it.

```
Object element = null;

List<Object> list = new ArrayList<>();

list.add(element);
```

## Insert elements at a specific index

```
list.add(0, "element4");
```

## Insert all elements from one List to another

```
List<String> listSource = new ArrayList<>();

listSource.add("123");
listSource.add("456");

List<String> listDest = new ArrayList<>();

listDest.addAll(listSource);
```
The *addAll()* method takes a Collection as parameter, so you can pass either a List or Java Set as parameter.

## Get elements from a List

Get elements by his index:

```
List<String> listA = new ArrayList<>();

listA.add("element 0");
listA.add("element 1");
listA.add("element 2");

//access via index
String element0 = listA.get(0);
String element1 = listA.get(1);
String element2 = listA.get(2);
```
## Find elements in a List

There are two methods that allows you to find elements in a List:
* indexOf():
	indexOf finds the index of the first occurrence in the List of the given element.
```
List<String> list = new ArrayList<>();

String element1 = "element 1";
String element2 = "element 2";

int index1 = list.indexOf(element1);
int index2 = list.indexOf(element2);

System.out.println("index1="+index1);
System.out.println("index2="+index2);
```

* lastIndexOf(():
	lasIndexOf finds the index of the last occurrence in the List of the given element.
```
List<String> list = new ArrayList<>();

String element1 = "element 1";
String element2 = "element 2";

list.add(element1);
list.add(element2);
list.add(element1);

int lastIndex = list.lastIndexof(element1);

System.out.println("lastindex= ="+lastIndex);
```

The output of the code above:
```
lastIndex = 2
```

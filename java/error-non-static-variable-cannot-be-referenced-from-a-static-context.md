# Error Resolution: Non-static variable cannot be referenced from a static context
> The static keyword modifies the lifecyle of a method or variable within a class. A *static* method or variable is created at the time a class is loaded. A method or variable that is not declared as *static* is created only when the class is instantiated as an object for example by using the *new* operator.
>So you need to create an instance of your class as an object and then you can access the methods and variables of the class that have not been declared with *static* modifier. Once your java program has started with the *main()* function you can then use any variables or methods that have the modifier of *static* since they exists as part of the class being loaded.
>However, those variables nad methods of the class which are outside of the *main()* method which do not have the *static* modifier can not be used until an instance of the class has been created as an object within the *main()* method. After creating the object, you can then use the variables and methods of the object. An attempt to use the variables and methods of the class which do not have the *static* modifier without going through an object of the class is caught by the Java compilar at compile time and flagged as an error.

```
import java.io.*;

class HelloWorld {
    int myInt;      // this is a class variable that is unique to each object
    static int myInt2;  // this is a class variable shared by all objects of this class

    static void main (String [] args) {
        // this is the main entry point for this Java application
        System.out.println ("Hello, World\n");
        myInt2 = 14;    // able to access the static int
        HelloWorld myWorld = new HelloWorld();
        myWorld.myInt = 32;   // able to access non-static through an object
    }
}
```
### References
[Stackoverflow Reference #1](https://stackoverflow.com/questions/2559527/non-static-variable-cannot-be-referenced-from-a-static-context)

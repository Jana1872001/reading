# Object’s life cycle
Java doesn’t allow you to allocate or deallocate memory yourself when you create or destroy objects. Java manages the memory for allocating objects and reclaiming the memory occupied byunused objects.

- The task of **reclaiming unused memory** is **taken care of by Java’s garbage collector**, which is a **low-priority thread**. **It runs periodically and frees up space occupied by unused objects.** 
- Java provides a method called **finalize**: accessible to all the classes, defined in the class java.lang.Object which is the base class of all Java classes.
- All Java classes can override the method finalize, which execute before an object is garbage collected.
- In theory, u can use this method to free up recource being used by object, although doing so isn’t recommended because its execution isn’t guaranteed to happen.

An object’s life cycle starts when it’s created and lasts until it goes out of scope or is
no longer referenced by a variable.When an object is accessible, it can be referenced by a variable and other classes can use it by calling its methods and accessing its variables.

## 3.2.1 An object is born 
The difference in variable declaration and object creation:

public class Example {
    public static void main(String[] args) {
        // Variable declaration
        Car myCar;
        
        // Object creation and assignment
        myCar = new Car();
        
        // Accessing an object method
        myCar.start();
    }
}

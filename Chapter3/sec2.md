# Object’s life cycle
Java doesn’t allow you to allocate or deallocate memory yourself when you create or destroy objects. Java manages the memory for allocating objects and reclaiming the memory occupied byunused objects.
- The task of **reclaiming unused memory** is **taken care of by Java’s garbage collector**, which is a **low-priority thread**. **It runs periodically and frees up space occupied by unused objects.** 
- Java provides a method called **finalize**: accessible to all the classes, defined in the class java.lang.Object which is the base class of all Java classes.
- 
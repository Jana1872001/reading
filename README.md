


# Wrapper classes
- Java defines a wrapper class for each of its primitive data types.
- The wrapper classes are used to wrap primitives in an object, so they can be added to a collection object.
- Wrapper classes help you write cleaner code, which is easy to read.

| # | Title |
|-----:|---------------|
|     1|[Class hierarchy of wrapper classes](README.md#class-hierarchy-of-wrapper-classes)|
|     2|[Creating objects of the wrapper classes](README.md#creating-objects-of-the-wrapper-classes)|


## Class hierarchy of wrapper classes
All the wrapper classes are immutable—classes that don’t allow changes to the state of
their instances after initialization.
> [!IMPORTANT]
> All these classes can be serialized to a stream, and their objects define a natural sort order.

## Creating objects of the wrapper classes
You can create objects of all the wrapper classes in multiple ways:
1. Assignment: By assigning a primitive to a wrapper class variable (autoboxing).
2. Constructor: By using wrapper class constructors.

3. Static methods:By calling static method of wrapper classes, like, valueOf().
> [!NOTE]
>All wrapper classes (except Character) define a constructor that
accepts a String argument representing the primitive value that needs to be
wrapped.


# **Wrapper classes**
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

## Retrieving primitive values from the wrapper classes
- The term
primitive refers to the exact primitive data type name , Ex: booleanValue().

## Parsing a string value to a primitive type
- To get a primitive data type value corresponding to a string value, you can use the static utility method parseDataType,except Character.
- Ex:  public static boolean parseBoolean(String s)
> [!NOTE]
>All these parsing methods throw NumberFormatExceptions for invalid values, except Boolean.parseBoolean();This method returns false whenever the string it parses is not equal to “true” (case-insensitive comparison).

## Difference between using the valueOf method and constructors of wrapper classes
- ValueOf method return obj of crossbonding wrraper class when it passed argument of primitive type or String. 
- These classes(Byte, Short, Integer,long -128 to 127) & (Character 0-127) define inner static classes that store objects for the primitive values.
- If you request an object of any of these classes,method Return a reference to a predefined object;Otherwise its crate new obj and return a ref of it.
- Boolean class,  cached instances are accessible directly because only two exist: static constants Boolean.TRUE and Boolean.FALSE
> [!NOTE]
>Wrapper classes Float and Double don’t cache objects for any
range of values

## Comparing objects of wrapper classes
- For equality by using the method equals or the comparison operator, that is, ==.
- **Method equals()** always compares the primitive value stored by a wrapper instance,**and ==** compares object references.
- ال autoboxing عادي بياخدهم اذا حطيت ==  "Autoboxing returns a cached  copy for applicable values." Ex:Integer i5 = 10; 
- valueOf returns a cached copy نفس الاشي 
- Constructors always create new instances.لهيك اذا بستخدم == رح يعطيني فولس لازم تستخدم .equal


> [!IMPORTANT]
> Cached instances exist for the wrapper Boolean class for the values true and false. The Character class caches instances with values from 0 to 127. Classes Byte, Short, Integer, and Long cache instances for values -127 to 128. No cached instances exist for the Float and Double wrapper classes. 


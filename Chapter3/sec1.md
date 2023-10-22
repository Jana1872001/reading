#  Scope of variables
1. Local variables (also known as method-local variables).
2. Method parameters (also known as method arguments).
3. Instance variables (also known as attributes, fields, and nonstatic variables).
4. Class variables (also known as static variables).

## Local variables
- بتعرف جوا الميثود 
 - **Defined within a method.**
 - **To store the intermediate results of a calculation.**
- The scope of a local variable depends on the location of its declaration within a method.
- defined within a loop, if-else, or switch construct or within a code block (marked with {}) is limited to these constructs.
- defined outside any of these constructs are accessible across the complete method.
##  Method parameters
- بتعرف جوا القوسين يلي قبال اسم الميثود
- **The variables that accept values in a method signature**. **Accessible only in the method that defines them**.
## Instance variables
- بتعرف جوا الكلاس
- **Instance is another name for an object.**
- An instance variable is declared within a class, outside all the method.
- It’s accessible to all the instance (or nonstatic) methods defined in a class. 
##  Class variables
**Defined by using the keyword static.**
- A class variable belongs to a class, not to individual objects of the class.
- A class variable is shared across all objects.
- You don’t even need an object to access a class variable. It can be accessed by using the name of the class.

# COMPARING THE USE OF VARIABLES IN DIFFERENT SCOPES
1. **Local variables** are defined **within a method** and are normally used to store the intermediate results of a calculation. 
2. **Method parameters** are used **to pass values to a method**. These values can be manipulated and may also be assigned to instance variables.
3. **Instance variables** are used **to store the state of an object**. These are the values that need to be accessed by multiple methods.
4. **Class variables** are used to store values that should be shared by all the objects of a class.

## * A local variable takes precedence over an instance variable defined in the class with the same names.


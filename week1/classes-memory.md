## Classes and Memory Management
**Classes**  
Class is a type of reference type and declared using the class keyword. The variable contains null until you create an instance using the new operator. Before the class keyword, you can have public, which lets anyone create an instance of the class. The class body is where behavior and data are defined and fields, properties, methods, and events are called class members.  
A class DEFINES a type of object. Classes support inheritance. When reated, you are able to inherit from another class/interface thats not defined as sealed and vice versa, it can also override class methods.  

**Constructors**  
- Its a method name should be the same as the type. Includes method name and parameter list. Does not include return type.
- Parameterless - If no constructor provided for a stuct, C# initializes each field to the default value
- Static - They are parameterless. If you do not give a static constructor to initialize static fields, C# initializes them to default values.  

**Properties**  
Provides flexibilty to read, write, compute values of a private field. They enable classes to expose a way to get and set values while they hide implementation or verification code.
- get: used to return property value
- set: used to assign a new value. Value is used to define values assigned by set  

**Garbage Collection**  
This is an automatic memory manager.
- You can develope an app without manually freeing memory
- allocates objects on heap 
- reclaims no longer used objects, clears memory, keeps memory available for the future
- gives memory safety. Objects cant use contents of another object.  
Memory has 3 states:  
1. Free - memory has no references and available
2. Reserved - memory is available but cant be used for another allocation request and cant store data until committed.
3. Committed - memory is assigned to physical storage.
This is when Garbage Collection happens:
- system has low memory
- memory used by allocated objects on head passes threshold.
- when the garbage collection method is called. Most of the time it is not needed to be called. It always runs and used rarely and for testing.
## Object-Oriented Programming(OOP)
- Encapsulation - group of related properties, methods, and other members are treated as a single unit or object.
- Inheritance - the ability to create new classes base of an existing class
- Polymophism - you can have more than one class that be can be used interchangeably even if each class uses the same props and methods differently.


**Inheritance**  
This allows you to create new classes that reuse,extend, and modify behaviors defined in other classes. The derived class can reuse the code in base without having to reimplement it. The class where members are inherited is the base class and the class that inherits those members is called derived class. A derived class only has one base class. When a class derived from another class is defined, the derived class gains all members of the base class except for the constructors and finalizers. 

**Abstract**  
Allows you to create classes and class members that are incomplete. Must be in a derived class.
Classes are declared abstract by the `abstract` keyword. Ex: `abstract public class ____`. This kind of class cant be instantiated. It provides a common definition of a base class that mult. derived classes can share. This class can override the virtual method with an abstract method.

**Polymorphism**  
Objects of a derived class can be treated as objects of a base class in places like method parameters, collections, or arrays. The this occurs, an objects declare type is not identical to the run time type. Base classes can implement virtual methods and derived classes can override them. In your source code, we can call a method of the base class and have a derived classes verion of the method to be ran. Virtual methods let you work with groups of related objects. A derived class can override a base class member if the member is declared virtual or abstract.
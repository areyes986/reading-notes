## Dependency Injection
Dependency is an object that another object requires. 
Dependency should be avoided:  
- if you want to replace a class with a different implementation, you would have to have the class modified 
- If you have a big projects with many classes depending on a dependency class, the code is scattered across the app.
- It would be hard to test.  
It helps with:  
- Usage of an interface/base class to abstracts the dependency implementation
- Registration of the dependency service container. 
- Injection into the constructor of the class that it is used. It creates an instance of dependency and disposes it when you don't need it anymore

**Solid**  
Five Principals:  
1. Single Responsibilty Principal - This is the idea that each method or class would only have ONE task. With doing so, it is easier to test the methods. If the tests fails, you will know where to look for the errors because it only looks at one thing. 
2. The Open/Close Principal - This unifies Encapsulations and Inheritances from OOP. Its the idea that methods or classes should be open for extension but closed to modification.
3. The Liskov Substitution Principal - This is the idea that an object in your app should be replaced with a type derived from it without breaking the app. If you app is expecting a base class, you should be able to pass in a derived class without any issue. It helps our code to be testable in creating substitues for dependencies that help our tests stay isolated.
4. The Interdace Segregation Principal - The idea that we should not be forced to rely on interfaces that are not used. Interfaces should be specific to the functions and needs of the client. Keep your interfaces small and specific so it is easier to test.
5. The Dependency Inversion Principal - Code should depend on abstractions not concrete implementations. 


### Unit Testing and Documentation

**Unit Testing**  
- These test isolate and exercise specific units of code. 
- You write a unit that lets you test a method in isolation.
- In the example, the tests were in their own class with an attribute of TestClass which lets VS test runner that it has tests.
- When writing tests, take it as if your test is a hypothesis and the test is an experiment. 
- We can use xUnit.net - free open source unit testing tool
- Best Practices: 
    - Arrange, act, assert
    - We should have one assert per test method.
    - Tests should handle the its set up and tear down.  
    - keep your tests simple and visible
    - If the arrange part of the test gets too hard, there is a design problem.
    - Add the new unit test execution to the build. 


**Documentation**
The documentation is important because most of the time, it is the first look to your application. You want to make sure you have all the information the user needs to start the app.
In the README.md, your documentation should have:
1. What it is.
2. Screen shots of what it looks like
3. How to use it
4. Any other relevant information

- Refer to this [link](https://github.com/jehna/readme-best-practices) for an example template for a README.


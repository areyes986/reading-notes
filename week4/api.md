## APIs
**User Secrets**
User secrets securely store private user info like API keys, client secrets, and connection string. Kind of like a .env file. This also will not push up to github.
To Enable:  
1. Select "Manager User Secrets" when you right click on your project.
    - this mimics your appsettings.json and opens up a secret.json file. What goes in it is usually a JSON key value pair.
2. In your .csproj, make sure you have the line of `<UserSecretsId>ID goes here</UserSecretsId>` inside.
3. Now we need to tell our startup that we are using a secret.json file.
    - we replace the default config with 

**Intro into APIs**
What is Web API?
- http service (application layer protocol)
- they are accessed across the interwebs
- logic/data accessible over http
To create:
- set up mvc, create a class to derive from the controller base, implement your actions

Handling HTTP requests:
- Server listens for the requests
- middleware is invoked for the requests
- MVC routes requests to a controller and action
- responses go back to the middleware

Model Binding/Validation:
- allows you get request and bind it to your actions

Action Results:
- used to prduce reponses
- Return IActionResult
- there are also helper extension methods on the controller base



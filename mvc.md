## Model-View-Controller (MVC)

This is a framework for making apps and APIs. User requests are routed to a controller that is responsible for working with the model to perform user actions and get results of queries. Controller chooses the view to show the user and gives it any model data required.
**Model:**  
Classes that represent data of the application. Model is the state of the application. Business logic is encapsulated also with other implementation logic for persisting the state of the application. Model objects retrieves and stores model state in database. 
**View:**  
View presents content to the user interface. Displays information. There is minimal logic with views really only to present content.  
**Controller:**  
Initial entry point. Classes that handle the browser requests.  Selects which model types to work with. This handles user interaction, works with model and selects a view to render. Its handles and responds to the user's input. 


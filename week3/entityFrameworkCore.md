## Entity Framework Core

This is an open source cross platform version of Entity Framework. It serves as an object-relationship mapper that lets us use the database.  
Model:   
Data is accessed using a model which had entity classes and a contect object that represents a session with the database. This allows you to query and save data. To do that, you make a model from the database and code out a model to match.  
Query:  
Instances of the classes are retrieved from querying from the database  

**Model Validation**  
*Model State:*  
This represents errors from two subsystems- model bniding and model validation. In model binding, it generally has data conversion errors. Model validation happens after the model binding. It reports errors where the data doesnt conform to business rules. These both happen before the execution of a controller action or Razor Pages hander method.  
*Rerun Validation:*     
You want to repeat validation manually. To retun a validation use the `TryValidateModel` method.  
*Validation Attributes:*    
This will let you specify the rules for the model's properties. There are many built-in validation attributes some commone ones are `[Phone]` which validates that the prop has a telephone format, `[Range0, 999.99]` which makes sure the prop value is in the specified ranged, or `[Required]` which validated that the field isn't null. These also help you specify the error messages you want to display in invalid input.  
*Custom Attributes*  
These are for when the built-in validation attributes can't handle certain scenarios. You would create a class that inherits from `ValidationAttribute` then override the `IsValid` method which accepts an object named value. 










## Components

View Components allow us to create reusable components. Similar to partial views. 
View components work with Razor Pages and from the article it: 
- renders a chunk rather than an entire response
-  has parameters and business logic
- is invoked from a layout page.  

They are used if you have reusable rendering logic thats too complex for a partial view. It supports dependency injection and doesn't take part in controllers. Filters cannot be used.  The file name for the view will typically be `Default.cshtml` and it is recommended to use the file path of `/Views/Shared/Components/{View Component Name}/{View Name}`
They consist of two parts:  
1. The class, derived from ViewComponent. Many devs use the methods/props deriving from the ViewComponent.
2. The result is returns, the view.

**View component methods**  
`InvokeAsync` method is where the view component defines its logic. It usually returns a `Task<IViewComponentResult>`, if it is synchronous, `returns IViewComponentResult`.  
Does not directly handle requests and initializes the model and passes it to a view in a `view` method. They are not reachable as an HTTP endpoint and is invoked from code.


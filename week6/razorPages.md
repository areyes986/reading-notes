## Razor Pages

Razor pages are enabled in the Startup.cs. In the cshtml, there is a `@page` directive that makes the file into an MVC action. It allows it to handle the request without going through a controller. It must be the first razor directive on the page and it affects the behavior of other constructs. Runtime looks for the razor pages by default and index is also defaulted page when a url doesn't include one.  
PageModel class is in the same namespace as the page. This allows separation of logic and the presentation. This makes it easier to do unit testing and dependency injections.  
`OnPostAsync` runs on post requests(on a form) and looks similar to a controller code. Common handler methods are an HTTP verb are `OnGet`, initialize state needed for page and `OnPost`, handle form submissions.  
**MVC vs Razor Pages**

**MVC**  
1. User requests /home/index
2. Asp.Net routes requests to controller action
3. View Engine locates, renders, and returns a view
4. User sees view

**Razor Pages**  
1. User requests /contact
2. routes to request to razor page
3. View Engine renders and returns a view
4. User sees view
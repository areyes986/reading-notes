## Views and Azure Deployment
Scripts and style sheets are used frequently by many pages within an app and these elements are defined i na layout file. Layouts reduce duplicate code in views. The default name for this file is `_Layout.cshtml`  Razor views has a layout property. When given a partial name, the view engine searches for the layout file.  
A Layout can also reference more sections by calling `RenderSection`. This helps organize where parge elements should be placed.

**Tag Helpers**  
Tag Helps help create and render HTML elements on Razor files. It can help with making forms, links, etc. Though tag helpers do not replace HTML helpers and there's not a tag helper for each html helper. They provide an HTML-friendly development experience. People with experience with HTML,css, and javascript dont have to know C# syntax to know whats going on. It also has great IntelliSense. The article says that devs work better with Tag Helpers rather than C# razor markup. Tag helps make you more productive and have better code using info only on the server. 

**Partials Views**  
This a a Razor markup file that renders HTML. Partial Views are used for an MVC app where markup files are called views. We use partial views to:  
- to make large markup files into smaller ones.
- Reduces duplication of common markup with each of the files
But shouldn't be used to maintain common layout elements that should be specified in `_Layout.cdhtml`. And also shouldn't be used with complex rendering logic.

**View Model**  
The view handles the apps presentaion and user interactions and is usually is an HTML template usings a Razor markup. Views are usually grouped into folders name for each controller. Benefits of using views are, it helps to maintain the app with it being organized, it is loosely coupled which means that we can build off of it without touching other important components of the app, because it is organized, there will be less duplicate code.

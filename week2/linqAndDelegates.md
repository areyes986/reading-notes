## LINQ & Delegates
**Language Integrated Query(LINQ)**  
This is a set of technologies on the integration of query capabilities. It has a consistent model for working with data across all kinds of sources and formats and is always working with objects. Usually queries against data are strings without type checking but for LINQ, a query is a first class language construct like classes, methods, and events. There is query syntax which allows you to perform filtering, ordering, and grouping with minimum code. Queries are not executed until you iterate over query variables.  
3 Parts of Query Operation:  
1. Open the data source
    - If a data source is not in memory already as a queryable type, LINQ must represent it. LINQ -> SQL, you create an object relational mapping manually or by using tools in Visual Studio. 
2. Create the query
3. Execute the query

**LINQ Query Operations**
- Obtain a Data Source
    - First step is to specify the data source. To do this, the `from` clause comes first to introduce the data source and range variable. Range variable is like the iteration in a foreach loop but no iteration actually occurs in a query expression. When executed, the range variable will serve as a reference to each element. 
- Filtering
    - It is common to apply a filter in the form of a boolean expression. The query will return only elements where the expression is true. You get the result by using the `where` clause. 
- Ordering
    - Used to sort the returned data. We do this with the `orderby` clause which will sort elements in the returned sequence. 
- Grouping
    - The `group` clause helps you group results based on a key that you specify. When a query is ended, the results take form of a list of lists. Each element in the list are objects that has a key. To iterate over, you must use a nested foreach loop. Outer loops iterated over group and innter over each group members.
- Joining 
    - help created associations betweem sequences that are modedled in data sources
- Selecting(Projections)
    - `select` gives you the results of a query and tells you the shape.type of the elements.

### Exception Handling

**Try/Catch**  
To use them, you put code statements in a _try_ block for ones that throw an exception. It specifies code that is subject to error-handling/cleanup code and must be followed by a _catch_ and/or a _finally._ Statements to handle the exception is a _catch_ block that happens when the _try_ has an error and includes the exception type(either `.Exception` or `System.Exception`)
 and contains additional statements if needed to handle that exception type. The _finally_ block happens after execution leaves the _try._Exceptions not handled by catch are caught using CLR.  
Results that may occur if so and depending on the CLR config:  debug dialog appears, the program doesn't execute with the dialog box with exception info shows up, and error will print out.  

**Exception Handling**
Statements are program instructions and followed by in sequence. Ex. of C# statements:  
_Selection Statements:_ if, else, switch, case  
_Iteration:_ do, for, foreach, in, while  
_Jump:_ break, continue, default, goto, return, yield.  
For more statement examples refer to the [reading.](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/statement-keywords)
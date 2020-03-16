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

**Therac-25**
This was a computer controlled radiation therapy machine. This machined was involved in 6 accidents from 1985-1987. Patients recieved massive amounts of radiation. The programming errors and overconfidence on the engineers resulted in bugs and is what caused the radiation dosage to be 100x greater than usual. This showed the dangers of software control of safety-critical systems. Some causes included:  
- the code was not independently reviewed
- When the system noticed something wrong, the only thing displayed was "Malfunction" with a number from 1-64. However the manual didn't explain what these error codes meant. The user can simply press the P key to override the warning.
- The program was never tested until the machine was already at the hospital.

**Ariane 5**  
This was a rocket designed by the French goverment space agency. It was to deliver payloads into low Earth orbit. It had a dual-launch capability, up to 2 large communication satellites can be mounted. 3 smaller sattelites were possible depending on the size.




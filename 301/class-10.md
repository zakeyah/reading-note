## What is call stack?

- Call stack is what a program uses to keep track of method calls. The call stack is made up of stack frames—one for each method call.
## What's usually stored in a stack?

- Local variables
- Arguments passed into the method
- Information about the caller's stack frame
- The return address—what the program should do after the function returns.

**Syntax errors**
I know it's in the name of the errors, but like it says itself, this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

**Range errors**
Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

**Type errors**
this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.

The fix is simple, just make sure that method exists before trying to access it, either by creating method or by checking for undefined.

## Debugging:

To debug your JS code, the easiest and maybe the most common way its to simply `console.log()` the variables you want to check or, by using chrome developer tools, open your page with your JS code *(press cmd+o in macOS or Ctrl+o in Windows)* and choose your file to debug, click the line you wanna debug and refresh your page again (F5).
The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.
You can also add conditional breakpoints by right-clicking a previous set breakpoint, which will make your program stop at that point only if a condition is met, this is awesome for when you want to debug huge cycles for specific values. In this example the breakpoint will point stop when the index reaches 40.

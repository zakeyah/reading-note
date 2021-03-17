![](https://image.slidesharecdn.com/debugging-javascript-web-141030080414-conversion-gate02/95/debugging-javascript-1-638.jpg?cb=1415345877)

## When you are writing JavaScript, do not expect to write it perfectly the first time. Programming is like problem solving: you are given a puzzle and not only do you have to solve it, but you also need to create the instructions that allow the computer to solve it. too. When writing a long script, nobody gets everything right in their first attempt. The error messages that a browser gives look cryptic at first, but they can help you determine what went wrong in your JavaScript and how to fix it. In this chapter you will learn about :
-	THE CONSOLE & DEV TOOLS
-	COMMON PROBLEMS
-	HANDLING ERRORS

## ORDER OF EXECUTION
To find the source of an error, it helps to know how scripts are processed.
The order in which statements are executed can be complex; some tasks
cannot complete until another statement or function has been run.

## EXECUTION CONTEXT
& HOISTING
Each time a script enters a new execution context, there are two phases
of activity:
1: PREPARE
• The new scope is created
• Variables, functions, and arguments are created
• The value of the this keyword is determined

2: EXECUTE
• Now it can assign values to variables
• Reference functions and run their code
• Execute statements

## UNDERSTANDING ERRORS
If a JavaScript statement generates an error, then it throws an exception.
At that point, the interpreter stops and looks for exception-handl ing code.
If you are anticipating that something in your code
may cause an error, you can use a set of statements
to handle the error

## ERROR OBJECTS
Error objects can help you find where your mistakes are
and browsers have tools to help you read them

### Debugging is the process of finding errors. It involves a
### process of deduction

### JavaScript has 7 different types of errors. Each creates
### its own error object, which can tell you its line number
### and gives a description of the error. 

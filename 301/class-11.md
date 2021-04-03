## What is EJS?

 - EJS is a simple templating language that lets you generate HTML markup with plain JavaScript. ... It's just plain JavaScript.

 ## When to use EJS

 - EJS is mostly useful whenever you have to output html with a lot of javascript, if you're dealing with generating dynamic contents or offering something that has to do with real time updates. 

 ## Why EJS?

 - There are several templating systems out there with their merits and demerits, I personally use EJS because of its simplicity in syntax and logic. Its also very easy to set up.

 ## Understanding The Syntax — The Tags

 While using express, there are 4 major tags that you will need to understand;

1. <% %>: This is used to embed javascript codes that do return outputs e.g control flow, conditionals, variable declaration, include statements.

2. <%= %>: Used to embed code that is supposed to return and output the result of an expression/computation to the view (page) at run-time.
 
3. <%- %> : This takes a string and outputs it's unescaped value to the view.

4. <%# %>: Used to include comments in files.

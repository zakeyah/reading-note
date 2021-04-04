# EJS Partials
## Partials come in handy when you want to reuse the same HTML across multiple views. Think of partials as functions, they make large websites easier to maintain as you don't have to go and change a piece of text in every page it appears in. Instead, you define that reusable bundle of code in a file andinclude it wherever you need it.




## the same navigation bar and footer appear in both the home and other pages. This makes them perfect candidates for partials!Under the views/partials/ directory create a file callednavbar.ejs which will contain only the HTML for the navigation bar.



 ## we have our partials defined, we can use them in our home.ejs and post.ejs templates! In EJS, any JavaScript or non-HTML syntax you include in your templates is always surrounded by <% %> delimiters

## including nav and footre
# WHAT IS A FUNCTION? 
### Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements). 

## declaring a function in javascript
![](data:image/jpeg;base64,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)

## calling function 
### It can be used to invoke (call) a method with an owner object as an argument (parameter).
say haloo ();

## declaring function that need information
function getarea (width , height){
    return width *  height ;
}
 ## getting a single value out of function
 
function calculate area (width , height){
   var area = width +  height
    return area ;
}
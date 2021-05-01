# Node Ecosystem, TDD, CI/CD

## Array.map()

- It iterates over an array and runs a callback function for each element.
- It returns a new array with the same length.
- No need to push to the new array.
- It doesn't affect the original array.

## Array.reduce()
- It takes 3 parameters (accumulator, value, index ).
- It iterates over an array and returns the result of the accumulator.
- The accumulator can be an initial empty object, variable, string, or array.
- There is an initial value that represents the value of the accumulator in the first iteration.

## superagent()
*With normal Promise .then() syntax*
```javascript
function getData (req,res){
    superagent.get(url)
    .then(data=>{
        console.log(data.body)
    })
    .catch(err=>console.error(err))
}
```

 *With async / await syntax*
 ```javascript
async function getData (req,res){
    try{
    let data = await superagent.get(url);
    console.log(data.body)
    }catch(err=>console.error(err))
}
```
## Explain promises
 ### promise is telling the code to NOT run until the function who called the promise is fully run because this function need time to fully run
*There are three states of Promise*

- pending
- Resolved
- Rejected
Pending which mean that the code need some amount of time to get done, if the time is fulfilled then it's maybe Resolved or Rejected, it will be resolved if the there is no errors occurred for any reason and Rejected if there is any error or anything didn't meet the requirements;

## Are all callback functions considered to be Asynchronous? Why or Why Not?

### no , not all callback are Asynchronous like Array.map() or Array.reduce() It iterates over an array and runs a callback function for each element without need  Asynchronous.
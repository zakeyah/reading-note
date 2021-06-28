# Redux - Asynchronous Actions

### How granular should your reducers be?
- There should be a separate reducer function for each slice of data. They are combined before being put into the store.

### Pro or Con – multiple reducers can “fire” when a commonly named action is dispatched
- When your reducer has finished and returned the new application state, asyncDispatch will trigger store. dispatch with whatever action you give to it. 

### Name a strategy for preventing the above
- Using switch

# Term

|    |  |
| ----------- | ----------- |
| store     |  A store is a state container which holds the application's state. Redux can have only a single store in your application. Whenever a store is created in Redux, you need to specify the reducer.This can only be changed when actions are dispatched to the store.    |
| combined reducers      |   Helper function turns an object whose values are different reducing functions into a single reducing function you can pass to createStore.   |

## Redux Thunk
- With a plain basic Redux store, you can only do simple synchronous updates by dispatching an action. Middleware extends the store's abilities, and lets you write async logic that interacts with the store.

Thunks are the recommended middleware for basic Redux side effects logic, including complex synchronous logic that needs access to the store, and simple async logic like AJAX requests.

- Redux Thunk is middleware that allows you to return functions, rather than just actions, within Redux. This allows for delayed actions, including working with promises. One of the main use cases for this middleware is for handling actions that might not be synchronous, for example, using axios to send a GET request.

- The most common use case for Redux Thunk is for communicating asynchronously with an external API to retrieve or save data. Redux Thunk makes it easy to dispatch actions that follow the lifecycle of a request to an external API.

### Some common kinds of side effects are things like
- Logging a value to the console
- Saving a file
- Setting an async timer
- Making an AJAX HTTP request
- Modifying some state that exists outside of a function, or mutating arguments to a function
- Generating random numbers or unique random IDs (such as Math. random() or Date.now())


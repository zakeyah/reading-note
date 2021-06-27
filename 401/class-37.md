# Redux - Combined Reducers

### Why choose Redux instead of the Context API for global state?

- Redux is the industry standard for managing state of large applications. It is more optimized for larger projects, because the context API re-renders more often.

### What is the purpose of a reducer?
- We need reducers to tell the application how to change state in response to an action. The action does not do anything except describe what happened and it is up to the reducer to respond to this.

### What does an action contain?
- An action contains a action type and whatever payload you want it to have.

### Why do we need to copy the state in a reducer?
- The reducer needs to be a pure function without any side-effects. It should only take in an action and return the new state.

# Term

|    |  |
| ----------- | ----------- |
| immutable state      |  This allows the state to only change when absolutely necessary to make React apps perform as well as possible.    |
| time travel in redux      |  The Redux DevTools records dispatched actions and the state of the Redux store at every point in time. This makes it possible to inspect the state and travel back in time to a previous application state without reloading the page or restarting the app.   |
| action creator      |  Actions send data from your application to your store, and are the only source of information for the store. An action creator is a function that creates an action.  |
| reducer      |   is a pure function that takes the current state and an action, and returns the next state.   |
| dispatch      |  Dispatch is the act of sending something somewhere.its the only way to update the state is to call store.dispatch() and pass in an action object   |

### combineReducers 
- The most common state shape for a Redux app is a plain Javascript object containing “slices” of domain-specific data at each top-level key. Similarly, the most common approach to writing reducer logic for that state shape is to have “slice reducer” functions, each with the same (state, action) signature, and each responsible for managing all updates to that specific slice of state. Multiple slice reducers can respond to the same action, independently update their own slice as needed, and the updated slices are combined into the new state object.

### State Shape
- There are two ways to define the initial shape and contents of your store’s state. First, the createStore function can take preloadedState as its second argument. This is primarily intended for initializing the store with state that was previously persisted elsewhere, such as the browser’s localStorage. The other way is for the root reducer to return the initial state value when the state argument is undefined. These two approaches are described in more detail in Initializing State, but there are some additional concerns to be aware of when using combineReducers.
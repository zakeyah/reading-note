# Redux - Additional Topics

## What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?
- The best practice is to wrap the opening preloaded in useEffect. 

### When using a thunk/async action that dispatches the actual action, which do you export from your reducer?
- the async function that will handle the data. 

# Term

|    |  |
| ----------- | ----------- |
| middleware     |  Redux middleware provides a third-party extension point between dispatching an action, and the moment it reaches the reducer. People use Redux middleware for logging, crash reporting, talking to an asynchronous API, routing, and more.    |
| thunk      |   Thunk is a redux middleware that allows you to do async functions in conjunction with Redux.   |

## Redux Toolkit (RTK)
- Redux Toolkit makes it easier to write good Redux applications and speeds up development, by baking in our recommended best practices, providing good default behaviors, catching mistakes, and allowing you to write simpler code.

## Redux Toolkit includes:

-  `configureStore()` function with simplified configuration options. It can automatically combine your slice reducers, adds whatever Redux middleware you supply, includes redux-thunk by default, and enables use of the Redux DevTools Extension.

- `createReducer()` utility that lets you supply a lookup table of action types to case reducer functions, rather than writing switch statements.

- `createAction()`=> utility that returns an action creator function for the given action type string. The function itself has toString() defined, so that it can be used in place of the type constant.

-  `createSlice()` function that accepts a set of reducer functions, a slice name, and an initial state value, and automatically generates a slice reducer with corresponding action creators and action types.

- `createSelector` utility from the Reselect library, re-exported for ease of use.

## RTK Query#
- *RTK Query* is provided as an optional addon within the `@reduxjs/toolkit` package. It is purpose-built to solve the use case of data fetching and caching, supplying a compact, but powerful toolset to define an API interface layer for your app. It is intended to simplify common cases for loading data in a web application, eliminating the need to hand-write data fetching & caching logic yourself.
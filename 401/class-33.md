# Context API

## Describe use cases for `useMemo()` and `useReducer()`?
- `useReducer()` is useful when you need to use complex state logic, when you have multiple sub values, or when the next state depends on the previous state.

- `useMemo()` runs during rendering, and it will only recompute the memoized value when one of its dependents has changed. This is an optimized way to avoid calculations every re-render.

## Why do custom hooks need the use prefix?
- so react can know it’s custom hook.Without this, it looks just like a regular function.

## What do custom hooks usually do?
- They give functionality that can be used across multiple components.

## Using any list of custom hooks, research and name one that you think will be useful in your applications
- change a value between true and false in flag function

## Describe how a hook that fetches API data might work
An API fetching hook would take in a url and any info necessary for the request and return the results of the API call.

# Term

|    |  |
| ----------- | ----------- |
| reducer      |  is a function that determines changes to an application’s state. It uses the action it receives to determine this change.    |


## Context
- is primarily used when some data needs to be accessible by many components at different nesting levels. Apply it sparingly because it makes component reuse more difficult. If you only want to avoid passing some props through many levels, component composition is often a simpler solution than context.

- Using context, we can avoid passing props through intermediate element .

- Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language .



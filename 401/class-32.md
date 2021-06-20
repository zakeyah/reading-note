# Custom Hooks

## What does a component’s lifecycle refer to?
- Lifecycle of a component is series of methods that are invoked in different stages of the component's existence. Lifecycle methods give ways to interact with component logic before/during/after being used in the DOM.
## Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect?
- because it fires a memoized version of the callback only if one of it's dependants has changed. This makes it faster and more efficient.

## Why are functional components preferred over class components?
- Functional components are much easier to read and test, they have less code, easier to separate container and presentational components.

## What is wrong with the following code?
- UseEffect can't be inside for loop.

# Term

|    |  |
| ----------- | ----------- |
| state hook      | `useState()`, similar to `this.setState()` in a class except it doesn't merge the old and new state together. The only argument to `useState()` is the initial state. Allows us to add a state powered variable to our application.        |
| effect hook |  By using this Hook, you tell React that your component needs to do something after render. React will remember the function you passed (we’ll refer to it as our “effect”), and call it later after performing the DOM updates.  |
| reducer hook |  s used to store and update states, just like the useState Hook. It accepts a reducer function as its first parameter and the initial state as the second.   |


### react custom hooks
- When we want to share logic between two JavaScript functions, we extract it to a third function. Both components and Hooks are functions, so this works for them too!

*A custom Hook is a JavaScript function whose name starts with ”use” and that may call other Hooks.*

- Unlike a React component, a custom Hook doesn’t need to have a specific signature. We can decide what it takes as arguments, and what, if anything, it should return. In other words, it’s just like a normal function. Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it.

#### async hooks
- Cannot use async keyword with useEffect will create race condition
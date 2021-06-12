# Component Based UI

### Name 5 Javascript UI Frameworks (other than React)?
- Angular
- Vue
- Ember
- Svelte
- Sencha

### What’s the difference between a framework and a library?
- The technical difference between a framework and library lies in a term called inversion of control. When you use a library, you are in charge of the flow of the application. You are choosing when and where to call the library. When you use a framework, the framework is in charge of the flow.

# Term

|    |  |
| ----------- | ----------- |
| Rendering | processing any piece of code that we have written and showing the result of it on the browser.        |
| Templates      | its feature programming language that allows functions and classes to operate with generic types. This allows a function or class to work on many different data types without being rewritten for each one.        |
| State      | object that holds some information that may change over the lifetime of the component .        |


*React is an open-source, front end, JavaScript library for building user interfaces or UI components. It is maintained by Facebook and a community of individual developers and companies. React can be used as a base in the development of single-page or mobile applications.*

## JSX
### JSX stands for JavaScript XML.
- JSX it is a syntax extension to JavaScript.
- JSX allows us to write HTML elements in JavaScript and place them in the DOM without any createElement() and/or appendChild() methods.
- React embraces the fact that rendering logic is inherently coupled with other UI logic: how events are handled, how the state changes over time, and how the data is prepared for display .


### Rendering Elements
React Only Updates What’s Necessary
React DOM compares the element and its children to the previous one, and only applies the DOM updates necessary to bring the DOM to the desired state.


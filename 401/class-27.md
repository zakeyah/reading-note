# Props and State

### Does a deployed React application require a server?
- No, it doesn't.
### Why do we prefer to test a React application at the behavior rather than the unit level?
- When it comes to React components you want to check how your component is rendered and if all props you pass to the component influence the behavior of your component as expected.

### What does npm run build do?
- When you're ready to deploy to production, running npm run build will create an optimized build of your app in the build folder .

### Describe the actual composition / architecture of a React application .
- React doesn't have a certain architecture that you have to follow.

# Term

|    |  |
| ----------- | ----------- |
| BDD |  behavior driven development, a branch of Test Driven Development (TDD), which uses human-readable descriptions of software user requirements as the basis for software tests   |
| Acceptance Tests      | is a term used in agile software development methodologies, particularly extreme programming, referring to the functional testing of a user story by the software development team during the implementation phase.        |
| mounting      | Mounting is the phase in which our React component mounts on the DOM. This method is called just before a component mounts on the DOM or the render method is called. After this method, the component gets mounted.        |
| build      | It saves you from time-consuming setup and configuration. You simply run one command and create react app sets up the tools you need to start your React project.      |


## React SetState
- React components with state render UI based on that state. When the state of components changes, so does the component UI.

- setState() is the only legitimate way to update state after the initial state setup.

- Think of setState() as a request rather than an immediate command to update the component. For better perceived performance, React may delay it, and then update several components in a single pass. React does not guarantee that the state changes are applied immediately.

##  Handling event
 ### Handling events with React elements is very similar to handling events on DOM elements. There are some syntax differences:

- React events are named using camelCase, rather than lowercase.
- With JSX you pass a function as the event handler, rather than a string.

## React Forms
- Just like in HTML, React uses forms to allow users to interact with the web page

### Handling Forms

- Handling forms is about how you handle the data when it changes value or gets submitted.

- In React, form data is usually handled by the components.

- When the data is handled by the components, all the data is stored in the component state

## React State:

- React components has a built-in state object.

- The state object is where you store property values that belongs to the component.

- When the state object changes, the component re-renders.

## React Lifecycle
*Lifecycle of Components*

- Each component in React has a lifecycle which you can monitor and manipulate during its three main phases.

- The three phases are: Mounting, Updating, and Unmounting.


*React has four built-in methods that gets called, in this order, when mounting a component:*

- constructor()
- getDerivedStateFromProps()
- render()
- componentDidMount()
- The render() method is required and will always be called, the others are optional and will be called if you define them.

## React Props
- React Props are like function arguments in JavaScript and attributes in HTML.
# Component Composition

### Can a parent component access the state of a child component?
- In React we can access the child's state using Refs. we will assign a Refs for the child component in the parent component. then using Refs we can access the child's state.


### What can be passed along in a prop variable?
- data , array , functions 

### How can a child component “know” the state of another component?
- component props: What we pass from the parent component to the child component to can access them.

- component state: Its a object specific to the one components.

- application state: Represent all the state of the application.


# Term

|    |  |
| ----------- | ----------- |
| component props |  Props are arguments passed into React components. Props are passed to components via HTML attributes.   |
| component state      | an object that determines how that component renders & behaves. In other words, “state” is what allows you to create components that are dynamic and interactive.        |
| application state     | represents the totality of everything necessary to keep your application running .       |

## react basics recap

- Higher-Order Components: The AuthWrapper component lifts all authentication logic into a unifying component. All it does is take a prop called isLoggedIn and returns the WrappedComponent or a paragraph tag based on whether or not that prop is true or false.

- As you can see, HOCs are extremely useful because they let us reuse code and remove bloat.

- React State and setState():

- This method takes an object and merges it into the current state. On top of this, there are a few things you should also know about it.

- First, setState is asynchronous. This means state won’t update exactly after you call setState and this can lead to some aggravating behavior which we will hopefully now be able to avoid!

- React Context: The React context API allows you to create global context objects that can be given to any component you make. This allows you to share data without having to pass props down all the way through the DOM tree.

- Stay up to date with React: It’s simply keeping up with the latest releases of React. React has made some serious changes lately and it’s only going to continue to grow and develop.

## React’s props.children
- props.children is a special prop, automatically passed to every component, that can be used to render the content included between the opening and closing tags when invoking a component

## Composition vs Inheritance
- Inheritance

*Those familiar with Object Oriented Programming are well aware of Inheritance and use it on a regular basis. When a child class derives properties from it’s parent class, we call it inheritance. There are variety of use-cases where inheritance can be useful.*

- Composition

*Composition is also a familiar concept in Object Oriented Programming. Instead of inheriting properties from a base class, it describes a class that can reference one or more objects of another class as instances.*
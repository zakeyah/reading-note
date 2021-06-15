# Routing
## Do child components have direct access to props/state from the parent?
- We can see there is no way to pass props from a child component to a parent component. However, we can always pass around functions from the parent to child component. The child component can then make use of these functions .

## When a component “wraps” another component, how does the child component’s output get rendered?
-By add the component as a props.children

## Can a component, such as <Content />, which is a child also be used as a standalone component elsewhere in the application?
- yes

## What trick can a parent use to share all props with it’s children ?
- pass all the props with the spread operator: <ChildComponent {...props}>

# Term

|    |  |
| ----------- | ----------- |
| props.children |  allows to pass a component or markup as a props to children.   |
| composition      | is a natural pattern of the component model. It's how we build components from other components, of varying complexity and specialization through props. Depending on how generalized these.        |


## React Router
- install react-router-dom.
-  router types : -BrowserRouter -HashRouter
- The *BrowserRouter* should be used when you have a server that will handle dynamic requests .
- The *HashRouter* should be used for static websites .
- if the website will be hosted on a server that only serves static files, then the *HashRouter* is the choise .
- A *Route* expects a path prop, which is a string that describes the pathname that the route matches .
- React Router uses the path-to-regexp package to determine if a route element’s path prop matches the current location. 

## Hooks
-React Router ships with a few hooks that let you access the state of the router and perform navigation from inside your components.

- useHistory

The useHistory hook gives you access to the history instance that you may use to navigate.

- useLocation

The useLocation hook returns the location object that represents the current URL. You can think about it like a useState that returns a new location whenever the URL changes.

- useParams

useParams returns an object of key/value pairs of URL parameters. Use it to access match.params of the current route.

- useRouteMatch
attempts to match the current URL in the same way that a *Route* would
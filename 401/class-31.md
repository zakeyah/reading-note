# Hooks API

## Why do we not need more .html pages in a multi-page React app?
- in React we need one HTML page and we will render the components for the route we want, so same page but just changing the components

## If we wanted a component to show up on every page, where would we put it and why?
- Inside the `<BrowserRouter />`, outside a `<Route />`, because we need to wrap the whole application with `<BrowserRouter />`, and outside `<Route />` because we only use `<Route />` inside of `<Switch />` to let the app decide which component to render based on the url.

## What does props.children contain?
- contain what inside the component <> </>
# Term

|    |  |
| ----------- | ----------- |
| composition      | is a natural pattern of the component model. It's how we build components from other components, of varying complexity and specialization through props. Depending on how generalized these.        |
| Children / Child Components |  components that are placed or defined inside of other components.   |
| Hash Routing |  is using the anchor part of the URL to simulate different content.   |
| Link Routing |  Provides declarative, accessible navigation around the application.   |

## React Hooks

- hooks are functions that let you “hook into” React state and lifecycle features from function components. Hooks don’t work inside classes — they let you use React without classes.

- Hooks let us organize the logic inside a component into reusable isolated units: Hooks apply the React philosophy inside a component, rather than just between the components.

- If you write a function component and realize you need to add some state to it, previously you had to convert it to a class. Now you can use a Hook inside the existing function component.

## Effect Hook
- You’ve likely performed data fetching, subscriptions, or manually changing the DOM from React components before. We call these operations “side effects” (or “effects” for short) because they can affect other components and can’t be done during rendering.
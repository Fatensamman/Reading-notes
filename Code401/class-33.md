# Context API

## Describe use cases for useMemo() and useReducer()

- useMeme eturns a memoized value.Pass a “create” function and an array of dependencies. useMemo will only recompute the memoized value when one of the dependencies has changed. This optimization helps to avoid expensive calculations on every render.

- useReducer is an alternative to useState. Accepts a reducer of type (state, action) => newState, and returns the current state paired with a dispatch method.

## Why do custom hooks need the use prefix?

 Its name should always start with use so that you can tell at a glance that the rules of Hooks apply to it.

## What do custom hooks usually do?

- A custom Hook is a JavaScript function whose name starts with ”use” and that may call other Hooks.
- Custom Hooks are a convention that naturally follows from the design of Hooks, rather than a React feature.
- Custom Hooks offer the flexibility of sharing logic that wasn’t possible in React components before. You can write custom Hooks that cover a wide range of use cases like form handling, animation, declarative subscriptions, timers, and probably many more we haven’t considered.

## Using any list of custom hooks, research and name one that you think will be useful in your applications

https://github.com/streamich/react-use This page has as a list of hooks that seem very useful like tracking location of user, track clicks, scolls, typing, screen orientation... 


## Describe how a hook that fetches API data might work



## Term

| Term | Definition |
| ------- | ----------------- |
| reducer |is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. It also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.|

## Materials 

[context api](https://reactjs.org/docs/context.html)

[hooks and context example](https://medium.com/swlh/snackbars-in-react-an-exercise-in-hooks-and-context-299b43fd2a2b)

[react context links](https://github.com/diegohaz/awesome-react-context)

[awesome react hooks](https://github.com/rehooks/awesome-react-hooks)
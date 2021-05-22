# Redux - Combined Reducers

## Why choose Redux instead of the Context API for global state?

- Redux is a predictable state container for JavaScript apps.
- Context provides a way to pass data through the component tree without having to pass props down manually at every level.

[React Context API vs Redux — the eternal dichotomy](https://blog.softwaremill.com/react-context-api-vs-redux-the-eternal-dichotomy-24639907fc98)

## What is the purpose of a reducer?

Reducers specify how the application's state changes in response to actions sent to the store. Remember that actions only describe what happened, but don't describe how the application's state changes.

## What does an action contain?

Actions are payloads of information that send data from your application to your store. They are the only source of information for the store. You send them to the store using store.dispatch().

Actions are plain JavaScript objects. Actions must have a type property that indicates the type of action being performed. Types should typically be defined as string constants. Once your app is large enough, you may want to move them into a separate module.

## Why do we need to copy the state in a reducer?

Redux's state is readonly, so you can't mutate the array and return it. You must send a copy with the mutations otherwise you break the pattern

## Term

| Term | Definition |
| ------- | ----------------- |
|immutable state|Immutability can bring increased performance to your app, and leads to simpler programming and debugging, as data that never changes is easier to reason about than data that is free to be changed arbitrarily throughout your app. In particular, immutability in the context of a Web app enables sophisticated change detection techniques to be implemented simply and cheaply, ensuring the computationally expensive process of updating the DOM occurs only when it absolutely has to (a cornerstone of React’s performance improvements over other libraries).|
|time travel in redux|Redux DevTools records dispatched actions and the state of the Redux store at every point in time. This makes it possible to inspect the state and travel back in time to a previous application state without reloading the page or restarting the app.|
|action creator|functions that create actions. In Redux, action creators simply return an action |
|reducer|Reducers specify how the application's state changes in response to actions sent to the store. Remember that actions only describe what happened, but don't describe how the application's state changes.|
|dispatch|dispatch is a function of the Redux store. You call store.dispatch to dispatch an action. This is the only way to trigger a state change.|

## Materials

[Multiple Reducers Example](https://www.youtube.com/watch?v=gBER4Or86hE)

[Redux Docs: Using Combined Reducers](https://redux.js.org/recipes/structuring-reducers/using-combinereducers/)

[Redux Docs: Combined Reducer Syntax](https://redux.js.org/api/combinereducers/)

[Time Travel in React Redux apps using the Redux DevTools](https://medium.com/the-web-tub/time-travel-in-react-redux-apps-using-the-redux-devtools-5e94eba5e7c0)
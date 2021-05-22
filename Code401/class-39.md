# Redux - Additional Topics

## What’s the best practice for “pre-loading” data into the store (on application start) in a Redux application?

group the "needs" of an entire component tree together by route. That way, when we preload the data for that route, the data for all of its children will also be loaded. In the client we would prefer to load data at the component level.

- [Preloading data in Redux app](https://gist.github.com/heygrady/c3307d8884378969cab0308cbc4cd575)
- [Correct way to pre-load component data in react+redux](https://stackoverflow.com/questions/39356517/correct-way-to-pre-load-component-data-in-reactredux)

## When using a thunk/async action that dispatches the actual action, which do you export from your reducer?

It does not generate any reducer functions, since it does not know what data you're fetching, how you want to track loading state, or how the data you return needs to be processed. You should write your own reducer logic that handles these actions, with whatever loading state and processing logic is appropriate for your own app.



## Term

| Term | Definition |
| ------- | ----------------- |
|middleware|Middleware like Redux Thunk or Redux Promise just gives you “syntax sugar” for dispatching thunks or promises, but you don’t have to use it.|
|thunk|With a plain basic Redux store, you can only do simple synchronous updates by dispatching an action. Middleware extends the store's abilities, and lets you write async logic that interacts with the store. Thunks are the recommended middleware for basic Redux side effects logic, including complex synchronous logic that needs access to the store, and simple async logic like AJAX requests.|

## Materials

[Redux Toolkit (RTK)](https://redux-toolkit.js.org/)

[Redux Toolkit Tutorial](https://redux-toolkit.js.org/tutorials/intermediate-tutorial)

[MobX](https://mobx.js.org/getting-started.html)

[HookState](https://hookstate.js.org/)

[What is a thunk](https://daveceddia.com/what-is-a-thunk/)

[createAsyncThunk#](https://redux-toolkit.js.org/api/createAsyncThunk)
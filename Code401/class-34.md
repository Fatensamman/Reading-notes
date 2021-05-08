# `<Login` /> and `<Auth />`

## Why is the Context API useful?

Context provides a way to pass data through the component tree without having to pass props down manually at every level.

- [context api](https://reactjs.org/docs/context.html)

## Can a component outside of a provider get its context?

No, every Context object comes with a Provider React component that allows consuming components to subscribe to context changes.



## What are some common use cases for using the Context API?

- Context provides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.
- Context is designed to share data that can be considered “global” for a tree of React components, such as the current authenticated user, theme, or preferred language.


## Describe “Context Hell”

there are two popular types of sharing logic in components which are Higher-Order Components and Rendering Props. When your applications have a massive quantity of nested Components, they will cause a “Wrapper Hell.”
- [React Hooks vs. Wrapper Hell](https://www.polidea.com/blog/react-hooks-vs-wrapper-hell-writing-state-in-a-function-with-ease/)

## Term

| Term | Definition |
| ------- | ----------------- |
|global state|keeping a state at the top level and provide access methods to all child levels without the need to pass props.|
|global context|React's context allows you to share information to any component, by storing it in a central place and allowing access to any component that requests it (usually you are only able to pass data from parent to child via props).|
|provider|The provider acts as a delivery service. When a consumer asks for something, it finds it in the context and delivers it to where it's needed.|
|consumer|A consumer is where the stored information ends up. It can request data via the provider and manipulate the central store if the provider allows it.|


## Materials 

[what is role based access control?](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more)

[react-cookies component](https://www.npmjs.com/package/react-cookies)

[react-cookie library](https://www.npmjs.com/package/react-cookie)

[Provider Pattern with React Context API](https://blog.flexiple.com/provider-pattern-with-react-context-api/)

[Working with the React Context API](https://www.toptal.com/react/react-context-api)
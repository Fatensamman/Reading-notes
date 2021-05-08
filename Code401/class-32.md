# Custom Hooks

## What does a component’s lifecycle refer to?

- In applications with many components, it’s very important to free up resources taken by the components when they are destroyed.

- We want to set up a timer whenever the Clock is rendered to the DOM for the first time. This is called “mounting” in React.

- We also want to clear that timer whenever the DOM produced by the Clock is removed. This is called “unmounting” in React.

## Why do you sometimes need to “wrap” functions in useCallback when called from within useEffect

Pass an inline callback and an array of dependencies. useCallback will return a memoized version of the callback that only changes if one of the dependencies has changed. This is useful when passing callbacks to optimized child components that rely on reference equality to prevent unnecessary renders 
- [useCallback](https://reactjs.org/docs/hooks-reference.html#usecallback)

## Why are functional components preferred over class components?

Hooks allow you to reuse stateful logic without changing your component hierarchy. This makes it easy to share Hooks among many components or with the community. Hooks let you use more of React’s features without classes. Hooks provide access to imperative escape hatches and don’t require you to learn complex functional or reactive programming techniques.
- [hooks intro](https://reactjs.org/docs/hooks-intro.html)


## What is wrong with the following code?

```
import React, {useState, useEffect} from 'react';

function MyComponent(props) {
  const [count, setCount] = useState(0);

  function changeCount(e) {
    setCount(e.target.value);
  }

  let renderedItems = []

  for (let i = 0; i < count; i++) {
    useEffect( () => {
      console.log('component mount/update');
    }, [count]);

    renderedItems.push(<div key={i}>Item</div>);
  }

  return (<div>
     <input type='number' value={count} onChange={changeCount}/>
      {renderedItems}
    </div>);
}
```

## Term

| Term | Definition |
| ------- | ----------------- |
|state hook|Hook that lets you add React state to function components|
|effect hook|The Effect Hook lets you perform side effects in function components. By using this Hook, you tell React that your component needs to do something after render. |
|reducer hook|is usually preferable to useState when you have complex state logic that involves multiple sub-values or when the next state depends on the previous one. It also lets you optimize performance for components that trigger deep updates because you can pass dispatch down instead of callbacks.|


## Materials

[custom hooks - all you need to know](https://www.telerik.com/kendo-react-ui/react-hooks-guide/#toc-custom-react-hooks)

[async hooks](https://dev.to/vinodchauhan7/react-hooks-with-async-await-1n9g)

[useReducer Hook](https://reactjs.org/docs/hooks-reference.html#usereducer)

[react custom hooks](https://reactjs.org/docs/hooks-custom.html)

[use hooks](https://usehooks.com/)

[hooks list](https://github.com/rehooks/awesome-react-hooks)

[10 essential react hooks](https://blog.bitsrc.io/10-react-custom-hooks-you-should-have-in-your-toolbox-aa27d3f5564d)
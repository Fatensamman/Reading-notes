# Routing


## Do child components have direct access to props/state from the parent?

No, children only have access to props when they're passed by their parents burt there are some ways for children to have access to props by using callbacks, props or redux
- [Passing Data Between React Components — Parent, Children, Siblings](https://towardsdatascience.com/passing-data-between-react-components-parent-children-siblings-a64f89e24ecf)

## When a component “wraps” another component, how does the child component’s output get rendered?
```
<Main>
  <Content />
</Main>
```

It can be rendered inside of the other component or called somewhere else and rendered there.

- [Goland Programs](https://www.golangprograms.com/how-to-render-one-component-in-another-component-in-react-js.html)

## Can a component, such as <Content />, which is a child also be used as a standalone component elsewhere in the application?

Yes by using composition

## What trick can a parent use to share all props with it’s children

you can use the spread operator:
```
const IntermediateComponent = (props) => {
  return (
    <ChildComponent {...props} />
  )
}
```
- [How to transfer props to child components](https://flaviocopes.com/react-pass-props-to-children/)

## Term

| Term | Definition |
| ------- | ----------------- |
|props.children|used to display whatever you include between the opening and closing tags when invoking a component.|
|composition|composition is a natural pattern of the component model. It's how we build components from other components, of varying complexity and specialization through props. Depending on how generalized these components are, they can be used in building many other components.|

## Materials

[browser router tutorial](https://blog.pshrmn.com/simple-react-router-v4-tutorial/)

[browser router api docs](https://reactrouter.com/web/api)

[react-if component](https://www.npmjs.com/package/react-if)
- Render React components conditionally.

[react testing library queries](https://testing-library.com/docs/dom-testing-library/api-queries)

[aria roles](https://www.w3.org/TR/html-aria/)

[A quick intro to React’s props.children](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)

[Thinking in React: Component Composition](https://dev.to/bouhm/thinking-in-react-component-composition-fp5#:~:text=In%20React%2C%20composition%20is%20a,in%20building%20many%20other%20components.)
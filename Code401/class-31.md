# Hooks API

## Why do we not need more .html pages in a multi-page React app?

React is using reusable component that are appended to the DOM. When a second page is create on a website, only components related to that page are loaded through the router. the website doesn't need a second html page.  

## If we wanted a component to show up on every page, where would we put it and why?
- Outside the `<BrowserRouter/>`
- Inside the `<BrowserRouter />`, outside a `<Route />`
- Inside a `<Route />`

We would tha component outside the `<BrowserRouter/>` because we want to app component to render it, not a particular route.

## What does props.children contain?

it is used to display whatever you include between the opening and closing tags when invoking a component.
- [A quick intro to React’s props.children](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)

## Term

| Term | Definition |
| ------- | ----------------- |
|Composition|composition is a natural pattern of the component model. It's how we build components from other components, of varying complexity and specialization through props. Depending on how generalized these components are, they can be used in building many other components.|
|Children / Child Components|all components rendered inside of another component|
|[Hash Routing](https://reactrouter.com/web/api/HashRouter)|A `<Router>` that uses the hash portion of the URL (i.e. window.location.hash) to keep your UI in sync with the URL.|
|[Link Routing](https://knowbody.github.io/react-router-docs/api/Link.html)|The primary way to allow users to navigate around your application. `<Link>` will render a fully accessible anchor tag with the proper href.|

## Materials

[making sense of hooks](https://medium.com/@dan_abramov/making-sense-of-react-hooks-fdbde8803889)

[the state hook](https://reactjs.org/docs/hooks-state.html)

[hooks api](https://reactjs.org/docs/hooks-overview.html)

[hooks api reference](https://reactjs.org/docs/hooks-reference.html)

[effects hook](https://reactjs.org/docs/hooks-effect.html)
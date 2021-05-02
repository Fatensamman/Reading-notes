# Props and State

## Does a deployed React application require a server?
React does work without server, just add script tags and make sure you use JavaScript that current browsers understand or download React source and use it anywhere that speaks JS and has DOM.

- [stackoverflow](https://stackoverflow.com/questions/40342100/run-react-application-without-server#:~:text=React%20does%20work%20without%20server,speaks%20JS%20and%20has%20DOM.)

- [Deploy your React app](https://blog.logrocket.com/8-ways-to-deploy-a-react-app-for-free/)

## Why do we prefer to test a React application at the behavior rather than the unit level?

Because front-end code isn’t about manipulating data. It’s about user events and rendering the right views at the right time.


## What does npm run build do?

npm run build creates a build directory with a production build of your app

## Describe the actual composition / architecture of a React application

- Directory Layout
- CSS in JavaScript
- Higher-order Components
- Function as Children
- Render Props

[React Architecture Best Practices](https://www.sitepoint.com/react-architecture-best-practices/)

## Term

| Term | Definition |
| ------- | ----------------- |
|BDD|behavior driven development: Agile software development process that encourages collaboration among developers, QA and non-technical or business participants in a software project.|
|Acceptance Tests|conducted to determine if the requirements of a specification or contract are met|
|mounting|Mounting is the process of outputting the virtual representation of a component into the final UI representation (e.g. DOM or Native Components). In a browser that would mean outputting a React Element into an actual DOM element (e.g. an HTML div or li element) in the DOM tree. In a native application that would mean outputting a React element into a native component.|
|build|the process of converting source code into an “executable” bundle by the browser.|

## Materials

[setState explained](https://css-tricks.com/understanding-react-setstate/)

- Update to a component state should be done using setState()
- You can pass an object or a function to setState()
- Pass a function when you can to update state multiple times
- Do not depend on this.state immediately after calling setState() and make use of the updater function instead.


[handling events](https://reactjs.org/docs/handling-events.html)

- you cannot return false to prevent default behavior in React. You must call preventDefault explicitly.

[forms](https://reactjs.org/docs/forms.html)

[state and lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)


[components and props](https://reactjs.org/docs/components-and-props.html)


[React Testing Library](https://testing-library.com/docs/react-testing-library/migrate-from-enzyme#what-is-react-testing-library)


[RTL Testing Example](https://thomlom.dev/beginner-guide-testing-react-apps/)
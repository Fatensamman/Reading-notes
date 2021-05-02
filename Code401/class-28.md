# Component Composition

## Can a parent component access the state of a child component?

yes by using props

- [Passing Data Between React Components — Parent, Children, Siblings](https://towardsdatascience.com/passing-data-between-react-components-parent-children-siblings-a64f89e24ecf)

## What can be passed along in a prop variable?

plain JavaScript objects

## How can a child component “know” the state of another component?

yes by using callbacks, props or redux
- [Passing Data Between React Components — Parent, Children, Siblings](https://towardsdatascience.com/passing-data-between-react-components-parent-children-siblings-a64f89e24ecf)

## Term

| Term | Definition |
| ------- | ----------------- |
|component props|Props are arguments passed into React components|
|component state|React components has a built-in state object. The state object is where you store property values that belongs to the component. When the state object changes, the component re-renders|
|application state|React apps have five types of state. Each type of state has a number of rules which it follows. It interacts with the other types of state in well defined ways — as long as it follows the rules. The five types of state are: Data, Communication, Control, Session, Location|


## Materials

[react basics recap](https://www.freecodecamp.org/news/these-are-the-concepts-you-should-know-in-react-js-after-you-learn-the-basics-ee1d2f4b8030/)

[props.children](https://codeburst.io/a-quick-intro-to-reacts-props-children-cb3d2fce4891)

> this.props.children is used to display whatever you include between the opening and closing tags when invoking a component.

[composition vs inheritance](https://reactjs.org/docs/composition-vs-inheritance.html)

[react testing library api example](https://testing-library.com/docs/react-testing-library/example-intro)

[The 5 Types Of React Application State](http://jamesknelson.com/5-types-react-application-state/)

[5 Types of Application State in React and How They Help in State Management](https://medium.com/@devisha.singh/5-types-of-application-state-in-react-and-how-they-help-in-state-management-a6a76cb1479e)
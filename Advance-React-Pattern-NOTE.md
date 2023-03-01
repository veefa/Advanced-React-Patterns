###### ADVANCED REACRT PATTERNS

##### 01. Context Module Functions

`The React Context Module Functions Pattern `is a design pattern used in React applications to provide global state management using the Context API.

##### 02. Compound Components


##### 04. Prop Collections and Getters

```javascript
import React from 'react';

function MyComponent(props) {
  return (
    <div>
      <h1>{props.title}</h1>
      <p>{props.text}</p>
    </div>
  );
}

function App() {
  const myProps = {
    title: 'Welcome to my app!',
    text: 'This is some text for my app.',
  };

  const getTitle = props => props.title;
  const getText = props => props.text;

  return (
    <div>
      <MyComponent {...myProps} />
      <h2>{getTitle(myProps)}</h2>
      <p>{getText(myProps)}</p>
    </div>
  );
}

export default App;
```

### Prop Collections

`Prop collections` are sets of related properties that are used to describe or define an object, component, or element in a programming language or framework. Prop collections are often used in frontend development frameworks like React or Vue.js, where they are used to pass data between components and define component behavior.

```javascript

  const myProps = {
    title: 'Welcome to my app!',
    text: 'This is some text for my app.',
  };

```

### Getters

A `prop getter`is a function that returns a prop value from a `prop collection`. `Prop getters` are commonly used in React and other frontend frameworks to pass data down to child components or to define the behavior of a component. Prop getters can also be used to create reusable components or to define a set of props that are commonly used in a project or application.


``` javascript

const getTitle = props => props.title;
const getText = props => props.text;

```
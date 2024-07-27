## Intro:
- A javascript library for building User interface
- Allows for the creation of custom HTML-like elements. For example, 
    ```
    <body>
        <MyHeader/>
        <PageContent/>
        <MyFooter/>
    </body>
    ```
-

### React vs React native 
-  The latter is a React JS-based framework to design mobile apps


### JSX:
- (JavaScript XML) is an extension syntax for JavaScript that allows you to write HTML-like code within your JavaScript code.

```
## With JSX:
const myElement = <h1>I Love JSX!</h1>;
const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(myElement);

## Without JSX:
const myElement = React.createElement('h1', {}, 'I do not use JSX!');
const root = ReactDOM.createRoot(document.getElementById('root'));
root.render(myElement);
```

### Babel:
- Javascript compiler used by "react" module.
- Able to compile latest js syntax into browser understandable vanilla js.

### To create a new react app:
- Install nodejs - https://nodejs.org/en
- `npx create-react-app app-name`

### Useful commands
- npm start

### Props
- Used to pass values to a react component
- Eg)
    ```
    function Component(props) {
        console.log(props.name);
    }
    <body>
        <Component name="test"/>
    </body>
    ``` 

### Hooks
- React Hooks are functions that let you use state and other React features in functional components. 
- Eg)
```
useState:
--------
import React, { useState } from 'react';

function Counter() {
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You've clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>Click me</button>
    </div>
  );
}
```
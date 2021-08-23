# react_components_introduction
Created with CodeSandbox.      
Notes from React module.     
The Complete 2021 Web Development Bootcamp     
Instructor: Dr. Angela Yu   

## Description
There were two ways of adding state into a React app: 
* Functional Component
* Class Component

### Functional Component
We create functions that render the separated React Components.

```
import React from "react";

function App() {
  return <h1>Hello World</h1>;
}

export default App;
```

### Class Component
Instead of splitting individual components into functions, we can  create a class. 

```
import React from "react";
import ClassComponent from "./ClassComponent";

class App extends React.Component {
  render() {
    return <ClassComponent />;
  }
}

export default App;
```
Class don't need parenthesis ()         
We need to extend our class from the React.Component      
To render our component we have to render inside our render() ...  method 

In the past, the main reason why people converted their functional components into class components        
was because it was required in order to have state.

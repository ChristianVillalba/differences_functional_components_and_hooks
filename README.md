# Functional Component & Class Component
Created with CodeSandbox.      
Notes from React module.     
The Complete 2021 Web Development Bootcamp     
Instructor: Dr. Angela Yu   

## Description
This project just makes a comparation between 
* Functional Component
* Class Component

These are the two ways to add state into a React app.

We created ClassComponent.jsx, it has a single button which increases the number of the count.           
FunctionalComponent.jsx does the same, but it requires less code.  

## Notes

In the past, the main reason why people converted their functional components into class components        
was because it was required in order to have state.      
* [State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html) > Converting a Function to a Class     

The code resulting using "class" is longer, harder and it gets pretty complicated when you want to reuse some of your state functionality across different components.
To solve this problem Hooks were created
* [Introducing Hooks](https://reactjs.org/docs/hooks-intro.html)     
 
We can only use hooks with Functional Components.      
The React team recommends using hooks instead of classes because this is a much easier way of managing state....      
But we will occasionally see components built using classes.      

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
Class don't need parenthesis ( )         
We need to extend our class from the React.Component      
To render our component we have to render inside our render() ...  method 

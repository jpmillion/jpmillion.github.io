---
layout: post
title:      "Functional Component Vs Class Component in React"
date:       2021-05-12 23:02:54 +0000
permalink:  functional_component_vs_class_component_in_react
---


## Class Component

A class component in react is a javascript class that extends React.Component class.  A valid class component in react is required to call the render method.

```
import React, {Component} from 'react';

class Greeting extends Component {
     render() {
      return <h1>Hello, {this.props.name}</h1>;
  }
}
```
The above component will return JSX.  JSX is the HTML that is returned from a react component.  There are also properties know as props in a react class component.  This.props is an object in a class component.  In the above example this.props.name is interpolating the value of the name in the props object.

```
this.props = { name: value }
```
The values of the props in a component are set by a parent or ancestor component and passed down.

```
import React, {Component} from 'react';
import Greeting from './Greeting;

class GreetingContainer extends Component {
  render() {
	  return <Greeting name='John' />
	}
}
```
Class Components are stateful components.  The state of a component is an object that holds data that may change over the lifespan of a component.  When the data in the state changes the component will rerender to reflect those changes.  There are also lifecycle methods that can be used to manipulate state or the rendering of the component when state is changed.

```
...

this.state = {
  timesClicked: 0
}
...

handleClick() {
  this.setState( state => ({
	  timesClicked: state.timesClicked + 1
	}))
}

...

<button onClick={this.handleClick} />

...
```

## Functional Components

Functional components are just javascript functions that return JSX.  

```
function Greeting(props) {
  return <h1>props.name</h1>
}
```

In the functional component above, props are an object( *props = { name: value }* ) passed in as an argument to the function.

Functional components are not stateful and do not have lifecyle functions. However there are hooks that can be used with functional components that will mimic state and cause rerendering of the functional component.

## Conclusion

Which type of component you use in your react app is dependent on the needs of the component.  If you do not need state(*data that may change over the lifespan of the component*) then the functional component is the appropiate choice.  Now, with the introduction of hooks, functional components can be used even when state(*ie useState hook*) and lifecycle methods(*ie useEffect hook*) are necessary.  Functional components are becoming more and more popular because of their simplicity and versitility.

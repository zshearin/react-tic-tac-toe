# react-tic-tac-toe
Following tutorial for creating react tic tac toe app [here](https://reactjs.org/tutorial/tutorial.html)


Running the application: 

```
cd my-app/src #where the index.js file is 
npm start
```

## Notes

JavaScript build toolchain typically consists of: 
* A package manager - lets you take advantage of a vast ecosystem of third-party packages, and easily install/update them (e.g. Yarn or npm)
* A bundler - lets you write modular code and bundle it together into small packages to optimize load time (e.g. webpack or Parcel)
* A compiler - lets you write modern JavaScript code that still works in older browsers (e.g. Babel)


React has a few different kinds of components
* Use components to tell React what we ant to see on the screen
* A component takes in parameters (called `props` - short for properties) and returns a hierarchy of views to display via the `render` method
* The `render` method returns a React element, which is a lightweight description of what to render
* To "remember" things, components use `state` (can have state by setting `this.state` in their constructors)
* In JavaScript classes, you need to always call `super` when defining the constructor of a subclass.  All React component classes that have a `constructor` should start with a `super(props)` call
* Calling `this.setState` from an `onClick` handler in a component's `render` method tells React to re-render the component whenever its `<button>` is clicked
* When you call `setState` in a component, React automatically updates the child components inside of it too
* **function components** are a simpler way to write components that only contain a `render` method and don't have their own state.


* Unlike the array `push()` you might be more familiar with, the `concat()` method doesn't mutate the original array, so we prefer it
* React elements are first-class JavaScript objects - we can pass them around in our applications.  To render multiple items  in React, we can use an array of React elements
* In JavaScript, arrays have a `map()` method that is commonly used for mapping data to other data.  Eg:
```
const numbers = [1, 2, 3];
const doubled = numbers.map(x => x * 2); // [2, 4, 6]
```

* **It's strongly recommended that you assign proper keys whenever you build dynamic lists** 

## Code snippets

Saves typing (the following 2 are the same):
```
onClick={function() { console.log('click'); }}
onClick={() => console.log('click')} 
```
Notice how the second one we're passing a function as the onClick prop.  React will only call this function after a click.  Forgetting the () => and writing `onClick={console.log('click')}` is a common mistake and would fire every time the component re-renders




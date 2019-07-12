## Building Blocks of ~~Life~~ Apps -  Components

React apps are made up of components. Think of components as different parts of the app. Each button is a component, each text is a component etc. From html, you might recognize some of the built in components like `<div />` and `<li />`, but in React, we can create our own components! How cool is that??

[ADD IMAGE HERE]

Take a look at the following line in `App.jsx`. 

```javascript
class App extends React.Component
```

This line is saying that we are taking all the properties a component has and creating our own component named "App". If you take a look inside the `render` method of `App`, you can see that there are a lot of other components like `<button/>`. These components are called **child components** because they are all a part of its parent, `App`. 

# Content

## Building Blocks of ~~Life~~ Apps -  Components

React apps are made up of components. Think of components as different parts of the app. Each button is a component, each text is a component etc. From html, you might recognize some of the built in components like `<div />` and `<li />`, but in React, we can create our own components! How cool is that??

![Assignments Solution](https://user-images.githubusercontent.com/25253905/61293228-11f26580-a788-11e9-90ac-9612c2bddf6b.png)

In our [solution](https://githubtraining.github.io/react-solution/), our assignments pages looks like the above. The overall webpage is a component that we call `App` and inside `App` there's a bunch of other components like buttons, titles, and even other custom components that we can create (like the Assginments List).

Take a look at the following line in `App.jsx`. 

```javascript
class App extends React.Component
```

This line is saying that we are taking all the properties a component has and creating our own component named "App". If you take a look inside the `render` method of `App`, you can see that there are a lot of other components like `<button/>`. These components are called **child components** because they are all a part of its parent, `App`. 

Scroll down to add a header component!
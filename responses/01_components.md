# Building Blocks of ~~Life~~ Apps -  Components

Awesome! You successfully opened a pull request!

In this Pull Request you will:

- Add components
- Pass data to child components
- Create and use state variables
- Use callback functions to communicate data

First, we'll learn about components.

## Components

**Components** are the **building blocks of React apps**. Think of components as different parts of the app. Each button is a component, each paragraph of text is a component, and so on. From html, you might recognize some of the built in components like `<div />` and `<li />`. In React, we can create our own components! How cool is that?

### Components in `src/App.jsx`

![Assignments Solution](https://user-images.githubusercontent.com/25253905/61293228-11f26580-a788-11e9-90ac-9612c2bddf6b.png)

In our [solution](https://githubtraining.github.io/react-solution/), our assignments page looks like the above. The overall webpage is a component called `App`. Inside `App` there are other components like buttons, titles, and custom components that we can create (like the Assginments List).

Take a look at the following line in `src/App.jsx`.

```javascript
class App extends React.Component
```

This line takes a component's properties to create a component named "App". In the `render` method of `App`, there are other components like `<button/>`. These components are **child components** because they are all a part of its parent, `App`.

Scroll down to add a header component.

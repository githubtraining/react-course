## Building Blocks of ~~Life~~ Apps -  Components

React apps are made up of components. Think of components as different parts of the app. Each button is a component, each text is a component etc. From html, you might recognize some of the built in components like `<div />` and `<li />`, but in React, we can create our own components! How cool is that??

[ADD IMAGE HERE]

Take a look at the following line in `App.js`. 

```javascript
class App extends React.Component
```

This line is saying that we are taking all the properties a component has and creating our own component named "App". If you take a look inside the `render` method of `App`, you can see that there are a lot of other components like `<button/>`. These components are called **child components** because they are all a part of its parent, `App`. 


### Add some code
Let's add a couple of child components and give our app a header and a footer.


[ADD CODE TO ADD HERE]


### Run your code
To run your code, inside your repo folder in your termainal run `npm start`.

### Push your code
Let's push your code to GitHub

Run the following lines inside your repo folder in your terminal.

```
git add src/App.js
git commit -m "added a header and footer"
git push origin changes
```

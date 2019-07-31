### Replace the title

But what does the `List` component do with this information? Let's take a look. 

Go to `List.jsx`. In the `render` method, in our input tag, you see that we set our `placeholder` to `this.props.placeholder`, and then at the bottom of our `render` method, we loop through out `this.props.currList`, to show each item in the list that we pass. Adding `this.props` tells the component to look for that property that was passed to it.

Let's go ahead and replace that ugly title with a prop. In our `render` method in `List.jsx`, where it says to replace the title with a prop, replace that with `{this.props.title}`.

### Run your code

To run your code, move inside your repo folder in your terminal and run `npm start`

### Push your code
Awesome! We are using props! You already learned so much! 

To push your code to Github, run the following lines inside the repo folder in your terminal.

```
git add src/App.jsx
git add src/List.jsx
git commit -m "using props for List component"
git push origin changes
```

I'll respond after you push.
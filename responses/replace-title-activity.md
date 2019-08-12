## Step 5 - Adding a prop

But what does the `List` component do with this information? Let's take a look. 

Go to `List.jsx`. In the `render` method, in our input tag, you see that we set our `placeholder` to `this.props.placeholder`, and then at the bottom of our `render` method, we loop through out `this.props.currList`, to show each item in the list that we pass. Adding `this.props` tells the component to look for that property that was passed to it.

Let's go ahead and replace that title with a prop. 

### :keyboard: Activity: Replace the title prop in `List.jsx`

1. In our `render` method in `List.jsx`, on line 31, where it says to replace the title with a prop, replace that with `{this.props.title}`
2. To run your code, move inside your repo folder in your terminal and run `npm start`
3. Commit and push your code to the `changes` branch:
    ```
    git add src/App.jsx
    git commit -m "import list component"
    git push origin changes
    ```

    I'll respond after you push.

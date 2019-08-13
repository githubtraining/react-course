## Step 5 - Adding a prop

But what does the `List` component do with this information? Let's take a look. 

Go to `List.jsx`. In the `render` method, in our input tag, you see that we set our `placeholder` to `this.props.placeholder`, and then at the bottom of our `render` method, we loop through out `this.props.currList`, to show each item in the list that we pass. Adding `this.props` tells the component to look for that property that was passed to it.

Let's go ahead and replace that title with a prop. 

### :keyboard: Activity: Replace the title prop in `src/List.jsx`

1. In our `render` method in `List.jsx`, on line 31, replace `REPLACE THIS TITLE WITH A PROP` with `{this.props.title}`
2. Save your code
3. To run your code, move inside your repo folder in your terminal and run `npm start`
4. Exit the process in your terminal using `Ctrl + C`
5. Commit and push your code to the `changes` branch:
    ```
    git add src/List.jsx
    git commit -m "import list component"
    git push
    ```

    After I detect a push, I'll respond

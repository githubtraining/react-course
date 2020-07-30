## Step 5: Adding a `prop`

What does the `List` component do with the information we just included? Adding `this.props` tells the component to look for the property that was passed to it.

To see, open the `src/List.jsx` file. In the `render` method, in our input tag, notice that we set our `placeholder` to `this.props.placeholder`. Then, at the bottom of our `render` method, we loop through our `this.props.currList`. This shows each item in the list that we pass.

Let's go ahead and replace the current title with another `prop`.

### :keyboard: Activity: Replace the title prop in `src/List.jsx`

1. In `src/List.jsx`, replace line 31 with `{this.props.title}`
2. Save your changes
3. To run your code, move inside your repo folder in your terminal and run `npm start`
4. Exit the process in your terminal using `Ctrl + C`
5. Stage, commit, and push your changes to the `changes` branch:
    ```
    git add src/List.jsx
    git commit -m "use a prop for the header"
    git push
    ```

<hr>
<h3 align="center">Watch below this comment for my response.</h3>

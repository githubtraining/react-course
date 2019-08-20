# Conditional Rendering

Let's take a look at what the code between lines 52 and 61 means. When we click the `Assignments` button, the list for assignments is assigned to the variable `tabChoice`. `tabChoice` is rendered in the `render` method.

But how do we specialize the `List` for our assignments? This where our props come into play. We create properties such as `placeholder`, and `currList`. We then assign values to them.

## Step 4: Import Assignments

Now that we imported the child component, let's use it in our code. At the end of this step, you should be able to click on the `Assignments` tab and render the following:

![No Title Assignments](https://user-images.githubusercontent.com/25253905/61294177-1ddf2700-a78a-11e9-963d-8b6d2a4f7b82.png)

### :keyboard: Activity: Uncomment the assignments conditional in `src/App.jsx`

1. In `src/App.jsx`, uncomment the conditional statement between lines 52 and 61
2. Save your changes
3. To run your code, move inside your repo folder in your terminal and run `npm start`
4. Exit the process in your terminal using `Ctrl + C`
5. Stage, commit, and push your code to the `changes` branch:
    ```
    git add src/App.jsx
    git commit -m "uncomment assignment rendering"
    git push
    ```
<hr>
<h3 align="center">Watch below this comment for my response.</h3>

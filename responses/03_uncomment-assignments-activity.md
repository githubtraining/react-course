## Step 4: Uncomment Assignments Section 

Now that we imported the child component, let's use it in our code. At the end of this step, you should be able to click on the `Assignments` tab and render the following:

![No Title Assignments](https://user-images.githubusercontent.com/25253905/61294177-1ddf2700-a78a-11e9-963d-8b6d2a4f7b82.png)

### Understanding Conditional Rendering

Let's take a look at what the code between lines 52 and 61 means. Basically, what it is saying is that when we click the `Assignments` button, the list for assignments will be assigned to the variable `tabChoice`. In our `render` method, we see that `tabChoice` is rendered.

But how do we specialize the `List` for our assignments? This where our props come into play. We create properties such as `placeholder`, and `currList`. We then assign values to them.

### :keyboard: Activity: Uncomment the assignments conditional in `src/App.jsx`

1. Go ahead and uncomment the conditional statement betweens lines 52 and 61 underneath where it says to `Uncomment below to render assignments` 
2. Save your code
3. To run your code, move inside your repo folder in your terminal and run `npm start`
4. Exit the process in your terminal using `Ctrl + C`
5. Commit and push your code to the `changes` branch:
    ```
    git add src/App.jsx
    git commit -m "uncomment assignment rendering"
    git push
    ```
<hr>
<h3 align="center">Watch below this comment for my response</h3>

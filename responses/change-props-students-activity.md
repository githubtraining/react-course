## Step 9: Adding the correct props

Take a look at this conditional between lines 71 and 80 in `src/App.jsx`. 

We are trying to render the correct component when we click `Students`.

There are some issues with this code. We want to be modifying the `students` list, not the `assignments` list. 

Let's go ahead and change some props!

### :keyboard: Activity: Change the props for Students

1. Uncomment the conditional statement between lines 71 and 80
2. On line 74, change the `placeholder` prop to `"Add Student..."`
3. On line 75, change the `currList` prop to `{this.state.students}`
4. On line 76, change the `addFunction` prop to `{this.addStudent}`
5. Save your code
6. To run your code, move inside your repo folder in your terminal and run `npm start`
7. Exit the process in your terminal using `Ctrl + C`
8. Commit and push your code to the `changes` branch:
    ```
    git add src/App.jsx
    git commit -m "change props for students rendering"
    git push
    ```

<hr>
<h3 align="center">Watch below this comment for my response</h3>
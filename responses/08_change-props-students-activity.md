## Step 9: Adding the correct props

There are some issues with this code. We want to be modifying the `students` list, not the `assignments` list.

Let's change some props between lines 71 and 80 to render the correct components when we click `Students`.

### :keyboard: Activity: Change the props for Students

1. Uncomment the conditional statement between lines 65 and 75 of `src/App.jsx`
2. On line 68, change the `placeholder` prop to `"Add Student..."`
3. On line 69, change the `currList` prop to `{this.state.students}`
4. On line 70, change the `addFunction` prop to `{this.addStudent}`
5. Save your changes
6. To run your code, move inside your repo folder in your terminal and run `npm start`
7. Exit the process in your terminal using `Ctrl + C`
8. Stage, commit, and push your changes to the `changes` branch:
    ```
    git add src/App.jsx
    git commit -m "change props for students rendering"
    git push
    ```

<hr>
<h3 align="center">Watch below this comment for my response.</h3>
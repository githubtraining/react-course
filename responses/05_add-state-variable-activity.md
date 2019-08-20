### Step 6: Add a state variable

In React, we store dynamic data in **state variables**. Let's take a look at how we store state variables. In `src/App.jsx`, take a look at the constructor. You'll see that we declare our state variables using `this.state = {.....}`.


Currently, in `App`, we have three state variables:
- `buttonClicked` - This stores which button was clicked. It is a state variable because the button that is clicked has the ability to change.
- `assignments` - This stores the list of assignments. It is a state variable because the list changes every time a new assignment is added.
- `grades` - This should store the grade for each student. However, we have no way to store students, so let's fix that!

### :keyboard: Activity: Add a state variable to `src/App.jsx`

1. On line 11, add a state variable named `students` 
2. Set `students` equal to an empty array
3. Add a comma: `students: [],`
4. Save your code
5. To run your code, move inside your repo folder in your terminal and run `npm start`
6. Exit the process in your terminal using `Ctrl + C`
7. Commit and push your code to the `changes` branch:
    ```
    git add src/App.jsx
    git commit -m "add a state variable for students"
    git push
    ```

<hr>
<h3 align="center">Watch below this comment for my response</h3>
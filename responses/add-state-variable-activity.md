### Step 6: Add a state variable

In React, we store dynamic data in **state variables**. Let's take a look at how we store state variables. In `App.jsx`, take a look at the constructor. You'll see that we declare our state variables using `this.state = {.....}`.


Currently, in `App`, we have three state variables:
- `buttonClicked` - This stores which button was clicked. It is a state variable because the button that is clicked has the ability to change.
- `assignments` - This stores the list of assignments. It is a state variable because the list changes every time a new assignment is added.
- `grades` - This should store the grade for each student. However, we have no way to store students, so let's fix that!

### :keyboard: Activity: Add a state variable to `App.jsx`

1. Add a state variable to `App` and name it `students`. Set it equal to an empty array. Make sure to add the comma! 
2. Save your code
3. Run your code with `npm start`
4. Commit and push your code to the `changes` branch:
    ```
    git add src/App.jsx
    git commit -m "add a state variable for students"
    git push
    ```

    After I detect a push, I'll respond
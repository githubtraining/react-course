# Activity

### Add a state variable

In React, we store dynamic data in **state variables**. Let's take a look at how we store state variables. In `App.jsx`, take a look at the constructor. You'll see that we declare our state variables using `this.state = {.....}`.


Currently, in `App`, we have three state variables:
- `buttonClicked` - This stores which button was clicked. It is a state variable because the button that is clicked has the ability to change.
- `assignments` - This stores the list of assignments. It is a state variable because the list changes every time a new assignment is added.
- `grades` - This should store the grade for each student. However, we have no way to store students, so let's fix that!

Add a state variable to `App` and name it `students`. Set it equal to an empty array. Make sure to add the comma! 

### Run your code
Run your code with `npm start` to make sure there are no errors.


### Push your code

```
git add src/App.jsx
git commit -m "using students state variable and setting state"
git push origin changes

```

I'll respond after you push.
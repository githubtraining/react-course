## A Date with Data - State Variables

So now, we learned how to pass data to components, but let's talk about the data itself.

There are two types of data: **static data** and **dynamic data**.

Static data doesn't change, hence the name static. Things like a title on a page or the name of a button would be static data.

Dynamic data, on the other hand, is data that does change because we can change it by adding an item to the list. Our list of assignments would be considered dynamic data. But how do we deal with dyanmic data in React? We can't just dump it in a component, because how will we tell the data to change?

In React, we store dynamic data in **state variables**. Let's take a look at how we store state variables. In `App.js`, take a look at the constructor. You'll see that we declare our state variables using `this.state = {.....}`.

[PUT THE CODE HERE]

Currently, in `App`, we have three state variables:
- `buttonClicked` - This stores which button was clicked. It is a state variable because the button that is clicked has the ability to change.
- `assignmentsList` - This stores the list of assignments. It is a state variable because the list changes every time a new assignment is added.
- `grades` - This should store the grade for each student. However, we have no way to store students, so let's fix that!

### Add some code

Add a state variable to `App` and name it `studentsList`. Set it equal to an empty list. Make sure to add the comma! 

Ok, so now we added a state variable, how do we actually change the data?

Unfortunatley, we can't just do `this.state.studentsList = .....` to change data. I wish it was that simple!

To set the state of a state variable we have to use the method, `this.setState`.

Take a look at the following code in `App.js`

```
handleButtonClicked(buttonName) {
    this.setState({
      buttonClicked: buttonName
    });
  }
```

When this method is called, it setting the state variable `buttonClicked` to the argument, `buttonName` using `this.setState`.

In our `render` method we see that `handleButtonClicked` is called when each button is clicked with it's respective arguments. For instance, when the `Assignments` button is clicked, we call `handleButtonClicked("assignments")`.

We are going to set some state in next steps.

### What your code should look like

`[ADD SCREEN VID]`

### Push your code
To push your code to Github, run the following lines inside the repo folder in your terminal.

```
git add -u
git commit -m "using props for List component"
git push origin changes
```
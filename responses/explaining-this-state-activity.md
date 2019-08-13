### Explaining `this.setState`

Ok, so now we added a state variable, how do we actually change the data?

Unfortunatley, we can't just do `this.state.studentsList = .....` to change data.

To set the state of a state variable we have to use the method, `this.setState`.

Take a look at the above code in `App.jsx`

When this method is called, it setting the state variable `buttonClicked` to the argument, `buttonName` using `this.setState`.

In our `render` method we see that `handleButtonClicked` is called when each button is clicked with it's respective arguments. For instance, when the `Assignments` button is clicked, we call `handleButtonClicked("assignments")`.

We are going to set some state in next steps.

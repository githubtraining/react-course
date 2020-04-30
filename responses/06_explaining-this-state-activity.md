### Explaining `this.setState`

How do we change data within a state variable?

Unfortunately, we can't just do `this.state.studentsList = .....` to change data.

To set the state of a state variable we have to use the method, `this.setState`.

Take a look at the method on line 30 in `src/App.jsx`

When this method is called, it is adding `assignmentName` to our state variable `assignments` by setting the state of `assignments` to itself with the concatenation of `assignmentName`.

We are going to set some state in next steps.

## Callback example in `src/List.jsx`

Navigate to `src/List.jsx`

Let's take a look at this piece of code between lines 18 and 25 in `src/List.jsx`.

```jsx
handleSubmit(event) {
    this.setState({
      value: ""
    });

    this.props.addFunction(this.state.value);
    event.preventDefault();
}
```

It looks like when the submit button is clicked, we call the `addFunction` with the value of our input box. For assignments, this `addFunction` references the `this.addAssignment` in `App`. So when we call `this.props.addFunction`, we are calling back to the parent component and using the parent's function. 

Scroll below for next steps!
## Throwing it Back - Callback Functions

Alright, let's go ahead and FIX EVERYTHING now! It may sound ambitious but let's dive in.

The last thing you need to know before you can call yourself a React Developer is callback functions.  We said that we can pass data to the child with `props`, but what about passing data from the child to the parent? 

With callback functions, we are able to do just that. Basically, we pass a function as a prop, and then the child component can call the function that was defined in the parent. Yeah, that's confusing. Let's look at an example.

Take a look at this code in `App.jsx`
```jsx
addAssignment(assignmentName) {
    this.setState({
      assignments: this.state.assignments.concat(assignmentName)
    });
  }
```
What's happening here? 

It looks like we are taking an `assignmentName` as an argument and then adding that to the end of our `assignments` list. But where is this function called?

So it looks like we pass the `addAssignment` function as a prop in this chunk of code.

```jsx
if (this.state.buttonClicked === "assignments") {
      tabChoice = (
        <List
          placeholder="Add Assignment..."
          currList={this.state.assignments}
          addFunction={this.addAssignment}
          title="Assignments"
        />
      );
    }
```

Navigate to `List.jsx`

Let's take a look at this piece of code:

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



### Add some more code

Hmmm, there's some stuff wrong about this code. We want to be modifying the `students` list, not the `assignments` list. 

Let's go ahead and change some props!

- Change the `placeholder` prop to `"Add Student..."`
- Change the `currList` prop to `{this.state.students}`
- Change the `addFunction` prop to `{this.addStudent}`

LAST THING! Let's get our grades working!

Uncomment this last chunk of code!
```
/*if (this.state.buttonClicked === "grades") {
      tabChoice = (
        <Table
          tableNames={this.state.assignments}
          rows={this.state.students}
          addFunction={this.addGrade}
          data={this.state.grades}
        />
      );
    }*/
```

### Run your code
To run your code, move inside your repo folder in your terminal and run `npm start`

### What your code should look like

`[ADD SCREEN VID]`

### Push your code
To push your code to Github, run the following lines inside the repo folder in your terminal.

```
git add -u
git commit -m "using props for List component"
git push origin changes
```
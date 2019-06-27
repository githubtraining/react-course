## Throwing it Back - Callback Functions

Alright, let's go ahead and FIX EVERYTHING now! It may sound ambitious but let's dive in.

The last thing you need to know before you can call yourself a React Developer is callback functions.  We said that we can pass data to the child with `props`, but what about passing data from the child to the parent? 

With callback functions, we are able to do just that. Basically, we pass a function as a prop, and then the child component can call the function that was defined in the parent. Yeah, that's confusing. Let's look at an example.

Take a look at this code in `App.js`
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

It looks like when the submit button is cicked, we call the `addFunction` with the value of our input box. For assignments, this `addFunction` references the `this.addAssignment` in `App`. So when we call `this.props.addFunction`, we are calling back to the parent component and using the parent's function. 


### Add some code
Now that we see how it works with assignments, let's try it with students! 

Below this line of code in `App.js`
```
  /*Write an addStudent function here for step 4*/
```

create a method called `addStudent`

`addStudent` should take `studentName` as a parameter and then concat that `studentName` to the end of `students` list that we created earlier. 

Also, since we created a method that changes the a state variable, we have to bind it to our class, so that when we call it, we know what method to reference.

Go ahead and uncomment the following line.

```
    /*this.addStudent = this.addStudent.bind(this);*/
```

Awesome, now let's actually add some functionality to our students button.

Go ahead and uncomment this code.

```
/*if (this.state.buttonClicked === "students") {
      tabChoice = (
        <List
          placeholder="Add Assignment..." 
          currList={this.state.assignments}
          addFunction={this.addAssignment}
          title="Student Roster"
        />
      );
    }*/
```

### Run your code
To run your code, move inside your repo folder in your terminal and run `npm start`

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
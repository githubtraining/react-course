## How to Talk to your Child - Props

Alright, so we established that components are awesome, but what about reusable components with different properties? 

That might sound a little confusing, but let's take a look. Go to our final solution and add some assignments along with students. You might start to notice that both lists look the same but with different values. In fact, both lists are the same component!

Hmmm, but how do we pass different values to a component? We do so by passing properties to the component, otherwise known as props. 

We will get a little deeper into that in a bit. 

[IMAGES]

### Add some code

Navigate to `List.jsx`. You'll see that we made our own component, `List`. 

Let's go ahead and import that component.

At the top of `App.js`, on line 3, add

```js
import List from "./List";
```
Awesome! Now around line 50, underneath where it says

```js
/*Uncomment below for step 2*/
```
go ahead and uncomment the following chunk of code

```js
/*if (this.state.buttonClicked === "assignments") {
      tabChoice = (
        <List
          placeholder="Add Assignment..."
          currList={this.state.assignments}
          addFunction={this.addAssignment}
          title="Assignments"
        />
      );
  }*/
```

### Run your code

To run your code, move inside your repo folder in your terminal and run `npm start`

### What your code should look like

`[ADD SCREEN VID]`

### Code Explanation

Let's take a look at what this code means. Basically, what it is saying is that when we click the `Assignments` button, the list for assignments will be assigned to the variable `tabChoice`. In our `render` method, we see that `tabChoice` is rendered.

But how do we specialize the `List` for our assignments? This where our props come into play. We create properties such as `placeholder`, and `currList`. We then assign values to them.

[IMAGES]

### Add some more code

But what does the `List` component do with this information? Let's take a look. 

Go to `List.jsx`. In the `render` method, in our input tag, you see that we set our `placeholder` to `this.props.placeholder`, and then at the bottom of our `render` method, we loop through out `this.props.currList`, to show each item in the list that we pass. Adding `this.props` tells the component to look for that property that was passed to it.

Let's go ahead and replace that ugly title with a prop. In our `render` method in `List.jsx`, where it says to replace the title with a prop, replace that with `{this.props.title}`.

### Run your code

To run your code, move inside your repo folder in your terminal and run `npm start`

### Push your code
Awesome! We are using props! You already learned so much! 

To push your code to Github, run the following lines inside the repo folder in your terminal.

```
git add -u
git commit -m "using props for List component"
git push origin changes
```
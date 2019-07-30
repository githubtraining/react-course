### Change the props for Students

Take a look at this conditional in `App.jsx`. 

We are trying to render the correct component when we click `Students`. Go ahead and uncomment the entire conditional statement.

Hmmm, there's some stuff wrong about this code. We want to be modifying the `students` list, not the `assignments` list. 

Let's go ahead and change some props!

- Change the `placeholder` prop to `"Add Student..."`
- Change the `currList` prop to `{this.state.students}`
- Change the `addFunction` prop to `{this.addStudent}`

## Welcome to React!

Congratulations on taking some of your first steps into full stack development! 

So why did you decide to click and join this course? Ideally, you are a learner who:

- Understands HTML tags
- Understands classes and methods in Javascript
- Understands git and GitHub

If you understand the topics above, you can start learning modern frontend development with React!

So why do we learn React?

React has growing popularity in the tech industry because of it's simplicity. With a simple knowledge of HTML and Javascript, picking up React shouldn't be too bad.

### What will we be building

So what are we going to be building today? We are going to build a gradebook for teachers! Take a look at `deployed link here`. Here's a recording of the finished app.

`[SCREEN RECODING HERE]`

### Clone the Repo and Install Node

Let's go ahead and get started.

First, clone this repo.

In your terminal, in a folder where you would like to keep this project, run the following:

```
git clone repo_name
cd repo_name
```

Great, now if you don't have Node installed on your computer, go ahead and [install it](https://nodejs.org/en/download/)!

Awesome!

### Current Functionality 

Now, inside your repo folder, run the following:

```
npm install
npm start
```

Your browser should open `http://localhost:3000/`

You'll see that our app can't really do anything! All we have is three buttons! We are going to add all the functionality.


### So what's in our React App
Let's take a look of what our React App looks like right now.

`[SCREENSHOT OF FILE STRUCTURE]`


##### package.json

`[SCREENSHOT OF PACKAGE.JSON]`

This file is our roadmap of the app. It tells us the name of the app, the version, the different dependencies we need to run our app, and more.

##### public

This directory contains our `index.html` which directs us to the rest of the web application that requires additional processing.

##### src

This is where pretty much ALL of your code will go. You'll notice we have `App.jsx` along with other `jsx` files, but what is `jsx`. Think of `jsx` as a mix between `html` and `javascript`. We can write tags as well as functions and classes. Take a look at `App.jsx`. Some of that stuff might look familiar from `html`, like thos `<div/>` tags. Don't worry, we will get to that stuff in a bit.


### Add some code
To get started, first checkout to a new branch called `changes`

Inside your repo folder, run the following in your terminal:

```
git checkout -b changes
```

Next, navigate to `README.md`, and change the author name to your name.

### Push your code
Let's push your code to GitHub

Run the following lines inside your repo folder in your terminal.

```
git add .
git commit -m "added my name"
git push origin changes
```

After you push, this issue will respond with next steps.

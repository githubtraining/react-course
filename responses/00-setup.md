### Clone the Repo and Install Node

Let's go ahead and get started.

First, clone this repo.

In your terminal, in a folder where you would like to keep this project, clone the repo, and do the following:

```
cd intro-react
git checkout changes
```

Next, open the folder in your favorite text editor. I reccommend VSCode.

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

![File Structure](https://user-images.githubusercontent.com/25253905/61294641-28e68700-a78b-11e9-9bc1-ff468312ca8b.png)


##### package.json

![package](https://user-images.githubusercontent.com/25253905/61294748-5e8b7000-a78b-11e9-9475-163d8c7bc6b3.png)

This file is our roadmap of the app. It tells us the name of the app, the version, the different dependencies we need to run our app, and more.

##### public

This directory contains our `index.html` which directs us to the rest of the web application that requires additional processing.

##### src

This is where pretty much ALL of your code will go. You'll notice we have `App.jsx` along with other `jsx` files, but what is `jsx`. Think of `jsx` as a mix between `html` and `javascript`. We can write tags as well as functions and classes. Take a look at `App.jsx`. Some of that stuff might look familiar from `html`, like thos `<div/>` tags. Don't worry, we will get to that stuff in a bit.


### Open a Pull Request
To get started, navigate to the `Pull Requests` tab and open a Pull Request for the `changes` branch. Make sure to title your Pull Request `Changes`. 

Once you open the Pull Request, steps will appear inside the Pull Request itself.

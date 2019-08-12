
# Set up a React Application Locally

### So what's in our React App
Let's take a look of what our React App looks like right now. We will go through our file structure which is a [standard React setup](https://facebook.github.io/create-react-app/docs/getting-started). You will not be editing any files in this step, but the structure is important for future code references.

![File Structure](https://user-images.githubusercontent.com/25253905/61294641-28e68700-a78b-11e9-9bc1-ff468312ca8b.png)



##### package.json
This file is our roadmap of the app. It tells us the name of the app, the version, the different dependencies we need to run our app, and more.

##### public

This directory contains our `index.html`. That file directs us to the rest of the web application that requires additional processing.

##### src

This is where most of your code will go. You'll notice we have `App.jsx` along with other `jsx` files, but what is `jsx`. Think of `jsx` as a mix between `html` and `javascript`. We can write tags as well as functions and classes. Take a look at `App.jsx`. Some of that stuff might look familiar from `html`, like those `<div/>` tags. Don't worry, we will get to that stuff in a bit.

## Step 1: Set up locally
In this repository, we have two branches - `master` and `changes`. We will be working off of the `changes` branch. Let's go ahead and get started.

### :keyboard: Activity: Clone the repository and install Node

1. Open your terminal
2. Move into a location where you want to keep this project
3. Clone this repository
4. Move into the repository: `cd intro-react`
5. Checkout to the `changes` branch: `git checkout changes`
6. Open the `intro-react` folder in your favorite text editor 
   - We recommend VSCode
7. Check for Node installation: `node -v`
8. [Install Node](https://nodejs.org/en/download/) if it is not installed
9. In your repository folder, install the necessary packages: `npm install`
10. Start the React Application: `npm start`

Your browser should automatically open `http://localhost:3000/`, and you should see our barebones gradebook application.

You'll see that our app can't really do anything! All we have is three buttons! We are going to add all the functionality.


# Set up a React Application Locally

Hello and welcome!

Before starting this course, we recommend completing the [Introduction to GitHub Learning Lab](https://lab.github.com/githubtraining/introduction-to-github) first with the option for working locally in the command line.

### What's in our React App

Let's take a look of what our React App looks like right now. We will go through our file structure which is a [standard React setup](https://facebook.github.io/create-react-app/docs/getting-started). You will not be editing any files in this step, but the structure is important for future code references.

![File Structure](https://user-images.githubusercontent.com/25253905/61294641-28e68700-a78b-11e9-9bc1-ff468312ca8b.png)

##### `package.json`

The `package.json` file is our roadmap of the app. It tells us the name of the app, the version, the different dependencies we need to run our app, and more.

##### `public/`

The `public/` directory contains our `index.html` file. The `index.html` file directs us to the rest of the web application that requires additional processing.

##### `src`

This is where most of your code will go. You'll notice we have `App.jsx` along with other `jsx` files. But, what is `jsx`? Think of `jsx` as a mix between `html` and `javascript`. We can write tags, functions, and classes. Take a look at the `App.jsx` file. Some of that contents might look familiar from `html`, like `<div/>` tags.

## Step 1: Set up the project locally

In this repository, we have two branches - `master` and `changes`. We will be working off of the `changes` branch. Let's go ahead and get started.

### :keyboard: Activity: Clone the repository and install Node

1. Open your terminal
    - If you're using a Windows operating system, we recommend downloading and using [git bash](https://git-scm.com/downloads) as your terminal
2. Change directories into a location where you want to keep this project
3. Clone this repository: `git clone {{ repoUrl }}`
4. Move into the repository's directory: `cd intro-react`
5. Checkout to the `changes` branch: `git checkout changes`
6. Open the `intro-react` folder in your favorite text editor
7. Check for Node installation: `node -v`
8. [Install Node](https://nodejs.org/en/download/) if it is not installed
9. In your repository folder, install the necessary packages: `npm install`
10. Start the React Application: `npm start`

Your browser should automatically open `http://localhost:3000/`, and you should see our barebones gradebook application.

You'll see that our app can't really do anything! All we have is three buttons! We are going to add all the functionality.

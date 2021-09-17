# Project Contact Form

### The goal of this project is to practice working with forms

We will be using HTML, CSS, JavaScript and React

**Basic functionality:** we want the user to be able to fill in their data and a message. For this purpose, the contact form will have fields for name, email and message.

1. Create a React app using `npx create-react-app project-contact-form`
1. Delete the css from the App.css file and use this file for your css
1. Delete the code in the App.js file between `<div className="App">` and the closing `</div>`
1. Create a folder called `components` in the src folder
1. Create a new file and create a function component called ContactForm (you can use the extension .jsx instead of .js)
1. The contact form has three input fields: name, email and message,
1. For each input field, add `name=`, `type=`, `value=` and `onchange=` (you have to think yourself about what needs to come after `=` ....)
1. Add a submit button (remember: React/JSX uses `htmlFor`, not `for`, and `className` instead of `class`)
1. Use flexbox to center the form, give it margins and add margins between the input fields (it can be very basic because you can style the form later on)
1. The ContactForm component uses *controlled inputs*: you control the input by creating state to hold the input, updating that state when the value changes, and tell the input what value to display
1. For this, you need to add a hook with an object containing the input data (**remember:** if your code used `useState()` then you need to import React useState())
1. Use `onChange` with a `handleChange()` function that detects any change to the value in the field, and set the variable to this new value with the hooks (remember to add `e.preventDefault()` to prevent automatic page refresh). Hint: you have `name` and `value` for each input field, and you can use those in the `handleChange()` function to set the new data values
1. We will use a JSON file as database for the user details and messages, and use this as an API mockup. This means adding the JSON data to a local file in the project directory, and make fetch or GET calls to that file instead of a real database.
1. For this, first create a `data.json` file in the `public` folder of the project (`fetch` API calls made from a React component always look for files inside this folder)
1. Put some dummy data in the `data.json` file, to be able to use this for testing later on
1. To fetch the data, create a method `getData()` (you can look at the code in the `fetch.js` file, if you get stuck)
1. 

---

## Please note:
If you want to download a project on your local machine, do not fork it but clone the repo locally, on your computer. After that, create a new repo in your own GitHub account *with exactly the same project name*, and link the local repo to the remote repo in your GitHub account (see below). Why should you clone and not fork? It will show the project as **your own project** and not a fork of someone else's project. You can use it as a project for your portfolio.

You can connect a local project to a new, empty GitHub repo [as follows](https://docs.github.com/en/github/importing-your-projects-to-github/adding-an-existing-project-to-github-using-the-command-line). We can do this together during a CodeWomen coding session: it is very good to know this so that you can start a project locally and afterwards link it with a remote GitHub repo.

If you clone the project without forking it, you will have to change the 'remote origin' repository after cloning. Check the remote of your local project using `git remote -v`. You will probably see:  
`origin  https://github.com/CodeWomen-Barcelona/some-codewomen-project.git (fetch)`  
`origin  https://github.com/CodeWomen-Barcelona/some-codewomen-project.git (push)`

To link your local project to your own GitHub repo, you need to change the remote origin. Have a look at this article: https://devconnected.com/how-to-change-git-remote-origin/. With `git remote -v` you can again check if remote origin has been reset and now shows the name of your GitHub account.

PS: if you work for a company that has a corporate social responsibility policy and wants to support women in tech, then here is the link to the [fundraising overview of MigraCode](https://docs.google.com/spreadsheets/d/1Zs-Mmi39bcjVw2U-iEQWSHSjkb-EmET-j1WB2oJF45Q/edit#gid=0).

---
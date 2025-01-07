# Script for create a vite react app

This scripts are made to create a react app on a linux environment. If you are using windows you must use wsl console or gitbash to execute this scripts.

### Warning!

You must have installed the following in your system on order that you don't have issues with the script:

- node
- npm
- nvm

## Running instructions

The first you need to do is clone this repo on your local machine on a location that you can remember easy:

```
cd your-favorite-path
git clone https://github.com/juanvidev1/create-react-app-script.git
```

Next you should enter to the repo folder. This step is very important or the script won't work

```
cd create-react-app-script
```

Then simply run the script and the magic will work

```
bash create-react-app.sh
```

The script will ask you for a path to create your app, a name for the app, if you want to work with JavaScript or TypeScript and an optional input for a github repo remote url that, if is provided, will associate your remote repo with your local repo (created by default)

Once the script finish the execution, will run automatically your app so you can see the example of a simple form validation like this

![Execution example](/readmeAssets/runningExample.png)

If you try to send that form, it will automatically validate the data
![Validation error example on form submit](/readmeAssets/validationExample.png)

The fields will validate on every change and will remove the errors in case that the validation pass

![Validation error on change](/readmeAssets/validationChangeExample.png)

Finally if you fill the fields on the correct way, you will have an alert with the form data, this is just for the example

![Form ready to send](/readmeAssets/success1.png)
![Form submit success and passed validations](/readmeAssets/success2.png)

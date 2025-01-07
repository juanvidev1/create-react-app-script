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

After that, you MUST give execution permissions to all the scripts so they can do all their job

```
sudo chmod +x *
```

Then simply run the script and the magic will work

```
bash create-react-app.sh
```

The script will ask you for a path to create your app, a name for the app, if you want to work with JavaScript or TypeScript, an optional input for specify the node versión you want to use on the template init and an optional input for a github repo remote url that, if is provided, will associate your remote repo with your local repo (created by default)

Once the script finish the execution, will run automatically your app so you can see the example of a simple form validation like this

![Execution example](/readmeAssets/runningExample.png)

If you try to send that form, it will automatically validate the data
![Validation error example on form submit](/readmeAssets/validationExample.png)

The fields will validate on every change and will remove the errors in case that the validation pass

![Validation error on change](/readmeAssets/validationChangeExample.png)

Finally if you fill the fields on the correct way, you will have an alert with the form data, this is just for the example

![Form ready to send](/readmeAssets/success1.png)
![Form submit success and passed validations](/readmeAssets/success2.png)

### <center>&#128640; Now you can start using this react template for your projects &#128640;</center>

But, wait! That's not everything you can do. If you see there are other several files that you can use independently.

For example using the script createBaseComponent you can create a basic structure for a react component, for this you will need the following info:

- A component name (should be with the React standards for naming a new component)
- A path for create the new file (if you do not provide a path it will take your current path as the initial path)
- An optional name folder to save the new component (if you don't provide a folder it will use components, and if that folder doesn't exist will create it)
- A file extension (by default will be jsx)

The usage of the script will be

```
bash createBaseComponent.sh ExampleComponent /home/juanvidev/Documentos/prueba
```

In the example above we're creating a new jsx component for React in the folder /home/juanvidev/Documentos/prueba/components (by default the script will create the folder if doesn't exist in the path provided)
Also the script will create the file with the jsx extension by default as we doesn't provide a different extension for our file

If we take a quickly look to our path we'll see that we should have a components folder, and a folder inside of it called ExampleComponent with an index.jsx file inside it with the code of our component

![Component creation example](/readmeAssets/componentCreateExample.png)

But if you provide all the parameters you will have a different route result with a tsx component created

```
bash createBaseComponent.sh ExampleComponentTS /home/juanvidev/Documentos/prueba molecules tsx
```

![Component creation with full parameters](/readmeAssets/componentScript.png)

# Create React App Study

<br>

# What is the Create React App Study?
The Create React App Study is an exploration of the ```create-react-app``` command line tool for setting up a React development environment quickly..

Here are a few questions from the study to explore:

* [How do you use npm/npx to create a React Apps?](#How-do-you-use-npm/npx-to-create-a-React-Apps)
* [How do you a create and run a React app?](#How-do-you-a-create-and-run-a-React-app)
* [How do you run tests on the React Application?](#How-do-you-run-tests-on-the-React-Application)
* [What does the build command do?](#What-does-the-build-command-do)
* [What does the eject command do?](#What-does-the-eject-command-do?)


<br>
<br>


# How do you use npm/npx to create a React Apps?

<dl>
<dd>

## NPM helps install and manage packages for your applications.
**NPM is a dependency/package manager that comes prepackages when you install node. With npm, you can install dependencies into your project, such as express, mongoose, etc.** NPM comes prepackaged with Node, which is a run-time environment that gives you the ability to run JavaScript outside the browser. Node has a number of packages that help make development simpler by reusing packages like building blocks. Libraries like jQuery, express, etc. are available as Node packages which you can access via NPM (Node Package Manager). Usually, node packages will be installled locally into a package.json file where you can observe, add, remove, etc. packages. To run npm, you simply need to use the ```npm``` command in command line.
```
  $ npm <package-name-here>
```

<br>

## NPX is a tool for executing Node packages.
**Unlike NPM, NPX runs dependencies by installing the package, but *caches* them instead of installing them.** NPX does a few useful things: Runs locally installed node modules, test packages by temporarily installing and invoking packages from npm, can be used to test Node module versions, run commands with different Node versions, execute code from a GitHub gist, etc. To run npx, you simply use ```npx``` in command line.
```
  $ npx <package-name-here>
```

<br>

## NPX is a tool for executing Node packages.
**NPX comes bundled with NPM (5.2+), so you simply need to use the ```npx``` command and your packages.** So if you have a package that already exists (i.e. npx my-package), NPX will first search for that package in local and global storage. If the package is found, it will run it. However, if the package does NOT exist in local or global storage, the NPX will download the and save temporarily in cache.

In the example below, we run a temporary package ```cowsay``` a string to execute.
```
  $ npx cowsay 'This is an example of binary execution wihtout installation!'
```
```
  $ npx cowsay 'This is an example of binary execution wihtout installation!'
  npx: installed 1 in 1.32s
  Path must be a string. Received undefined
  npx: installed 10 in 1.932s
  C:\Users\Admin\AppData\Roaming\npm-cache\_npx\4460\node_modules\cowsay\cli.js
  __________________________________________
  / This is an example of binary execution w \
  \ ihtout installation!                     /
  ------------------------------------------
          \   ^__^
          \   (oo)\_______
              (__)\       )\/\
                  ||----w |
                  ||     ||
```

</dd>
</dl>

<br>
<br>

# How do you a create and run a React app?

<dl>
<dd>

## "create-react-app" is a ready-made React app starter.
**With ```create-react-app```, you can save time on setup and configuration to get going quicker with one simple command.** When you run this command, npx is going to download the most recent ```create-react-app``` release, run it, and then remove it from your local system. This means you will NEVER have an outdated version of the system.

<br>

## Use "create-react-app" for quick, up-to-date build setup.
The environment created from running ```create-react-app```, including: React, JSC, ES6, and Flow syntax, langauge extras like the spread operators, autoprefixed CSS, an interactive unit test runner, a live development server, offline-first server worker and web app manifest meeting Progressive web app criteria, and updates for all tools handled through a single dependency.

To create a React app using ```create-react-app```, use the following at the command line:
```
  $ npx create-react-app <name-of-app>
```

<br>

## Use "npm start" to run a React app.
Once you run the code above, it will take at least a few minutes to set everything up. Once the setup is finished, check out the scripts located in the package.json file. You will see four default commands. To run the application *in development mode*(which means that it will reload in the browser the same way as nodemon), use the following at the command line:
```
  $ npm start
```

<br>

## Use "npm run" for current script commands.
If you cant remember offhand what the script commands are, run ```npm run``` and you'll get a list of the default scripts. In the case of this app, you will see lifecycle scripts (for development) and run-scripts. For example, if you run ```npm run``` at the command line, you will see something like this:
```
  $ npm run
  Lifecycle scripts included in cra-test-app:
    start
      react-scripts start
    test
      react-scripts test

  available via `npm run-script`:
    build
      react-scripts build
    eject
      react-scripts eject
```

</dd>
</dl>

<br>
<br>

# How do you run tests on the React Application?

<dl>
<dd>

## To run tests, use the "run test" command.
Running the test command will start the test runner that lets you test your app with Jest as you build it out. This is an interactive test environment that can be used to great effect. To use the test command, run the following at the command line:
```
  $ npm test
```

</dd>
</dl>

<br>
<br>

# What does the build command do?

<dl>
<dd>

## Run "npm run build" to bundle app for production.
The build command prepares your application for production deployment. When you run the build, it correctly bundles the React application into static files for production mode and optimizes the build for the best performance. The build is minified and the filenames include the hashes and is ready to be deployed to a server. To use the build command, run the following at the command line:
```
  $ npm run build
```




</dd>
</dl>

<br>
<br>

# What does the eject command do?

<dl>
<dd>

## Run "npm run eject" to further customize project.
Although ```create-react-app``` is extremely convienent with common denominator conventions, you are limited to the options you have and eventually you may outgrow the capabilites of the initial setup. The eject command takes the app out of the ```create-react-app``` setup and allows you to customize the project configuration. The drawbacks are that you will lose automatic updates but gain flexibility in other configurations, like Babel or webpack.

For example, if you wanted to tweak the scripts and build the environment in some unique way you can *eject*, which means that it removes the single dependency and copies everything directly to the project. Be careful, because once ejected you cannot go back to a single dependency.
```
  npm run eject
```

</dd>
</dl>

<br>
<br>

# How do you install packages via NPM?

<dl>
<dd>

## Run "npm install" with the package name.
To install packages via NPM, you need to run the install command. But before you install any packages, you need to get the exact name of the package from the npm registry.  For example, if you wanted to implement a package like browserify, express, moment, grunt, etc. you simply need to use the installation name. If you have multiple packages to install, insert the name and a space between each package. Once you have the name, simple write the command as follows:
```
  $ npm install express                       // install a single package.
  $ npm i express                             // short version of installation of single package.
  $ npm install express broswerify            // install multiple packages.
```
<br>

## Check your package.json file to see if packages was added.
You package.json file will list all of the dependencies specific to your application. For example, if you installed express on your application, it would show in the "dependencies" property of the package.json object.
```
{
  ...
  ...
  ...
  "dependencies": {
    "@testing-library/jest-dom": "^4.2.4",
    "@testing-library/react": "^9.4.1",
    "@testing-library/user-event": "^7.2.1",
    "express": "^4.17.1",                         // express installed as a dependency of the application.
    "react": "^16.13.0",
    "react-dom": "^16.13.0",
    "react-scripts": "3.4.0"
  },
  ...
  ...
  ...
}
```


</dd>
</dl>

<br>
<br>

# How do you use packages in your React application?

<dl>
<dd>

## Import installed packages to your application.
To use packages in your react application, you need to import those dependencies into each and every specific document that uses them (e.g. app.js, etc.). To import the dependency, you need ot use an *import statement*.  **Import statements** are used to make JavaScript modules available to use in your specific file. For example, if you installed the "moment" library (which is use to parse, manipulate, and format dates), you would need to *import* that module *from* the dependency module you installed earlier in the following way:
```JavaScript
  import moment from 'moment';
```
<br>

## 


</dd>
</dl>

<br>
<br>
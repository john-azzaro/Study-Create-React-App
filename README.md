# Create React App Study
See it Live: 

<br>

# What is the Create React App Study?
The Create React App Study is an exploration of the ```create-react-app``` command line tool for setting up a React development environment quickly..

Here are a few questions from the study to explore:

* [How do you use npm/npx to create a React Apps?](#How-do-you-use-npm/npx-to-create-a-React-Apps)


<br>
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
          \  (oo)\_______
              (__)\       )\/\
                  ||----w |
                  ||     ||
```

</dd>
</dl>

<br>
<br>
<br>

# How do you a create a React app with create-react-app?

<dl>
<dd>

## Create React App is a quick build setup for React applications.
**With ```create-react-app```, you can save time on setup and configuration to get going quicker with one simple command.**
The environment created from running ```create-react-app```, including: React, JSC, ES6, and Flow syntax, langauge extras like the spread operators, autoprefixed CSS, an interactive unit test runner, a live development server, offline-first server worker and web app manifest meeting Progressive web app criteria, and updates for all tools handled through a single dependency.





</dd>
</dl>

<br>
<br>
<br>
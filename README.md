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
**Node is a run-time environment that gives you the ability to run JavaScript outside the browser.** Node has a number of packages that help make development simpler by reusing packages like building blocks. Libraries like jQuery, express, etc. are available as Node packages which you can access via NPM (Node Package Manager). NPM is a dependency/package manager that comes prepackages when you install node. With npm, you can install dependencies into your project, such as express, mongoose, etc. Usually, the package will be installled locally into a package.json file. To run npm, you simply need to use the ```npm``` command in console.
```
  $ npm <package-name-here>
```

<br>

## NPX is an npm package runner.
**Unlike NPM, NPX runs dependencies by installing the package, but *caches* them instead of installing them.** Additionally, NPX can help avoid versioning, dependency issues, and intalling unecessary packages that you just want to try out as well as give you a clear and easy way to execute packages, commands, modules, and event GitHub gists and repositories. To run npx, you simply need ot 
```
  $ npx <package-name-here>
```

<br>

## NPX searches and/or downloads package files.
**NPX comes bundled with NPM (5.2+), so you simply need to use the ```npx``` command and your packages.** So if you have a package that already exists (i.e. npx my-package), NPX will first search for that package in local and global storage. If the package is found, it will run it. However, if the package does NOT exist in local or global storage, the NPX will download the and save temporarily in cache.



```
  npx cowsay
```
<br>



</dd>
</dl>
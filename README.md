# Meteor Boilerplate Project

## Description

Meteor boilerplate code based on personal workflow and Meteor Guide's recommendations for [Code Style](http://guide.meteor.com/code-style.html) and [Project Structure](http://guide.meteor.com/structure.html)

## Usage

**1. Refactor project's name**
   
1. Rename the folder
2. Rename the project's name in package.json

**2. Install all dependencies**

1. meteor npm install

**3. Configure your IDE**

**WebStorm**

1. Set the correct language version.
 
    Set JavaScript version to ECMAScript6 in Preferences > Languages & Frameworks > JavaScript 

2. Enable ESLINT

    1. Enable ESLINT in Preferences > Languages & Frameworks > JavaScript > Code Quality Tools > ESLint 
    2. Indicate the route to your node interpreter
    3. Indicate the route to your ESLint package. You can use both the globally installed or your project's package after executing meteor npm install command.
    4. Indicate the route to the especified .eslintrc file in the Configuration file field. The .eslintrc is placed in the root of the project.

3. Enable Babel transpiler.

    1. Create a new folder called '.out' at your project's root level.
    2. Create a new File watcher in Preferences > File Watchers.
    3. Select Babel from the list of available templates.
    4. Select JavaScript for the File type
    5. Create a new Custom Scope excluding the following files and folders: 
        .idea
        .meteor
        node_modules
        .out
        .eslintignore
        .eslintrc
        .gitignore
        package.json
        README.md
        
    6. Indicate the path to babel if this has not been automatically filled.
    7. Indicate the following Arguments: $FilePathRelativeToProjectRoot$ --source-maps --out-dir .out
    8. Specify the following Working directory: $ProjectFileDir$
    9. Indicate the '.out' as the Output paths to refresh.     

**4. Enjoy** 
     



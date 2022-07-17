# Node.js
## What is Node.js?
```
Node.js run with javascript, is fast and alows scalable and fast website application.
Until now javascript was trapped in the browser without the ability to manipulate the computer files.
Node.js helps to create a web application and write code that can interact directly with the computer.
Use Node.js to run javascript code on somebody else's computer, or rather a server.
```

## The power of the command line and how to use Node
```
1.- Create a folder in the desktop call "intro-to-node"
2.- Create a index.js file inside that folder
3.- Edite the index.js and write a "console.log("hello world")" inside
4.- Execute the index.js file local in the command linde
Hint: use the command "node"
```
```
The Node REPL (Read Evaluation Print Loops) allows you to exectue code in bite size chunks
like what we did with the chrome developer tools console inside the chrome browser

commands:
node: Enter the REPL
.exit: Exit the REPL
You can also use "Control-C" to exit the routine
```

## How to use native Node modules
```
Node comes bundled with built in modules, these are libraries of code
We can use Node.js to get access directly to the local files of the computer

Enter the link below this lecture https://nodejs.org/api/fs.html and acces to the
file system: This helps you interact with the local file system using Node
```
```javascript
//fs stand for file system but you can call this constant whatever you want like "fileSystem"
//And we're going to set it to equal the file system module
//In order to use libraries of code, or modules, or packages inside our project we have to require the module
const fs = require("fs")

//Things that you can do: for example, Specify paths, Open files, Change files, Access and read and wirte to the local file system
//Inside visual studio create a new "file1.txt" wit some random text

//Use method "copyFileSync" in order to create a copy of the file
fs.copyFileSync(src, dest[, mode]) //src, dest[, mode]are parameters "source" and "destination"

const fs = require("fs");
fs.copyFileSync("file1.txt", "file2.txt");
```
```
From the terminal execute the index.js that contains the code, see how a new file2.txt is created
This code will create a new one if there is no "file2.txt" and overwritten if alredy are one
```

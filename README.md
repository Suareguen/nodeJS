# Node Introduction

## Learning Goals

After this lesson, you should be able to:

1. Understand what Node is and why you should use it
2. Learn how to use Node and practice with it
3. Learn about npm and modules and why to use them.
4. Learn how to install packages and use them.

## Prerequisites

- Understand JavaScript fundamentals.

## Introduction
### What’s Node.js?

[Node.js](https://nodejs.org/en) or Node is an open-source **JavaScript runtime environment** developed in 2009 by [Ryan Dahl](https://en.wikipedia.org/wiki/Ryan_Dahl). 

![desc](https://res.cloudinary.com/mypath/image/upload/v1673971639/mypath-assets/199d94ed-132c-412f-a103-855a16974edd/image_gurjcj.png){{{width="auto" height="auto"}}}

Dahl created Node.js because of the synchronous limitations of current web frameworks make it challenging to develop high-performant web servers. Most frameworks make it very difficult to create asynchronous code, so requests are typically blocked until they are entirely resolved.

Node.js allows developers to run JavaScript code on the server-side, enabling the creation of server applications.

However, Node.js changed this by introducing a runtime environment for JavaScript on servers.

In the past, the only runtime environment for JavaScript was the browser. Chrome, Safari, and Internet Explorer had their own JavaScript runtimes, but we could not run JavaScript on our computers outside the browser.

A benefit of Node.js is its underlying engine, [Google's V8 JavaScript engine](https://v8.dev/). V8 is the same engine used by the Chrome browser to execute JavaScript code.

![Untitled](https://github.com/Suareguen/nodeJS/assets/103899316/28b31ec7-9da7-4de7-aefb-3bd041711ed7)
:::tip
A [Runtime environment](https://en.wikipedia.org/wiki/Runtime_system) provides all the necessary tools and features for running a specific program or language.
:::

Typically, a computer's operating system doesn't understand high-level programming languages directly. 

These languages need to be translated into a lower-level format called [bytecode](https://en.wikipedia.org/wiki/Bytecode), which can be understood by the computer. 

This bytecode is then further transformed into machine code, which is the binary code that the computer's processor can execute. Additionally, the runtime environment handles tasks such as [memory management](https://en.wikipedia.org/wiki/Memory_management), file system access, and interaction with the operating system's features.

It's important to note some common misnomers and misconceptions related to Node.js:

- **First**: Node.js is not a framework, although there are frameworks built on top of it (such as Express.js). Node.js itself provides a foundation and runtime for executing JavaScript code on the server-side. 
- **Second**: Node.js is not a new programming language. The programming language remains JavaScript, and Node.js allows JavaScript to be executed outside of the browser environment.

NodeJS is managed by the [OpenJS Foundation](https://openjsf.org/), which includes members such as Github, Coinbase, IBM, Google, Microsoft, etc.

### Why Node.js?


Node.js incorporates [non-blocking I/O](https://nodejs.org/en/docs/guides/blocking-vs-non-blocking) and [event-driven architecture](https://en.wikipedia.org/wiki/Event-driven_architecture) to maintain its lightweight and efficient nature when handling data-intensive real-time applications that span across distributed devices.

One advantage of Node.js for developers already familiar with front-end JavaScript is the lower learning curve.

This reduces the need to learn a completely new programming language or ecosystem, allowing for a smoother transition into back-end development.

Its alignment with front-end JavaScript knowledge and its ability to benefit from ongoing engine advancements make it an attractive choice for developers seeking to build high-performance server-side applications.

Another benefit of Node.js is the use of the V8 engine ( [Google's V8 JavaScript engine](https://v8.dev/) ), mentioned in the previous section, because Google continues to enhance V8 to compete with other JavaScript engines like Mozilla’s SpiderMonkey or Microsoft’s Chakra, Node.js can take advantage of these improvements as well.

Any optimizations, performance enhancements, or language features added to V8 can be utilized by Node.js, resulting in improved performance and compatibility.

:::tip MOST COMMON STACKS FOR WEB DEVELOPMENT:
:::details View More
![desc](https://res.cloudinary.com/mypath/image/upload/v1686911307/mypath-assets/3e30c15a-94d6-4507-a0ca-1a3ccd3997e6/fullstack_cqf3xg.jpg){{{width="auto" height="auto"}}}

:::

## Installing Node JS

We can install Node.js, in Mac or Linux, using `brew` or `apt-get` to install Node, but we’re also going to want to keep Node up to date.

Some projects may use a different version of Node than your own, this can become a hassle to deal with, so what we would suggest doing is installing [Node Version Manager(NVM)](https://github.com/nvm-sh/nvm).

![desc](https://res.cloudinary.com/mypath/image/upload/v1674042987/mypath-assets/199d94ed-132c-412f-a103-855a16974edd/image_w96rvp.png){{{width="auto" height="auto"}}}

NVM allows you to pick which version of Node to use, install new versions, and more.

I'm here to guide you through the installation process of Node.js using Node Version Manager (NVM). Here's a step-by-step explanation:

- Open your terminal ( Ctrl + Alt + T ).

- Install NVM in the terminal, run the following command: 
```bash
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
```

- Close and reopen the terminal ( Ctrl + Alt + T ).

- Verify installation: In the terminal type the code below and press Enter, if a version number is displayed in hte terminal like the image below it means NVM is succesfully installed.
```bash
nvm --version
``` 

![desc](https://res.cloudinary.com/mypath/image/upload/v1686669623/mypath-assets/3e30c15a-94d6-4507-a0ca-1a3ccd3997e6/image_t0fbae.png){{{width="auto" height="auto"}}}

- Installing Node.js with NVM:  In the terminal type and run the following code: 
``` sh
nvm install node
```

- Verify Node.js Installation: In the terminal type the code below in the terminal, press Enter and you should see installed the Node.js version displayed like in the image below.
```sh
node --version
```
![desc](https://res.cloudinary.com/mypath/image/upload/v1686670077/mypath-assets/3e30c15a-94d6-4507-a0ca-1a3ccd3997e6/image_glngu2.png){{{width="auto" height="auto"}}}
- If you want to see the different version of Node.js installed,  type and run the following command in the terminal: 
```sh
nvm ls
```

In the terminal we will see the list of node versions installed in our system:

![desc](https://res.cloudinary.com/mypath/image/upload/v1686674894/mypath-assets/3e30c15a-94d6-4507-a0ca-1a3ccd3997e6/image_q35igc.png){{{width="auto" height="auto"}}}

- Once we see the different Node.js versions, we can choose and use a Node.js version with the following command:
```sh
nvm use <node version>
```

Remember to refer to the official [Documentation](https://github.com/nvm-sh/nvm) and specific instructions for your operating system when installing Node.js or any related tools. 

## First Steps

Now we show you how to run and script with Node.js. Heres’s and step-by-step explanation:
- Create a folder: 
```sh
mkdir folderName
```

- Go inside that folder: 
```sh
cd folderName
```

- Inside that folder create a new file called index.js:
``` sh
touch index.js
```

- Then add the following code in your index.js: 
```js
console.log("Hello from Node")
```

- In your terminal type the following command: 
```sh
node index.js
```

In the terminal we will see something like this:



And that’s all, we’re running with Node.js.

::: details Example
Following the steps above:


Create a folder

```sh
mkdir newProject
```

Go into the folder

``` sh
cd newProject
```

Create an index.js

```sh
touch index.js
```

In your index.js create a `sum` function:
```js
function sum(a, b) {
return a + b
}
const add = sum(1, 3)
console.log(add)
//The result should be 3
```

Run the script with reserved keyword `node` in your terminal
```sh
node index.js
```

When you execute the command ```node index.js``` in your terminal you should see a result like this: 

![desc](https://res.cloudinary.com/mypath/image/upload/v1686671136/mypath-assets/3e30c15a-94d6-4507-a0ca-1a3ccd3997e6/image_mlss0g.png){{{width="auto" height="auto"}}}

:::

We can write any JavaScript code we like in Node, but we must keep in mind there’s no DOM.

## NPM & Modules

[NPM](https://www.npmjs.com/) (Node Package Manager) is a package manager specifically designed for Node.js. It allows you and other developers to easily share JavaScript code by using a command line tool. 

![desc](https://res.cloudinary.com/mypath/image/upload/v1673974750/mypath-assets/199d94ed-132c-412f-a103-855a16974edd/image_pecb8q.png){{{width="auto" height="auto"}}}

With NPM, you can access and download external packages that are part of one of the largest ecosystems in the software development community.
      
      
[Modules](https://www.freecodecamp.org/news/what-are-node-modules/) are bundles of reusable code that are packaged with any dependencies they rely on. 

By using modules, you can organize your code, making it easier to maintain, share, and reuse. The benefits of using modules are numerous, and we will discuss them further shortly.
::: tip Common Challenge
::: details Explanation
One common challenge in managing packages for projects is ensuring compatibility among different versions. 

For example, let's say you and your colleague, Bob, are working on a project together.

You're using version 1.8 of a package, while Bob is using version 1.2. However, these two versions may have significant differences in their code.

When you both try to implement a new feature using this package, it may work on your computer but not on Bob's.

This problem is compounded when there are multiple team members involved. If a package updates, everyone on the team needs to update their version to avoid compatibility issues.
:::


      
      
Fortunately, package managers like npm come to the rescue. It allows you to define the exact version of a package you want to use in your project, ensuring consistency among team members. 

When a package updates, individual team members can choose to update their versions selectively, reducing the risk of breaking changes.
      
      
Furthermore, npm encourages good software development principles and code sharing. Rather than reinventing the wheel for every project, npm enables you to leverage existing packages and modules created by other developers. 

These packages cover a wide range of functionalities, such as coloring text in the terminal, handling command line input, retrieving Chuck Norris jokes, and much more.

 ::: tip  
The fact that npm is already included when you install Node.js is excellent news.
:::


You can verify this by running in the terminal the command:  
```bash
npm --version
``` 

If you receive a version number in response, it confirms that npm is successfully installed and ready to use as we can see in the image below:

![desc](https://res.cloudinary.com/mypath/image/upload/v1686673138/mypath-assets/3e30c15a-94d6-4507-a0ca-1a3ccd3997e6/image_faywpg.png){{{width="auto" height="auto"}}}

By utilizing npm you can streamline your development process, leverage existing code, and adhere to good software development practices. This not only saves time and effort but also contributes to the growth and efficiency of the entire software development community.


## Installing Packages

In order to install packages in our programs we must define our manifest file.
A manifest file is a file that lists out all the packages our program depends on to work. In NPM, this file is called ```package.json```.
```package.json``` defines all of our projects packages and dependencies.

**How to create a package.json?**

When we start a project in first instance we need to create a 
Here’s a guide step-by-step about how t create a ```package.json```:

- Create a directory and go in:
```bash
mkdir newProject 
```
```bash
cd project
```

- Type and run the following command in your terminal: 
```bash
npm init -y
```

```npm init``` create a file called ```package.json``` ([**Manifest File**](https://developer.mozilla.org/en-US/docs/Web/Manifest)) that specifies all of the modules your project will use and ```-y``` acceppt default values for our package.json.

When you run the command above you should see something like this in your ```package.json```:

![desc](https://res.cloudinary.com/mypath/image/upload/v1686734546/mypath-assets/3e30c15a-94d6-4507-a0ca-1a3ccd3997e6/image_f2fyr7.png){{{width="auto" height="auto"}}}

```json
{
  "name": "newproject",
  "version": "1.0.0",
  "description": "",
  "main": "index.js",
  "scripts": {
    "test": "echo \"Error: no test specified\" && exit 1"
  },
  "keywords": [],
  "author": "",
  "license": "ISC"
}
```

And now we have a package.json ready to add packages.

**How to install modules?**

To install modules we use the commands (they are the same):
```bash
npm install
``` 
or 

```bash
npm i
```

For example, let’s install [chalk](https://www.npmjs.com/package/chalk):

![desc](https://res.cloudinary.com/mypath/image/upload/v1686735020/mypath-assets/3e30c15a-94d6-4507-a0ca-1a3ccd3997e6/image_pycogo.png){{{width="auto" height="auto"}}}

Run the following command in your terminal within the folder where the ```package.json``` file is located.

```bash
npm install --save chalk
```

You should see this structure in your project folder:

![desc](https://res.cloudinary.com/mypath/image/upload/v1686734856/mypath-assets/3e30c15a-94d6-4507-a0ca-1a3ccd3997e6/image_a0bayp.png){{{width="auto" height="auto"}}}

This goes to the npm servers and grabs a package called ``` chalk ``` and ``` --save ``` adds this as a dependency to our package.json. In new versions of npm ```--save``` it’s done by default and it isn’t necessary to use.

When you run the npm install command, it retrieves the necessary modules or packages from the npm registry and installs them in your project. 

As a result, it creates a folder called ```node_modules``` within your project directory. This folder serves as a storage location for all the code associated with the installed modules.


After installing a module, you need to require the module in Node.js. This allows you to import the module's functionality into your own codebase. You typically assign the imported module to a variable, allowing you to access its features and functions.

```js
import chalk from 'chalk'

const log = console.log

log(chalk.blue.bgRed.bold("Hello world!"))
```
You should see in your terminal something like this:

![desc](https://res.cloudinary.com/mypath/image/upload/v1686736295/mypath-assets/3e30c15a-94d6-4507-a0ca-1a3ccd3997e6/image_oton29.png){{{width="auto" height="auto"}}}

:::tip
::: details 
Once you have required the module and assigned it to a variable, you can utilize that variable to call upon the module's exposed functions, methods, or properties.
   
By calling the variable and accessing its attached functions, you can leverage the capabilities provided by the module. This enables you to extend your own code's functionality by incorporating the features and utilities offered by the module.

The process involves installing a module using ```npm install```, which creates a ```node_modules``` folder to store the module's code. 

You then require the module in your code, assigning it to a variable. This allows you to access and utilize the module's API, including its functions, methods, or properties, by calling upon the variable and invoking the desired functionality.
:::

:::warning
Please note that the filename is not `index.js` but `index.mjs`. This is due to the fact that in nodeJS, there are two types of modules available:

- **[CJS (CommonJS)](https://nodejs.org/docs/latest/api/modules.html)**: original nodejs system. Uses `require` and `module.exports` to import/export code. If a file has the extension `.cjs`, Node assumes it is commonJS.
- **[ESM (EcmaScript Modules)](https://nodejs.org/docs/latest/api/esm.html)**: newer and default module system in nodejs. It uses `import` and `export` methods. If a file has the extension `.mjs`, nodejs assumes it is ESM.
:::

If you want all the functionality Chalk makes you can visit the [Documentation](https://www.npmjs.com/package/chalk) page.
      
Chalk is one of many npm packages and you feel free to prove many of them and practice.
      
When you commit your updates never commit ` node_modules` folder to git, it will make your repository a lot larger, remember create a [` .gitignore`](https://git-scm.com/docs/gitignore) file to ensure it.

### NPM install

When you clone a repository or takes a project with a ``` package.json``` inside, you only need run the following command in the folder directory: 
```sh
npm install
```
In a Node.js project, when you run ``` npm install```, NPM reads the ``` package.json``` file and installs all the specified dependencies listed within it. This ensures that your project has all the necessary packages and modules to run successfully.

Now, imagine you have a project that relies on several external dependencies, and you want to share your code with others. If you commit only the ``` package.json``` file to your version control system (such as Git), you provide others with a way to recreate the exact set of dependencies you have installed in your project.
      
By sharing only the package.json file, other users can clone your project repository and, with a simple command, restore the ``` node_modules``` folder and install all the necessary dependencies. This command, typically ``` npm install```, reads the ``` package.json``` file and retrieves the specified packages from the npm registry, recreating the ``` node_modules``` folder with the required modules.



This approach has several advantages:
- **Reduced repository size**: By excluding the ``` node_modules``` folder from version control, you avoid bloating your repository with large amounts of code that can be easily obtained through package installation.
- **Consistency and reproducibility**: By relying on the ``` package.json``` file, all users can recreate the same development environment, ensuring consistent behavior across different machines. This is particularly important in collaborative projects or when deploying code to different environments.
- **Simplified updates and maintenance**: By relying on the ``` package.json``` file, users can easily update and manage dependencies by modifying the version ranges specified in the file. Running ``` npm install``` again will install the latest compatible versions of the dependencies.

It's essential to ensure that your ``` package.json``` file accurately reflects the necessary dependencies and version constraints to maintain the stability and compatibility of your project.
## Summary

In this lesson, we have learned what node is, how to install it, how to execute JavaScript files from the console, what NPM is and how to install packages.
- **Node**: What is and how to install.
- What Node Pacakge Manager is.
- **Install packages**: ```npm install packageName```.

## Extra Resources

[NVM Installation](https://www.freecodecamp.org/news/node-version-manager-nvm-install-guide/)
[NPM rank](https://gist.github.com/anvaka/8e8fa57c7ee1350e3491) - updated daily

# Node JS

## Introduction


**What’s Node.js?**

Node.js is an open-source JavaScript runtime environment developed by Ryan Dahl. It allows developers to run JavaScript code on the server-side, enabling the creation of server applications. Traditionally, JavaScript was mainly used within web browsers, with each browser having its own JavaScript runtime. However, Node.js changed this by introducing a runtime environment for JavaScript on servers.
![Node.js image](data:image/png;base64,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)
![OpenAI logo]()


In the past, when JavaScript was limited to browsers, it was not possible to directly run JavaScript code on computers. JavaScript, along with other programming languages like Python, Ruby, or Java, needs a runtime environment to execute. 



A runtime environment provides all the necessary tools and features for running a specific program or language.



Typically, a computer's operating system doesn't understand high-level programming languages directly. These languages need to be translated into a lower-level format called bytecode, which can be understood by the computer. This bytecode is then further transformed into machine code, which is the binary code that the computer's processor can execute. Additionally, the runtime environment handles tasks such as memory management, file system access, and interaction with the operating system's features.




Node.js serves as a runtime environment specifically for JavaScript. It utilizes the V8 JavaScript engine, originally developed for the Chrome browser, and extracts it to create a standalone runtime environment for servers. By leveraging the V8 engine, Node.js can efficiently translate JavaScript programs into bytecode that can be executed by the computer.



It's important to note some common misnomers and misconceptions related to Node.js. First, Node.js is not a framework, although there are frameworks built on top of it (such as Express.js). Node.js itself provides a foundation and runtime for executing JavaScript code on the server-side. Second, Node.js is not a new programming language. The programming language remains JavaScript, and Node.js allows JavaScript to be executed outside of the browser environment.




Node.js has gained significant popularity due to its versatility and performance. It has a vast ecosystem of modules and packages available through NPM (Node Package Manager), allowing developers to easily incorporate third-party libraries into their projects. With Node.js, developers can build scalable and efficient server applications, APIs, real-time applications, and more using JavaScript, promoting code reuse and reducing the need to switch between different languages for server and client development.




By understanding the role of Node.js as a runtime environment and its relationship with the JavaScript language, programmers can leverage its power to create server-side applications efficiently.





**Why Node.js?**


Node.js incorporates non-blocking I/O and event-driven architecture to maintain its lightweight and efficient nature when handling data-intensive real-time applications that span across distributed devices.


Non-blocking I/O, or input/output, is a programming approach that allows multiple I/O operations to be performed concurrently without waiting for each operation to complete before moving on to the next one. In the context of Node.js, this means that when an I/O operation, such as reading from a file or making a network request, is initiated, Node.js doesn't pause the execution of other operations. Instead, it continues to handle other tasks while waiting for the I/O operation to complete. This non-blocking nature enables Node.js to efficiently handle concurrent requests, making it suitable for applications that involve a high volume of I/O operations, such as real-time chat applications or streaming services.




The event-driven architecture of Node.js is closely tied to its non-blocking I/O. In an event-driven model, the flow of the program is determined by events or asynchronous actions. When an event occurs, such as the completion of an I/O operation or a user interaction, Node.js triggers the associated event handler function. This approach allows Node.js to handle multiple events concurrently, ensuring that the application remains responsive even while waiting for I/O operations to complete.



One advantage of Node.js for developers already familiar with front-end JavaScript is the lower learning curve. Since Node.js utilizes JavaScript as its primary language, developers who are proficient in front-end JavaScript can leverage their existing knowledge and apply it to server-side development with Node.js. This reduces the need to learn a completely new programming language or ecosystem, allowing for a smoother transition into back-end development.



Another benefit of Node.js is its underlying engine, Google's V8 JavaScript engine. V8 is the same engine used by the Chrome browser to execute JavaScript code. This shared foundation means that as Google continues to enhance V8 to compete with other JavaScript engines like Mozilla's SpiderMonkey or Microsoft's Chakra, Node.js can take advantage of these improvements as well. Any optimizations, performance enhancements, or language features added to V8 can be utilized by Node.js, resulting in improved performance and compatibility.



By incorporating non-blocking I/O, event-driven architecture, and leveraging the benefits of the V8 engine, Node.js provides an efficient and scalable platform for developing real-time, data-intensive applications. Its alignment with front-end JavaScript knowledge and its ability to benefit from ongoing engine advancements make it an attractive choice for developers seeking to build high-performance server-side applications.






### Installing Node.js

We can install node in Mac or Linux using brew or apt-get to install Node, but we’re also going to want to keep Node up to date.


Some projects may use a different version of Node than your own, this can become a hassle to deal with, so what we would suggest doing is installing Node Version Manager(nvm).
NVM allows you to pick which version of Node to use, install new versions, and more.
I'm here to guide you through the installation process of Node.js using Node Version Manager (NVM). NVM is a helpful tool that allows you to manage multiple Node.js versions on your machine. Here's a step-by-step explanation:
- Open your terminal ( Ctrl + Alt + T ).
- Install NVM: in the terminal, run the following command: curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
- Close and reopen the terminal.
- Verify installation: IN the terminal type '***nvm --version***' and press Enter, if a version number is displayed it means NVM is succesfully installed.
- Installing Node.js with NVM:  In the terminal type and run the following code:
nvm install node
- Verify Node.js Installation: In the terminal type and run ‘node –version’ and you should see installed the Node.js version displayed.
- If you want to see the different version of Node.js installed,  type and run the following command in the terminal: nvm ls
- Once we see the different Node.js versions, now we can use a Node.js version with the following command:
nvm use <node version>

Remember to refer to the official Documentation and specific instructions for your operating system when installing Node.js or any related tools. 


### Our First code
      
Now we show you how to run and script with Node.js. Heres’s and step-by-step explanation:
- Create a folder (‘mkdir folderName’) and inside create a new file called index.js (‘touch index.js’). 
- Then add the following code:  console.log(“Hello from node”)
- In your terminal type the following command: node index.js
And that’s all, we’re running with Node.js.
We can write any JavaScript code we like in Node, but we must keep in mind there’s no DOM.



### Npm and Modules

Npm (Node Package Manager) is a package manager specifically designed for Node.js. It allows you and other developers to easily share JavaScript code by using a command line tool. With npm, you can access and download external packages that are part of one of the largest ecosystems in the software development community. As of now, there are over 35,000 npm modules available for you to utilize in your projects.
      
      
Modules are bundles of reusable code that are packaged with any dependencies they rely on. By using modules, you can organize and compartmentalize your code, making it easier to maintain, share, and reuse. The benefits of using modules are numerous, and we will discuss them further shortly.
One common challenge in managing packages for projects is ensuring compatibility among different versions. For example, let's say you and your colleague, Bob, are working on a project together. You're using version 1.8 of a package, while Bob is using version 1.2. However, these two versions may have significant differences in their code. When you both try to implement a new feature using this package, it may work on your computer but not on Bob's. This problem is compounded when there are multiple team members involved. If a package updates, everyone on the team needs to update their version to avoid compatibility issues.
      
      
Fortunately, package managers like npm come to the rescue. npm helps address this problem by providing version management capabilities. It allows you to define the exact version of a package you want to use in your project, ensuring consistency among team members. When a package updates, individual team members can choose to update their versions selectively, reducing the risk of breaking changes.
      
      
Furthermore, npm encourages good software development principles and code sharing. Rather than reinventing the wheel for every project, npm enables you to leverage existing packages and modules created by other developers. These packages cover a wide range of functionalities, such as coloring text in the terminal, handling command line input, retrieving Chuck Norris jokes, and much more. This approach saves time, promotes code reuse, and fosters collaboration within the development community.
      
The fact that npm is already included when you install Node.js is excellent news. This means that if you have Node.js installed, you automatically have npm available as well. You can verify this by running the command npm --version in the terminal. If you receive a version number in response, it confirms that npm is successfully installed and ready to use.
By utilizing npm and its vast collection of modules, you can streamline your development process, leverage existing code, and adhere to good software development practices. This not only saves time and effort but also contributes to the growth and efficiency of the entire software development community.






### Installing Packages


In order to install packages in our programs we must define our manifest file.
A manifest file is a file that lists out all the packages our program depends on to work. In NPM, this file is called package.json.
Package.json defines all of our projects packages and dependencies.

How to create a package.json?

Here’s a guide step-by-step about how to create it:
- Create a directory and go in: mkdir project – cd project
- Type and run the following command in your terminal: npm init -y. Npm init create a file called package.json ( manifest file ) that specifies all of the modules your project will use and ‘-y’ install default values for our package.json.
And now we have a package.json ready to install packages.

How to install modules?
To install modules we use the command npm install or npm i.

Npm install –save chalk

This goes to the npm servers and grabs a package called “chalk” and’--save’ adds this as a dependency to our package.json. In new versions of npm ‘--save’ it’s done by default and it isn’t necessary to use.

When you run the npm install command, it retrieves the necessary modules or packages from the npm registry and installs them in your project. As a result, it creates a folder called node_modules within your project directory. This folder serves as a storage location for all the code associated with the installed modules.
      
      
After installing a module, you can make use of it in your code. To do so, you need to require the module by using the require keyword in Node.js. This allows you to import the module's functionality into your own codebase. You typically assign the imported module to a variable, allowing you to access its features and functions.
      
      
Once you have required the module and assigned it to a variable, you can utilize that variable to call upon the module's exposed functions, methods, or properties. These functions are often referred to as the module's "API" (Application Programming Interface). The module's API provides a set of predefined functions or behaviors that you can utilize within your own code.
      
      
By calling the variable and accessing its attached functions, you can leverage the capabilities provided by the module. This enables you to extend your own code's functionality by incorporating the features and utilities offered by the module.
      
      
In summary, the process involves installing a module using npm install, which creates a node_modules folder to store the module's code. You then require the module in your code, assigning it to a variable. This allows you to access and utilize the module's API, including its functions, methods, or properties, by calling upon the variable and invoking the desired functionality.
Understanding how to install and utilize modules is crucial for leveraging the extensive ecosystem of npm packages and enhancing your own code with ready-made solutions and features provided by the community.
      
      

If you want all the functionality Chalk makes you can visit the documentation page.
      
      
Normally all packages have a documentation and a nice package wold have a good documentation for people to learn how to use it.
      
      
Chalk is one of many npm packages and you feel free to prove many of them and practice.
      
      
When you commit your updates never commit node_modules folder to git, it will make your repository a lot larger, remember create a .gitignore file to ensure it.
      

When you clone a repository or takes a project with a package.json inside, you only need run the following command in the folder directory: 
npm install 
In a Node.js project, the package.json file serves as a manifest or configuration file that defines various aspects of your project, including its dependencies. When you run npm install, npm reads the package.json file and installs all the specified dependencies listed within it. This ensures that your project has all the necessary packages and modules to run successfully.
Now, imagine you have a project that relies on several external dependencies, and you want to share your code with others. If you commit only the package.json file to your version control system (such as Git), you provide others with a way to recreate the exact set of dependencies you have installed in your project.
      
      
      
By sharing only the package.json file, other users can clone your project repository and, with a simple command, restore the node_modules folder and install all the necessary dependencies. This command, typically npm install, reads the package.json file and retrieves the specified packages from the npm registry, recreating the node_modules folder with the required modules.
This approach has several advantages:
- Reduced repository size: By excluding the node_modules folder from version control, you avoid bloating your repository with large amounts of code that can be easily obtained through package installation.
- Consistency and reproducibility: By relying on the package.json file, all users can recreate the same development environment, ensuring consistent behavior across different machines. This is particularly important in collaborative projects or when deploying code to different environments.
- Simplified updates and maintenance: By relying on the package.json file, users can easily update and manage dependencies by modifying the version ranges specified in the file. Running npm install again will install the latest compatible versions of the dependencies.
      
      

It's worth noting that while sharing only the package.json file is convenient for managing dependencies, it assumes that the project adheres to good practices in terms of dependency management.
      
It's essential to ensure that your package.json file accurately reflects the necessary dependencies and version constraints to maintain the stability and compatibility of your project.
      
In conclusion, by committing only the package.json file to your repository, you allow other users to recreate the node_modules folder and install the required dependencies easily. This approach promotes consistency, reproducibility, and simplified dependency management across different environments and collaborators.

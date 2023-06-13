# nodeJS

Node JS

Introduction


What’s Node.js?

Node.js is an open-source JavaScript runtime environment developed by Ryan Dahl. It allows developers to run JavaScript code on the server-side, enabling the creation of server applications. Traditionally, JavaScript was mainly used within web browsers, with each browser having its own JavaScript runtime. However, Node.js changed this by introducing a runtime environment for JavaScript on servers.
In the past, when JavaScript was limited to browsers, it was not possible to directly run JavaScript code on computers. JavaScript, along with other programming languages like Python, Ruby, or Java, needs a runtime environment to execute. A runtime environment provides all the necessary tools and features for running a specific program or language.
Typically, a computer's operating system doesn't understand high-level programming languages directly. These languages need to be translated into a lower-level format called bytecode, which can be understood by the computer. This bytecode is then further transformed into machine code, which is the binary code that the computer's processor can execute. Additionally, the runtime environment handles tasks such as memory management, file system access, and interaction with the operating system's features.
Node.js serves as a runtime environment specifically for JavaScript. It utilizes the V8 JavaScript engine, originally developed for the Chrome browser, and extracts it to create a standalone runtime environment for servers. By leveraging the V8 engine, Node.js can efficiently translate JavaScript programs into bytecode that can be executed by the computer.
It's important to note some common misnomers and misconceptions related to Node.js. First, Node.js is not a framework, although there are frameworks built on top of it (such as Express.js). Node.js itself provides a foundation and runtime for executing JavaScript code on the server-side. Second, Node.js is not a new programming language. The programming language remains JavaScript, and Node.js allows JavaScript to be executed outside of the browser environment.
Node.js has gained significant popularity due to its versatility and performance. It has a vast ecosystem of modules and packages available through NPM (Node Package Manager), allowing developers to easily incorporate third-party libraries into their projects. With Node.js, developers can build scalable and efficient server applications, APIs, real-time applications, and more using JavaScript, promoting code reuse and reducing the need to switch between different languages for server and client development.
By understanding the role of Node.js as a runtime environment and its relationship with the JavaScript language, programmers can leverage its power to create server-side applications efficiently.





Why Node.js?


Node.js incorporates non-blocking I/O and event-driven architecture to maintain its lightweight and efficient nature when handling data-intensive real-time applications that span across distributed devices.
Non-blocking I/O, or input/output, is a programming approach that allows multiple I/O operations to be performed concurrently without waiting for each operation to complete before moving on to the next one. In the context of Node.js, this means that when an I/O operation, such as reading from a file or making a network request, is initiated, Node.js doesn't pause the execution of other operations. Instead, it continues to handle other tasks while waiting for the I/O operation to complete. This non-blocking nature enables Node.js to efficiently handle concurrent requests, making it suitable for applications that involve a high volume of I/O operations, such as real-time chat applications or streaming services.
The event-driven architecture of Node.js is closely tied to its non-blocking I/O. In an event-driven model, the flow of the program is determined by events or asynchronous actions. When an event occurs, such as the completion of an I/O operation or a user interaction, Node.js triggers the associated event handler function. This approach allows Node.js to handle multiple events concurrently, ensuring that the application remains responsive even while waiting for I/O operations to complete.
One advantage of Node.js for developers already familiar with front-end JavaScript is the lower learning curve. Since Node.js utilizes JavaScript as its primary language, developers who are proficient in front-end JavaScript can leverage their existing knowledge and apply it to server-side development with Node.js. This reduces the need to learn a completely new programming language or ecosystem, allowing for a smoother transition into back-end development.
Another benefit of Node.js is its underlying engine, Google's V8 JavaScript engine. V8 is the same engine used by the Chrome browser to execute JavaScript code. This shared foundation means that as Google continues to enhance V8 to compete with other JavaScript engines like Mozilla's SpiderMonkey or Microsoft's Chakra, Node.js can take advantage of these improvements as well. Any optimizations, performance enhancements, or language features added to V8 can be utilized by Node.js, resulting in improved performance and compatibility.
By incorporating non-blocking I/O, event-driven architecture, and leveraging the benefits of the V8 engine, Node.js provides an efficient and scalable platform for developing real-time, data-intensive applications. Its alignment with front-end JavaScript knowledge and its ability to benefit from ongoing engine advancements make it an attractive choice for developers seeking to build high-performance server-side applications.






Installing Node.js

We can install node in Mac or Linux using brew or apt-get to install Node, but we’re also going to want to keep Node up to date.
Some projects may use a different version of Node than your own, this can become a hassle to deal with, so what we would suggest doing is installing Node Version Manager(nvm).
NVM allows you to pick which version of Node to use, install new versions, and more.
I'm here to guide you through the installation process of Node.js using Node Version Manager (NVM). NVM is a helpful tool that allows you to manage multiple Node.js versions on your machine. Here's a step-by-step explanation:
      - Open your terminal ( Ctrl + Alt + T ).
      - Install NVM: in the terminal, run the following command: 
      curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash
- Close and reopen the terminal.
- Verify installation: IN the terminal type ‘nvm –version’ and press Enter, if a version number is displayed it means NVM is succesfully installed.
- Installing Node.js with NVM:  In the terminal type and run the following code:
nvm install node
- Verify Node.js Installation: In the terminal type and run ‘node –version’ and you should see installed the Node.js version displayed.
- If you want to see the different version of Node.js installed,  type and run the following command in the terminal: nvm ls
- Once we see the different Node.js versions, now we can use a Node.js version with the following command:
nvm use <node version>

Remember to refer to the official Documentation and specific instructions for your operating system when installing Node.js or any related tools. 


Our First code
Now we show you how to run and script with Node.js. Heres’s and step-by-step explanation:
- Create a folder (‘mkdir folderName’) and inside create a new file called index.js (‘touch index.js’). 
- Then add the following code:  console.log(“Hello from node”)
- In your terminal type the following command: node index.js
And that’s all, we’re running with Node.js.
We can write any JavaScript code we like in Node, but we must keep in mind there’s no DOM.








Npm and Modules

Npm (Node Package Manager) is a package manager specifically designed for Node.js. It allows you and other developers to easily share JavaScript code by using a command line tool. With npm, you can access and download external packages that are part of one of the largest ecosystems in the software development community. As of now, there are over 35,000 npm modules available for you to utilize in your projects.
Modules are bundles of reusable code that are packaged with any dependencies they rely on. By using modules, you can organize and compartmentalize your code, making it easier to maintain, share, and reuse. The benefits of using modules are numerous, and we will discuss them further shortly.
One common challenge in managing packages for projects is ensuring compatibility among different versions. For example, let's say you and your colleague, Bob, are working on a project together. You're using version 1.8 of a package, while Bob is using version 1.2. However, these two versions may have significant differences in their code. When you both try to implement a new feature using this package, it may work on your computer but not on Bob's. This problem is compounded when there are multiple team members involved. If a package updates, everyone on the team needs to update their version to avoid compatibility issues.
Fortunately, package managers like npm come to the rescue. npm helps address this problem by providing version management capabilities. It allows you to define the exact version of a package you want to use in your project, ensuring consistency among team members. When a package updates, individual team members can choose to update their versions selectively, reducing the risk of breaking changes.
Furthermore, npm encourages good software development principles and code sharing. Rather than reinventing the wheel for every project, npm enables you to leverage existing packages and modules created by other developers. These packages cover a wide range of functionalities, such as coloring text in the terminal, handling command line input, retrieving Chuck Norris jokes, and much more. This approach saves time, promotes code reuse, and fosters collaboration within the development community.
The fact that npm is already included when you install Node.js is excellent news. This means that if you have Node.js installed, you automatically have npm available as well. You can verify this by running the command npm --version in the terminal. If you receive a version number in response, it confirms that npm is successfully installed and ready to use.
By utilizing npm and its vast collection of modules, you can streamline your development process, leverage existing code, and adhere to good software development practices. This not only saves time and effort but also contributes to the growth and efficiency of the entire software development community.






Installing Packages


In order to install packages in our programs we must define our manifest file.
A manifest file is a file that lists out all the packages our program depends on to work. In NPM, this file is called package.json.
Package.json defines all of our projects packages and dependencies.

How to create a package.json?

Here’s a guide step-by-step about how to create it:
 -Create a directory and go in: mkdir project – cd project
- Type and run the following command in your terminal: npm init -y. Npm init create a file called package.json ( manifest file ) that specifies all of the modules your project will use and ‘-y’ install default values for our package.json.
And now we have a package.json ready to install packages.

How to install modules?
To install modules we use the command npm install or npm i.

Npm install –save chalk

This 

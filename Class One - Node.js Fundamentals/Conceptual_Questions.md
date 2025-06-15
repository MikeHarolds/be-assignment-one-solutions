# Conceptual Questions



### 1. What is NPM and what role does it play in Node.js development?

NPM stands for **Node Package Manager**, and it comes installed automatically when you install Node.js. As a developer, NPM is super useful because it allows you to install and manage third-party libraries (called packages) that help you build apps faster.

Instead of writing everything from scratch, you can just install useful packages with one command like `npm install express`. It also helps manage versions of your packages through the `package.json` file, so your project remains organized and other developers can easily know what packages are used.

NPM also has a huge online registry where developers publish and share their code with others.

**Reference:** [https://docs.npmjs.com/about-npm](https://docs.npmjs.com/about-npm)



### 2. Why is Node.js considered cross-platform, and what are the benefits of this feature?

Node.js is considered **cross-platform** because you can write your code once and run it on different operating systems like Windows, macOS, and Linux without changing it. This is made possible because Node.js is built using C++ and runs on top of Google’s V8 engine.

The main benefit is flexibility. For example, if I develop a web app using Node.js on my Windows laptop, it can still run on a Linux server when I deploy it. This helps teams that use different devices and also saves time, since you don’t have to rebuild your code for each OS.

**Reference:** [https://nodejs.dev/en/learn/introduction-to-nodejs](https://nodejs.dev/en/learn/introduction-to-nodejs)



### 3. What are built-in modules in Node.js, and why are they important?

Built-in modules are modules that come with Node.js. You don’t need to install them with NPM—they are ready to use. Some common ones are `http` (for creating servers), `fs` (for file system stuff), and `path` (for working with file paths).

They are important because they allow you to build basic server functionalities quickly without downloading anything extra. For example, using the `http` module, you can create a simple web server in just a few lines. This saves time and keeps your project lightweight.

**Reference:** [https://nodejs.org/api/](https://nodejs.org/api/)


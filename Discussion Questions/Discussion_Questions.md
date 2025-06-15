# Discussion Questions

## Node.js
### 1. How does Node.js's single-threaded nature affect its performance and scalability?

Node.js uses a **single-threaded event loop**, which means it can handle many connections at once without starting a new thread for each one. This makes it super **fast and memory-efficient**, especially for I/O-heavy apps like chats or APIs.

However, it's not the best for **CPU-heavy tasks** (like image processing) because one heavy task can block everything else.



### 2. What are the advantages and disadvantages of using an event-driven architecture?

**Advantages:**

* Handles many users at once without slowing down.
* Great for real-time apps like messaging or live dashboards.
* Uses less system resources.

**Disadvantages:**

* Can be tricky to debug or manage if too many events are firing.
* Makes code harder to read if you don’t structure it well (callback hell).

It’s good for apps with lots of network or file operations.



### 3. How does Node.js's non-blocking I/O model benefit web applications?

Node.js uses **non-blocking I/O**, meaning it doesn’t wait for one task (like reading a file) to finish before starting the next. Instead, it continues running other code and handles the result later using callbacks or promises.

This makes web apps **faster and more responsive**, especially when handling many users at once, like in APIs or streaming apps.

---
## Version Control


### 1. Why is version control important in software development?

Version control is important because it helps keep track of every change made to the code. It allows you to go back to previous versions, fix mistakes, and see who made what change. It also prevents losing code and helps manage updates in a clean and organized way.



### 2. How does version control help in team collaboration?

It allows many developers to work on the same project without clashing. Each person can work on their own branch, and changes can be reviewed before merging. This makes teamwork smooth, avoids code overwrites, and keeps everyone in sync.



### 3. What are the best practices for organizing a Git repository?

* Use clear folder structures (e.g., `src/`, `assets/`, `docs/`)
* Write helpful commit messages
* Always use branches for features or fixes
* Keep the `main` branch stable
* Use `.gitignore` to avoid tracking unwanted files
* Keep README updated

These makes project clean, easy to manage, and team-friendly.

---

## Combined Concepts


### 1. How would you explain the relationship between Node.js and version control in a development workflow?

Node.js is used to build the app, while version control (like Git) is used to track changes in the Node.js project. Together, they help you build and manage your app smoothly—Node.js handles the logic, and Git makes sure you don’t lose track of what’s been changed or by who.



### 2. What are the key considerations when setting up a new Node.js project with version control?

* Initialize Git first using `git init`
* Run `npm init` to create `package.json`
* Add `node_modules/` to `.gitignore` so it’s not tracked
* Create a clear folder structure
* Make the first commit with a message like `Initial commit`

This setup keeps the project clean and trackable from day one.



### 3. How can version control help in managing Node.js dependencies?

Instead of tracking all the installed packages, Git only tracks the `package.json` and `package-lock.json` files. These files list all dependencies and their versions. So when someone else clones your repo, they can run `npm install` to get the exact same setup. This keeps the app consistent across all devices.


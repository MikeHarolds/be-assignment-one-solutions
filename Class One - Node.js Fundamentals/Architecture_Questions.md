# Architecture Questions



### 1. How does Node.js handle multiple concurrent connections despite being single-threaded?

Node.js uses an event loop and non-blocking I/O to handle many connections at once. Even though it's single-threaded, it doesn’t wait for one task to finish before moving to the next. Instead, it listens for events and handles tasks like file reads or database queries in the background.

**Reference:** [https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/)



### 2. Explain the concept of non-blocking I/O in Node.js and provide an example of when it's beneficial.

Non-blocking I/O means Node.js doesn’t wait for tasks like reading files or fetching data to finish before moving on. It continues running other code while waiting. This is useful in web apps where many users make requests at once, like a chat app or live sports update site.

**Reference:** [https://nodejs.dev/en/learn/understanding-asynchronous-programming-in-nodejs/](https://nodejs.dev/en/learn/understanding-asynchronous-programming-in-nodejs/)



### 3. What is the event-driven architecture in Node.js and how does it contribute to its efficiency?

Node.js runs on an event-driven system, which means it reacts to events like clicks, data arrival, or timers. It uses an event loop to manage these actions. This makes it efficient and responsive, especially for apps that do a lot of I/O like APIs or messaging platforms.

**Reference:** [https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/](https://nodejs.org/en/docs/guides/event-loop-timers-and-nexttick/)

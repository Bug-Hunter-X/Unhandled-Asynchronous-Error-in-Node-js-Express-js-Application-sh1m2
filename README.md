# Unhandled Asynchronous Error in Node.js Express.js Application

This repository demonstrates a common error in Node.js applications involving unhandled asynchronous errors.  The example shows how an error thrown within an asynchronous operation in an Express.js route handler can cause the application to crash without proper error handling.

## Bug Description
The `bug.js` file contains a simple Express.js application.  A route handler simulates an asynchronous operation (using `setTimeout`) that randomly throws an error. If the error occurs, it's not caught, leading to an unhandled exception and application crash.

## Solution
The `bugSolution.js` file demonstrates the correct way to handle such asynchronous errors using `try...catch` blocks or async/await and error handling.

## How to Reproduce the Bug
1. Clone this repository.
2. Navigate to the directory containing `bug.js`.
3. Run the application using `node bug.js`.
4. Refresh the page several times until you encounter a server crash caused by the unhandled exception.

## How to Fix the Bug
Refer to `bugSolution.js` for a demonstration of proper error handling.  The key is to use a `try...catch` block or async/await with appropriate error handling within your asynchronous operations.
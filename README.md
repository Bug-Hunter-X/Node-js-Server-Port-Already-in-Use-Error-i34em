# Node.js Server Port Already in Use Error

This repository demonstrates a common error in Node.js: attempting to start a server on a port that is already in use.  The `bug.js` file shows the problematic code, while `bugSolution.js` provides a robust solution.

## Problem

The `bug.js` file creates an HTTP server and attempts to listen on port 8080. If another process is already using this port, the server will throw an error and crash.

## Solution

The `bugSolution.js` file addresses this issue by using the `'error'` event listener of the `http.Server` object.  This listener captures the error and handles it gracefully, preventing the application from crashing.
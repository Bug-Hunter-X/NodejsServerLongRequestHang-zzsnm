# Node.js Server Hang Issue

This repository demonstrates a common issue in Node.js where a long-running request can cause the server to become unresponsive.  The `server.js` file contains the buggy code, while `serverSolution.js` provides a solution using asynchronous operations.

## Problem

The server uses a `while` loop to simulate a long-running task. During this time, the event loop is blocked, preventing the server from accepting new requests.  This results in a unresponsive server.

## Solution

The solution involves using asynchronous programming techniques, such as promises or async/await, to handle long-running tasks without blocking the event loop.  This ensures that the server remains responsive to new requests, even while processing long-running ones.

## How to run

1. Clone this repository.
2. Run `node server.js` to see the hanging issue.
3. Run `node serverSolution.js` to see the solution in action.
# Express.js Server Unresponsiveness Under Load

This repository demonstrates a common issue in Express.js applications where the server becomes unresponsive under heavy load or when dealing with asynchronous operations that take longer than expected.  The problem stems from a lack of proper error handling and asynchronous flow management. The `bug.js` file demonstrates the problem and `bugSolution.js` shows the solution.

## Problem Description:

The provided `bug.js` code uses `setTimeout` to simulate an asynchronous operation.  Under normal conditions, this works fine; however, if multiple requests arrive concurrently, the server might not be able to handle them efficiently, leading to some requests timing out.

## Solution:

The `bugSolution.js` file introduces a solution using techniques for better handling of asynchronous operations. This improves responsiveness under load.
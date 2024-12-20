# React useEffect Cleanup Function Unexpected Behavior

This repository demonstrates a common issue with React's `useEffect` hook:  incorrect cleanup function execution. The example shows a component where the cleanup function is not behaving as expected, leading to potential performance problems or memory leaks.

## The Problem
The provided code shows a `useEffect` hook with a cleanup function. However, the cleanup function does not always run when anticipated. This often happens due to improper use of the dependency array or component lifecycle events.

## The Solution
The solution is to ensure correct implementation and use of the dependency array in `useEffect`.  A correctly implemented dependency array ensures the effect runs only when the values in the array change. A proper cleanup function releases resources and prevents unexpected behaviors.

## How to reproduce
1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`. 
4. Observe the console logs to see the effect and cleanup function executions. Note the unexpected behavior in `bug.js`
5. Compare with the corrected version in `bugSolution.js`

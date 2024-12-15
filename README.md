# Unnecessary Re-renders in React useEffect Hook

This repository demonstrates a common React bug involving the `useEffect` hook.  The provided `bug.js` file showcases a scenario where the `useEffect` hook re-renders unnecessarily, leading to performance issues. The solution, found in `bugSolution.js`, addresses this by correctly specifying the dependencies array. 

## Bug Description

The `useEffect` hook in the `bug.js` file is missing a dependency array.  As a result, it runs after every render, causing unnecessary console logs and potential performance problems. This is particularly impactful in applications with frequent state updates.

## Solution

The `bugSolution.js` file provides a corrected version. By including `[count]` as the dependency array, the `useEffect` hook only runs when the `count` variable changes, significantly improving performance. 

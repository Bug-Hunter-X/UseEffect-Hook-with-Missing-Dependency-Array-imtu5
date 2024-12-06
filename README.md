# React useEffect Hook with Missing Dependency Array

This repository demonstrates a common error in React applications involving the `useEffect` hook.  When the dependency array is omitted or incorrect, the effect runs after every render, leading to an infinite loop or unexpected behavior. This example shows how to correctly use the dependency array to prevent this.

## Bug Description
The `useEffect` hook in `bug.js` is missing a dependency array. This causes the effect to run after every render, which in turn leads to the `console.log` statement being executed repeatedly. This example showcases the issue with the console being spammed and performance degradation. 

## Solution
The `bugSolution.js` file shows the correct way to use `useEffect`, using the dependency array `[count]` to ensure the effect only runs when `count` changes.
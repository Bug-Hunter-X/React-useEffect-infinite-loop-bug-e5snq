# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by a missing dependency in the effect's dependency array. 

## The Bug

The `bug.js` file contains a component that uses `useEffect` to log the current count.  However, the dependency array `[count]` is missing, causing the effect to run on every render, leading to an infinite loop of updates. 

## The Solution

The `bugSolution.js` file shows the correct implementation where the dependency array is included, preventing the infinite loop.
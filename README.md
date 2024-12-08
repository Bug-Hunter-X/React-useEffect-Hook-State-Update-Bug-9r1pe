# React useEffect Hook State Update Bug
This repository demonstrates a common error in React applications when working with the `useEffect` hook and state updates.  The issue arises from directly manipulating a state variable within the `useEffect` hook, without using the state setter function.  This leads to unexpected behavior and no re-render, as React's state update mechanism isn't triggered.

## Problem
The `bug.js` file contains a component that uses the `useState` hook to manage a counter. A `useEffect` hook attempts to increment the counter directly, bypassing the `setCount` function.  This results in the counter not updating correctly when the component is rendered. 

## Solution
The `bugSolution.js` file corrects this issue by using the `setCount` function provided by `useState` to update the state. This ensures that React's state management system is correctly informed, leading to the UI updating accordingly.  This is the crucial method of managing states within React components.

## How to run the example
1. Clone the repository
2. Navigate to the project folder in your terminal
3. Run `npm install`
4. Run `npm start`
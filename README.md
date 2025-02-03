# React 19 useEffect Infinite Render Loop

This repository demonstrates a common bug in React 19 involving infinite render loops within the `useEffect` hook.  The bug arises from the improper use of the dependency array, leading to unnecessary re-renders and potential application crashes.

## Bug Description

The `useEffect` hook, without a proper dependency array, runs after every render. If the effect modifies state or props that trigger re-renders, an infinite loop is created. This example showcases this issue and its solution.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the console logs and the application behavior.

## Solution

The provided solution shows how to fix this by correctly specifying the dependency array in the `useEffect` hook.
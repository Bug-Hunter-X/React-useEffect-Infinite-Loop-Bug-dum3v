# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications where an infinite loop occurs within the `useEffect` hook.  The bug stems from incorrectly updating state within the dependency array, causing the effect to run repeatedly and infinitely.

## Bug Description
The `MyComponent` uses `useEffect` to increment a counter. However, because the state update is within the `useEffect`'s dependency array, this will create an infinite loop.
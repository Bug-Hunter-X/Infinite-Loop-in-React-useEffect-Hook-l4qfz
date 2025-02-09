# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by missing dependency array.  The `useEffect` hook, without a dependency array, runs after every render, creating a cycle where state updates trigger re-renders, which in turn trigger more `useEffect` calls.
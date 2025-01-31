# React useEffect Hook Memory Leak
This repository demonstrates a common error in React applications involving the `useEffect` hook and memory leaks.  The provided code shows an example of how to cause a memory leak and how to properly fix it using the cleanup function in useEffect hook.

## Problem
The `setInterval` function within the `useEffect` hook is not properly cleaned up when the component unmounts. This leads to the interval continuing to run indefinitely in the background, consuming resources and potentially causing unexpected behavior or memory leaks.
# React useEffect Cleanup Function Issue

This repository demonstrates a common issue related to React's `useEffect` hook where the cleanup function isn't always triggered as expected.  The example showcases a scenario where the cleanup function should run when the component unmounts or before the next effect is triggered, but doesn't always behave as intended.

## Problem

The provided code demonstrates a simple counter component that uses `useEffect` to log changes to the count. The cleanup function is intended to log a message before the next effect runs or when the component is unmounted.  However, under certain circumstances (rapid state changes, component re-renders, etc), the cleanup function might be skipped.

## Solution

The solution focuses on ensuring the cleanup function executes reliably.  A common approach to handle this involves carefully considering dependencies and using techniques to guarantee cleanup. The solution addresses the problem by using a more robust cleanup mechanism that reliably executes when needed. 

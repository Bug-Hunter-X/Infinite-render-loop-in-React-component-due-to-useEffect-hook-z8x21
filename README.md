# React Infinite Render Loop Bug

This repository demonstrates a common React bug: an infinite render loop caused by an incorrectly used `useEffect` hook.  The `useEffect` hook, without a dependency array, triggers after every render, leading to an endless cycle of updates.

## Bug Description

The `MyComponent` component uses `useState` to track a count. The `useEffect` hook logs the count to the console. However, the lack of dependency array causes the effect to run every time, leading to an infinite rendering cycle and potentially crashing the application.
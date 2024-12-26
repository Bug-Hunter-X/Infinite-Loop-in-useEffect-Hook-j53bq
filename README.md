# Infinite Loop in useEffect Hook
This example demonstrates a common mistake when using the `useEffect` hook in React.  Improper use of the dependencies array can lead to unexpected behavior, such as infinite loops.

## Bug Description
The provided `MyComponent` uses the `useEffect` hook without a dependencies array (`[]`). This means the effect runs after every render, leading to an infinite render loop. Each render triggers the effect, causing another render, creating a cycle.
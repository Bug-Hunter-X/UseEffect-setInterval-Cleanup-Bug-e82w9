# useEffect setInterval Cleanup Bug
This example demonstrates a common bug in React: using setInterval within useEffect without providing a cleanup function. This results in memory leaks as the interval continues to run even after the component unmounts.

The bug.js file contains the buggy code, and bugSolution.js provides a solution.

## How to reproduce
1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the count continuously increasing even after unmounting the component. This indicates a memory leak caused by the uncleaned setInterval.
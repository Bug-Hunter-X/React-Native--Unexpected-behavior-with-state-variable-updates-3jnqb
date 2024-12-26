# React Native: Unexpected behavior with state variable updates

This repository demonstrates a common error in React Native development: directly modifying state variables outside the `useState`'s `setState` function. This can lead to unexpected behavior and make debugging difficult.

## Bug Description
The provided `bug.js` demonstrates incorrect state management. The `incrementCount` function attempts to increment the `count` variable directly without using `setCount`. This causes React to not re-render the component correctly, resulting in the UI not reflecting the actual state change.

## Solution
The `bugSolution.js` demonstrates the correct way to update state variables.  The `incrementCount` function now uses `setCount` to update the state, triggering a re-render and correctly updating the UI.

## How to Run
1. Clone the repository.
2. Run `npm install` to install the dependencies.
3. Run `npx react-native run-android` or `npx react-native run-ios` to run the app on an emulator or physical device.
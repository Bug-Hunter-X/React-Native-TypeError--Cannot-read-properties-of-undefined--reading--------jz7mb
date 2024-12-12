# React Native TypeError: Cannot read properties of undefined (reading '...')

This repository demonstrates a common error in React Native applications: the `TypeError: Cannot read properties of undefined (reading '...')` error. This error arises when attempting to access a property of an object that is currently `null` or `undefined`.  The solution showcases best practices for preventing this error.

## Problem
The problem is that asynchronous operations, such as fetching data from an API, may not have completed when the component attempts to render. Thus, trying to access properties on the not-yet-loaded data causes an error.

## Solution
The solution employs optional chaining (`?.`) and the nullish coalescing operator (`??`) to gracefully handle the situation where the data is not yet available. Optional chaining safely accesses properties only if the object exists, while nullish coalescing provides a default value if the property is `null` or `undefined`.

## How to run
1. Clone the repo
2. `npm install`
3. `npx react-native run-android` or `npx react-native run-ios`
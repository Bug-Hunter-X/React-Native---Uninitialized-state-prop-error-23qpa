# React Native - Uninitialized State/Prop Error

This repository demonstrates a common error in React Native applications: accessing state or props before they have been initialized.  This often occurs in asynchronous operations (like API calls) where the data might not be available immediately.

The `bug.js` file shows the problematic code. The `bugSolution.js` file provides a corrected implementation using optional chaining and a default value to handle potential undefined values.

## Steps to Reproduce

1. Clone the repository.
2. Run `npm install`.
3. Run the app on a simulator or device.
4. Observe the error in the console (in `bug.js`) and the corrected behavior in `bugSolution.js`.

## Solution

The solution utilizes optional chaining (`?.`) to safely access the property only if it exists, and provides a default value in case it's undefined.
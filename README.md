# AsyncStorage getItem Promise Handling Error in React Native

This repository demonstrates a common error encountered when using AsyncStorage in React Native: incorrectly handling the promise returned by `getItem`.  The provided code showcases the error and its solution.

## Problem

The `AsyncStorage.getItem` method is asynchronous; it returns a promise that resolves with the stored value.  If you try to access the value directly without awaiting the promise, you'll get a promise object instead of the actual value, leading to unexpected behavior or crashes.

## Solution

The solution involves correctly handling the promise using `.then()` to access the value once the promise resolves.  Error handling with `.catch()` is also crucial for robustness.

## Usage

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install` to install dependencies.
4. Run the app using your preferred React Native development tools.

Observe the differences between the incorrect and correct usage within the code samples.
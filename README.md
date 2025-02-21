# React Native FlatList: Missing keyExtractor
This repository demonstrates a common error in React Native when using FlatList or SectionList components: forgetting to include the `keyExtractor` prop.

The `keyExtractor` prop is essential for efficient rendering and data management.  Without it, React Native will issue a warning or potentially crash if your data changes because it cannot identify and update each item efficiently.

## Bug
The `bug.js` file shows a FlatList implementation missing the `keyExtractor` prop.  This will result in warnings and performance issues.

## Solution
The `bugSolution.js` file demonstrates the correct implementation, including the `keyExtractor` prop to provide unique keys for each item in the FlatList.

## How to run
1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run `npx react-native run-android` or `npx react-native run-ios`.
# Unhandled Promise Rejection in React Native FlatList

This repository demonstrates a common issue in React Native: unhandled promise rejections when using FlatList to display data fetched from an API.

The bug is caused by a missing error handling mechanism within the `useEffect` hook which fetches the data.  When the API request fails, the promise rejects, leading to a crash without informative error message in the app UI.

The solution demonstrates proper error handling using a `try...catch` block and displaying appropriate error messages to the user.
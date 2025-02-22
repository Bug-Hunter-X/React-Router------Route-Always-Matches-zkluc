# React Router: '*' Route Always Matches

This repository demonstrates a common issue in React Router v6 where the catch-all route ('*') always matches, overriding other defined routes. This occurs even when more specific routes are defined before the catch-all route.  The solution involves carefully considering the order and specificity of routes.

## Bug
The bug is present in `bug.js`.  The `*` route always matches, regardless of the URL.

## Solution
The solution is provided in `bugSolution.js`. The issue is resolved by properly ordering routes and making sure that more specific routes are matched before the catch-all.  In this example, adding a path parameter to handle additional routes fixes this issue.
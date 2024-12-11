# React Router Dom v6 Nested Route Bug

This repository demonstrates a bug in React Router Dom v6 where nested routes are not correctly rendered. The catch-all route (`/*`) matches even when a more specific route should be active.  This issue occurs even with seemingly correct route definitions.

## How to Reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe that navigating to `/about` still shows the 'Not Found' component instead of the 'About' component.

## Solution

The solution involves using the `useLocation` hook to correctly handle nested routes, as shown in `bugSolution.js`.
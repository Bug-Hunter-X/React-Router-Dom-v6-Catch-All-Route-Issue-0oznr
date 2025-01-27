# React Router Dom v6 Catch-All Route Issue

This repository demonstrates a common issue encountered when using catch-all routes (`/*`) in React Router Dom v6.  The catch-all route incorrectly intercepts all requests, even if a more specific route should match first. 

The solution provided demonstrates how to correctly order routes to ensure that more specific routes are matched before the catch-all.

## Problem:
The `/*` route in the original `App.js` file always matches, regardless of the URL.  This prevents other routes from ever being triggered.

## Solution:
The `AppSolution.js` file shows the corrected route order.  By placing the catch-all route at the very end of the `Routes` component, the more specific routes have priority and are matched before the catch-all.
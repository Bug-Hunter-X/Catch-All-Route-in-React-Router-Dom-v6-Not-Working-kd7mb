# Catch All Route Issue in React Router Dom v6

This repository demonstrates a problem with the catch-all route (`*`) in React Router DOM v6.  The catch-all route is intended to render a component when no other route matches, but in this case, it's not working as expected.

## Problem Description

When navigating to an invalid path, the catch-all route component (`NotFound`) does not render.  Other routes are working correctly.

## Solution

The issue is resolved by ensuring the catch-all route is placed as the last route in the Routes component.  This ensures it acts as a true fallback for any unmatched paths.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Navigate to an invalid path (e.g., `/invalid-path`).  The `NotFound` component should render.
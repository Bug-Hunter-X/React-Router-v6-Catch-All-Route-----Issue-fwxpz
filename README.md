# React Router v6 Catch-All Route Issue

This repository demonstrates a common issue encountered when using the catch-all route ('*') in React Router v6.  The issue is that the catch-all route, intended to handle all non-matching routes, doesn't seem to work correctly under certain circumstances.

## Problem

The `App.js` file shows a basic React Router setup. When you navigate to a non-existent route, the `NotFound` component should render.  However, in this case, it may not render as expected, instead possibly showing a blank screen or the previously visited page.

## Solution

The `AppSolution.js` file provides a solution by ensuring the catch-all route is placed as the last route within the `<Routes>` component.  This placement is crucial for the catch-all functionality to work properly.  No other changes are typically needed. 

## Setup

1. Clone this repository.
2. Navigate to the project directory: `cd react-router-catch-all-issue`
3. Install dependencies: `npm install`
4. Run the application: `npm start`

Try navigating to non-existent routes to observe the issue and solution.
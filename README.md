# React Router Dom: Missing Catch-All Route

This repository demonstrates a common error in React Router v6 when using `Routes` and `Route` components:  forgetting to include a catch-all route (`/*`). Without it, unexpected routes or typos lead to a blank screen or unexpected behavior instead of a graceful 404.

## The Problem

The provided `App.js` showcases a simple React Router setup.  It includes routes for '/' (home) and '/about'.  However, if a user navigates to a non-existent route (e.g., '/invalid'), React Router doesn't display a default or 404 page.  This leads to a confusing user experience.

## The Solution

`AppSolution.js` demonstrates the solution. Adding a `Route` with `path="/*"`, handles all unmatched routes, enabling you to render a 404 page or a default component, avoiding unexpected blank screens or errors.
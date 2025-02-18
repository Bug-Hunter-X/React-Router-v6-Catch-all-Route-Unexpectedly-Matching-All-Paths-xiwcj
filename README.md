# React Router v6 Catch-all Route Issue

This repository demonstrates a problem with the catch-all route (`/*`) in React Router v6.  The catch-all route is unintentionally matching all paths, overriding other, more specific routes.  This prevents the application from navigating to any other route except the catch-all route. The solution demonstrates how to fix this, ensuring routes work as intended.

## Problem

The primary issue is in the order of routes. Because the `/*` route is placed after other routes, it intercepts all requests. To solve this, the catch-all route should always be placed last in the route definition.
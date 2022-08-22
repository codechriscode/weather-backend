# Weather Backend

This repo was created to be in the middle of my React front-end application Weather, a portfolio app, and a weather provider.

## Why

When a React application is built, it bundles all its code and sends it to the client. This could include secrets like API keys (which is the case).

## Solution

The only correct storage of secrets is in-server-memory, not in repositories or on the client side. So this little backend application written in Rails is running on a free environment with my API key securely stored.
The React app sends requests to it, and it authenticates and asks the weather provider about the current weather, and sends the answer back to React.

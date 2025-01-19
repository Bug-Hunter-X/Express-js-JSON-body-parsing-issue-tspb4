# Express.js JSON Body Parsing Issue

This repository demonstrates a common issue encountered when working with JSON request bodies in Express.js applications.

## Bug Description
The provided Express.js application attempts to parse the JSON request body using `express.json()`. However, despite the middleware being applied, the `req.body` remains empty when a POST request with a JSON payload is sent.

## Solution
The issue is solved by ensuring that the `express.json()` middleware is applied *before* the route handler that expects the JSON body.  The bug and solution files demonstrate the problem and correction.
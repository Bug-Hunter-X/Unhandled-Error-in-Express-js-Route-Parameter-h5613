# Unhandled Error in Express.js Route Parameter

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling for invalid or unexpected input parameters.  Specifically, this example shows a route that retrieves user data based on an ID.  If an invalid ID is provided, the application crashes without gracefully handling the error.

## Bug

The `bug.js` file contains the flawed code.  The route handler doesn't check if `req.params.id` is a valid user ID before attempting to use it.  This leads to potential errors if an invalid ID is passed, like trying to access a non-existent resource or a database record.
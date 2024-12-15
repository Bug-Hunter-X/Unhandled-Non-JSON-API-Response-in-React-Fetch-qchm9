# Unhandled Non-JSON API Response in React

This example demonstrates a common error in React applications: failing to properly handle non-JSON responses from an API.  The `fetch` call is made, but the `.then(response => response.json())`  will throw an error if the response is not valid JSON.  The error handling is inadequate leading to a silent failure with no clear indication to the user.

The solution provided addresses this by adding a check to the response status and type before parsing as JSON, providing more robust error handling.
# Unhandled FormatException in Dart JSON Decoding

This repository demonstrates a common error in Dart when parsing JSON responses from HTTP requests.  The `bug.dart` file contains code that doesn't properly handle potential `FormatException` exceptions that can occur if the server returns non-JSON data. The `bugSolution.dart` file provides a corrected version.

## Problem
The original code attempts to decode the response body using `jsonDecode` without error handling. If the server returns an unexpected response, this causes a runtime exception, crashing the app.

## Solution
The improved solution incorporates error handling to gracefully manage invalid JSON responses, providing a more robust application.
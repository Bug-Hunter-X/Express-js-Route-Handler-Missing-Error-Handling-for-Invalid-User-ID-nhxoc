# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers: the lack of proper error handling for invalid input.  Specifically, this example shows a route that retrieves a user by ID, but fails to handle cases where the ID is not a valid integer.

## Bug

The `bug.js` file contains the erroneous code.  The route handler attempts to parse the user ID as an integer, but doesn't handle potential errors (e.g., if the ID is not a number, or is not a valid user ID).  This can lead to unexpected behavior or crashes. 

## Solution

The `bugSolution.js` file provides a corrected version of the code. The solution includes comprehensive error handling to check for invalid user IDs and to provide appropriate responses.

## How to Run

1. Clone the repository: `git clone <repository_url>`
2. Navigate to the directory: `cd express-error-handling`
3. Install dependencies: `npm install`
4. Run the server: `node bug.js` (or `node bugSolution.js` for the fixed version)
5. Test with various user IDs, including invalid ones, to observe the difference.
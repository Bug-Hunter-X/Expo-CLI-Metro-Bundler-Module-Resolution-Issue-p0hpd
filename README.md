# Expo CLI Metro Bundler Module Resolution Issue

This repository demonstrates a bug encountered with the Expo CLI Metro bundler where modules from a correctly installed library fail to be resolved.  The error messages are unhelpful, making debugging difficult.  The solution provided addresses the issue by clearing the Metro cache and ensuring proper module paths.

## Steps to Reproduce

1. Clone this repository.
2. Install the dependencies using `npm install`.
3. Run the app using `expo start`.  You will likely encounter a module resolution error.
4. Apply the solution in `bugSolution.js` and re-run `expo start` to see the fixed version.

## Bug

The bug occurs intermittently, and may not always reproduce depending on your local environment.
The main issue is the inability of the Metro bundler to correctly resolve modules despite them being correctly installed. This results in vague error messages that don't point to the root cause.

## Solution

The solution involves clearing the Metro bundler cache and carefully verifying the module paths within the project.
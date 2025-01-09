# Missing Content-Type Header in Node.js HTTP Response

This repository demonstrates a common error in Node.js HTTP servers: omitting the `Content-Type` header in the response.  This can lead to unexpected behavior in the browser, including incorrect content rendering or errors.

## Bug

The `bug.js` file shows a simple HTTP server that sends a 'Hello World!' response without specifying the `Content-Type` header.  Browsers may struggle to interpret this response, potentially displaying it incorrectly.

## Solution

The `bugSolution.js` file corrects this by adding the `Content-Type` header to the response, specifically setting it to `text/plain`. This ensures the browser correctly identifies the content as plain text and renders it accordingly. 

This illustrates the importance of setting appropriate headers for a robust and predictable HTTP server in Node.js.
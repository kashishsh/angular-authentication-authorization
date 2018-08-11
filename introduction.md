- To implement authentication, on the client we should build a login page and on server build a api end point to validate the user.
- Call authentication api as user clicks on login button and server returns a JSON web token or JWT if login is valid.
- JWT is a JSON object that contains certain attributes about the logged in user(emailId, username etc)  and we use it to identify the user on the client and also on the server. We get this jwt on client and need to store it to some persistent place. If user closes the browser and opens the browser again , jwt should be there. Localstorage is used to save jwt.
- On the client we can use JWT for :
  - Display current username.
  - Show/hide parts of page.
  - prevent access to certain routes.

- If user want to access something from server which needs some authentication. Then the jwt token should be included with the request in request headers. server will extract that token and valide it.. if token is valid, server with return the required result, otherwise unauthorized response should return.

- JWT are an open industry standard method for representing claims securely between two parties.
- JWT token is not encrypted, it is just encoded with base64 encoding.






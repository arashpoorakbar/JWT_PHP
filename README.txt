This is a simple module with two functions to create and validate JSON Web Tokens using SHA256 signature.

Function generate_jwt() receives two arguments. First is the payload and the second is the secret key. It returns a string which is the token.

Function validate_jwt() receives two arguments. First is the token itself and the secret key. In case of damaged or corrupted tokens it will return error whic must be handled.
In case of uncorrputed tokens the function returns the decoded payload. If the token is expired the function will return false.
# HTTP Status Codes

This documentation provides a concise overview of the main HTTP status codes, explaining their meanings, typical usage scenarios, and practical examples. HTTP status codes are standardized codes returned by the server in response to a client request, giving information on whether the request was successful, redirected, encountered a client or server error, or any other special condition.

---

## 1. Informational Responses (100–199)
**These codes indicate that the request was received and understood, and the client can continue with the request.**

- **100 Continue**: Initial part of the request received; the client can continue with the request.
- **101 Switching Protocols**: The server is switching protocols as requested by the client.

---

## 2. Successful Responses (200–299)
**These codes indicate that the client's request was successfully received, understood, and accepted.**

### 200 OK
- **Meaning**: The request has succeeded.
- **Usage**: Returned for successful requests. In a GET request, it may contain the requested resource; in a POST, it could confirm resource creation.
- **Example**: A successful API call to retrieve user data.

### 201 Created
- **Meaning**: The request has been fulfilled, and a new resource was created.
- **Usage**: Used in response to a POST request for resource creation.
- **Example**: A new user registration.

### 204 No Content
- **Meaning**: The server processed the request but returns no content.
- **Usage**: Often used for DELETE requests or PUT updates.
- **Example**: After deleting a resource.

---

## 3. Redirection Messages (300–399)
**These codes indicate that the client must take additional action to complete the request.**

### 301 Moved Permanently
- **Meaning**: The resource has been permanently moved to a new URL.
- **Usage**: Clients should update their bookmarks or links.
- **Example**: A website changing its URL structure.

### 302 Found
- **Meaning**: The resource is temporarily at a different URL.
- **Usage**: Temporary redirect; the original URL should be used for future requests.
- **Example**: Redirecting users to a maintenance page.

---

## 4. Client Error Responses (400–499)
**These codes indicate that there was an error in the request that the client must correct.**

### 400 Bad Request
- **Meaning**: The request could not be processed due to a client error.
- **Usage**: When a request has invalid syntax or parameters.
- **Example**: Malformed JSON in a POST request.

### 401 Unauthorized
- **Meaning**: Authentication is required and has not been provided.
- **Usage**: Used when access requires authentication.
- **Example**: Accessing a protected resource without credentials.

### 403 Forbidden
- **Meaning**: The server understands the request but refuses to authorize it.
- **Usage**: Indicates lack of permission regardless of authentication.
- **Example**: A user trying to access an admin-only section.

### 404 Not Found
- **Meaning**: The server cannot find the requested resource.
- **Usage**: Indicates the resource is missing or the URL is incorrect.
- **Example**: Accessing a non-existent webpage.

---

## 5. Server Error Responses (500–599)
**These codes indicate that the server failed to fulfill a valid request due to an error.**

### 500 Internal Server Error
- **Meaning**: The server encountered an unexpected condition.
- **Usage**: A generic error when the server cannot process the request.
- **Example**: An unhandled exception in server code.

### 502 Bad Gateway
- **Meaning**: The server, acting as a gateway, received an invalid response.
- **Usage**: When an upstream server returns an error to a proxy server.
- **Example**: An upstream server is down or misconfigured.

---

### Additional Status Codes

- **418 I'm a Teapot**: An April Fools' joke (RFC 2324); indicates the server is a teapot and cannot brew coffee.
- **429 Too Many Requests**: The client has made too many requests in a given time frame, often used to prevent abuse.

For a full list of HTTP status codes, please refer to the official [HTTP Status Code Definitions](https://developer.mozilla.org/en-US/docs/Web/HTTP/Status).

---

This overview is a reference to understand the purposes and behaviors of standard HTTP status codes in web and API development.

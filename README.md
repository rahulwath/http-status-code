# HTTP Status Codes

This document provides a comprehensive overview of HTTP status codes, categorized into five classes based on their response types. Each status code is followed by a brief description to aid in understanding its purpose.

## 1. Informational Responses (100–199)

- **100 Continue**: The initial part of a request has been received, and the client may continue with the request.
- **101 Switching Protocols**: The server is switching protocols as requested by the client.
- **102 Processing**: The server has received and is processing the request but has no response available yet (WebDAV).

## 2. Successful Responses (200–299)

- **200 OK**: The request has succeeded. The meaning of the success depends on the HTTP method used.
- **201 Created**: The request has succeeded, resulting in the creation of a new resource.
- **202 Accepted**: The request has been accepted for processing, though processing is incomplete.
- **203 Non-Authoritative Information**: The request was successful, but the response may be from another source.
- **204 No Content**: The server processed the request but returns no content.
- **205 Reset Content**: The server processed the request and asks the client to reset the document view.
- **206 Partial Content**: The server is delivering only part of the resource due to a range request.

## 3. Redirection Messages (300–399)

- **300 Multiple Choices**: The request has multiple possible responses; the client or user should choose one.
- **301 Moved Permanently**: The resource has been permanently moved to a new URL.
- **302 Found**: The resource is temporarily located at a different URL.
- **303 See Other**: The response is at another URI, accessible with a GET request.
- **304 Not Modified**: The resource has not changed since the last request; the client may use the cached version.
- **305 Use Proxy**: The resource must be accessed through the specified proxy.
- **307 Temporary Redirect**: The resource is temporarily moved, but the original method should be used for subsequent requests.
- **308 Permanent Redirect**: The resource has been permanently moved; future requests should use the new URL.

## 4. Client Error Responses (400–499)

- **400 Bad Request**: The server cannot process the request due to client error (e.g., malformed syntax).
- **401 Unauthorized**: Authentication is required and has either failed or not been provided.
- **402 Payment Required**: Reserved for future use.
- **403 Forbidden**: The server understands the request but refuses authorization.
- **404 Not Found**: The requested resource is not found on the server.
- **405 Method Not Allowed**: The method is not supported for the specified resource.
- **406 Not Acceptable**: The server cannot produce a response matching the acceptable values in the request headers.
- **407 Proxy Authentication Required**: The client must authenticate with the proxy.
- **408 Request Timeout**: The server timed out waiting for the request.
- **409 Conflict**: The request cannot be completed due to a conflict with the resource’s current state.
- **410 Gone**: The requested resource is no longer available.
- **411 Length Required**: The request lacks a defined Content-Length.
- **412 Precondition Failed**: One or more conditions specified in the request headers are not met.
- **413 Payload Too Large**: The request entity exceeds the server's size limits.
- **414 URI Too Long**: The URI is too long for the server to process.
- **415 Unsupported Media Type**: The request’s media type is not supported.
- **416 Range Not Satisfiable**: The server cannot satisfy the Range header in the request.
- **417 Expectation Failed**: The server cannot meet the requirements of the Expect header.
- **418 I'm a teapot**: A playful response indicating refusal to brew coffee (RFC 2324).
- **421 Misdirected Request**: The request was directed at a server that cannot produce a response.
- **422 Unprocessable Entity**: The request is well-formed but contains semantic errors (WebDAV).
- **423 Locked**: The resource is locked (WebDAV).
- **424 Failed Dependency**: A previous request dependency failed (WebDAV).
- **425 Too Early**: The server is unwilling to process the request due to potential replay risks.
- **426 Upgrade Required**: The client should switch protocols.
- **428 Precondition Required**: The origin server requires the request to be conditional.
- **429 Too Many Requests**: The client has sent too many requests in a short period.
- **431 Request Header Fields Too Large**: The request headers are too large.

## 5. Server Error Responses (500–599)

- **500 Internal Server Error**: A generic error indicating an unexpected condition.
- **501 Not Implemented**: The server does not support the functionality required to fulfill the request.
- **502 Bad Gateway**: The server received an invalid response from an upstream server.
- **503 Service Unavailable**: The server is temporarily unable to handle the request.
- **504 Gateway Timeout**: The server did not receive a timely response from an upstream server.
- **505 HTTP Version Not Supported**: The HTTP version used in the request is not supported.
- **511 Network Authentication Required**: The client must authenticate to gain network access.

---

This README serves as a quick reference to understand each HTTP status code and its significance.

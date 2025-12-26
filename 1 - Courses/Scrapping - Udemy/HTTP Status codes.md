
HTTP status codes are standardized responses from a server to a client’s request when[[HTTP Protocol]] are used. They indicate whether the request was successful, encountered an error, or requires further action. These codes are grouped into five classes based on their purpose.

The notation to uderstand the status codes are the following:

![[Pasted image 20241229195139.png]]
### Status Code Classes

#### 1xx: Informational

- **Description**: The request was received and is being processed.
    
- **Common Codes**:
    
    - **100 Continue**: The server has received the request headers and the client should proceed to send the request body.
        
    - **101 Switching Protocols**: The server agrees to switch protocols as requested by the client.
        
#### 2xx: Success

- **Description**: The request was successfully received, understood, and processed.
    
- **Common Codes**:
    
    - **200 OK**: The request succeeded, and the response contains the requested data.
        
    - **201 Created**: The request succeeded, and a new resource was created.
        
    - **204 No Content**: The request succeeded, but there is no content to return.
        
#### 3xx: Redirection

- **Description**: Further action is required to complete the request.
    
- **Common Codes**:
    
    - **301 Moved Permanently**: The requested resource has been permanently moved to a new URL.
        
    - **302 Found**: The requested resource resides temporarily under a different URL.
        
    - **304 Not Modified**: The cached version of the resource is still valid; no new data is sent.
        
#### 4xx: Client Error

- **Description**: The request contains bad syntax or cannot be fulfilled.
    
- **Common Codes**:
    
    - **400 Bad Request**: The server cannot process the request due to client error.
        
    - **401 Unauthorized**: Authentication is required to access the resource.
        
    - **403 Forbidden**: The server understands the request but refuses to authorize it.
        
    - **404 Not Found**: The requested resource could not be found on the server.
        
#### 5xx: Server Error

- **Description**: The server failed to fulfill a valid request.
    
- **Common Codes**:
    
    - **500 Internal Server Error**: The server encountered an unexpected condition.
        
    - **502 Bad Gateway**: The server received an invalid response from an upstream server.
        
    - **503 Service Unavailable**: The server is temporarily unable to handle the request.
        
    - **504 Gateway Timeout**: The server did not receive a timely response from an upstream server.
        
### Common Usage Examples

#### Handling Success (2xx):

```
GET /users/123 HTTP/1.1
Host: api.example.com

Response:
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": 123,
  "name": "John Doe"
}
```

#### Handling Redirection (3xx):

```
GET /old-path HTTP/1.1
Host: api.example.com

Response:
HTTP/1.1 301 Moved Permanently
Location: https://api.example.com/new-path
```

#### Handling Client Errors (4xx):

```
GET /non-existent HTTP/1.1
Host: api.example.com

Response:
HTTP/1.1 404 Not Found
Content-Type: text/plain

The requested resource was not found.
```

#### Handling Server Errors (5xx):

```
GET /users HTTP/1.1
Host: api.example.com

Response:
HTTP/1.1 500 Internal Server Error
Content-Type: text/plain

An unexpected error occurred on the server.
```

### Conclusion

Understanding HTTP status codes is critical for diagnosing and handling server responses. Proper use of status codes ensures clear communication between clients and servers, improving the reliability and usability of web applications.
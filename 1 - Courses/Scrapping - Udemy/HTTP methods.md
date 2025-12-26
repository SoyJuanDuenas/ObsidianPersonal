
HTTP verbs (also known as HTTP methods) define the actions that can be performed on resources in a web application. They are essential for [[RESTful APIs]] and web development, enabling communication between clients and servers.

### Common HTTP Verbs

#### GET

- **Purpose**: Retrieve data from the server.
    
- **Characteristics**:
    
    - Should not have any side effects.        
    - Can be cached.
    - Can include query parameters to filter or modify the request.
        
- **Example**:
    
    ```
    GET /users/123 HTTP/1.1
    Host: api.example.com
    ```
    

#### POST

- **Purpose**: Submit data to be processed by the server.
    
- **Characteristics**:
    
    - Often used to create new resources.
    - Includes a request body containing the data.
    - Not idempotent (repeating the request may create duplicate resources).
        
- **Example**:
    
    ```
    POST /users HTTP/1.1
    Host: api.example.com
    Content-Type: application/json
    
    {
      "name": "John Doe",
      "email": "john.doe@example.com"
    }
    ```
#### PUT

- **Purpose**: Update or create a resource.
    
- **Characteristics**:
    
    - Idempotent (repeating the request produces the same result).
    - Typically requires the full representation of the resource.
        
- **Example**:
    
    ```
    PUT /users/123 HTTP/1.1
    Host: api.example.com
    Content-Type: application/json
    
    {
      "name": "Jane Doe",
      "email": "jane.doe@example.com"
    }
    ```
    

#### DELETE

- **Purpose**: Remove a resource from the server.
    
- **Characteristics**:
    
    - Idempotent (repeating the request has no additional effect).
    - Usually does not include a request body.
        
- **Example**:
    
    ```
    DELETE /users/123 HTTP/1.1
    Host: api.example.com
    ```
    
#### PATCH

- **Purpose**: Partially update a resource.
    
- **Characteristics**:
    
    - Requires only the fields to be updated in the request body.
    - Not necessarily idempotent.
        
- **Example**:
    
    ```
    PATCH /users/123 HTTP/1.1
    Host: api.example.com
    Content-Type: application/json
    
    {
      "email": "new.email@example.com"
    }
    ```
    
#### HEAD

- **Purpose**: Retrieve metadata about a resource.
    
- **Characteristics**:
    
    - Similar to GET but without the response body.
    - Often used for checking resource availability or caching information.
        
- **Example**:
    
    ```
    HEAD /users/123 HTTP/1.1
    Host: api.example.com
    ```
    

#### OPTIONS

- **Purpose**: Determine the HTTP methods and features supported by a resource.
    
- **Characteristics**:
    
    - Provides information about communication options.
    - Often used in preflight requests for CORS.
        
- **Example**:
    
    ```
    OPTIONS /users HTTP/1.1
    Host: api.example.com
    ```
    

#### TRACE

- **Purpose**: Echo the request to see what changes or modifications have been made by intermediaries.
    
- **Characteristics**:
    
    - Primarily used for debugging.
    - Not commonly used in production.
        
- **Example**:
    
    ```
    TRACE /users/123 HTTP/1.1
    Host: api.example.com
    ```
    

### Idempotence and Safety

1. **Idempotent Methods**: GET, PUT, DELETE, and HEAD are idempotent, meaning repeated identical requests produce the same result.
    
2. **Safe Methods**: GET and HEAD are considered safe as they do not modify resources.
    
### Conclusion

Understanding HTTP verbs is fundamental to building and consuming web APIs effectively. By adhering to their intended use, developers can create predictable, maintainable, and scalable web services.
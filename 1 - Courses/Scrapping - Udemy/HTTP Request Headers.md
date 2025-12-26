
HTTP request headers are key-value pairs sent from the client to the server. They provide additional context or instructions about the request, such as metadata, authentication details, or content specifications. Headers are an essential part of HTTP communication in [[HTTP Protocol]], enabling functionality like content negotiation, caching, and security.

In Web Scrapping, headers are important because can be used to send aditional information that the server use to identify the client, often times servers are configurated in a way that discriminate some clients (like WebScrapers)

For example we can pretend be Google bots (with headers) to go througt PayWalls

### Common Request Headers

#### 1. **Host**

- **Description**: Specifies the domain name and port of the server being requested.
    
- **Example**:
    
    ```
    Host: api.example.com
    ```
    
#### 2. **User-Agent**

- **Description**: Identifies the client software making the request, such as a browser or API client.
    
- **Example**:
    
    ```
    User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/96.0.4664.110 Safari/537.36
    ```
    
#### 3. **Authorization**

- **Description**: Contains credentials for authenticating the client with the server.
    
- **Example**:
    
    ```
    Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...
    ```
    

#### 4. **Accept**

- **Description**: Indicates the media types the client can process.
    
- **Example**:
    
    ```
    Accept: application/json, text/html
    ```
    

#### 5. **Content-Type**

- **Description**: Specifies the media type of the request body (used in POST and PUT requests).
    
- **Example**:
    
    ```
    Content-Type: application/json
    ```
    

#### 6. **Accept-Language**

- **Description**: Specifies the preferred language(s) for the response.
    
- **Example**:
    
    ```
    Accept-Language: en-US, en;q=0.9
    ```


#### 7. **Cookie**

- **Description**: Contains [[browser cookies]] previously sent by the server to maintain [[state]].
    
- **Example**:
    
    ```
    Cookie: sessionId=abc123; theme=dark
    ```
    
#### 8. **Referer**

- **Description**: Indicates the URL of the resource from which the request was initiated.
    
- **Example**:
    
    ```
    Referer: https://www.example.com
    ```
    
#### 9. **Cache-Control**

- **Description**: Directs caching behavior for the request.
    
- **Example**:
    
    ```
    Cache-Control: no-cache
    ```
    

#### 10. **Connection**

- **Description**: Controls whether the network connection remains open after the request.
    
- **Example**:
    
    ```
    Connection: keep-alive
    ```
    

### Example Request with Headers

```
GET /users/123 HTTP/1.1
Host: api.example.com
User-Agent: Mozilla/5.0 (Windows NT 10.0; Win64; x64)
Authorization: Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9...
Accept: application/json
Content-Type: application/json
Accept-Language: en-US
```

### Custom Headers

- **Purpose**: Applications can define custom headers to convey application-specific information.
    
- **Example**:
    
    ```
    X-Custom-Header: my-custom-value
    ```
    

### Conclusion

Request headers are a powerful mechanism for enhancing HTTP communication. Understanding and using them effectively allows for more secure, efficient, and feature-rich client-server interactions.
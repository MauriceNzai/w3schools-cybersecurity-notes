## Cybersecurity: Web Applications

### Overview
Web applications are essential for modern internet usage, enabling users to access services and interact with systems remotely. Understanding how they work is key to securing them.

---

### HTTP Protocol
- HTTP is the core protocol used to transfer data (HTML, CSS, images, etc.) between clients (browsers) and servers.
- It defines how requests and responses are structured.

---

### URLs, Parameters & Schemes
- A URL (Uniform Resource Locator) identifies a web resource.
- Components include:
  - **Domain** (e.g., google.com)
  - **Path** (e.g., /search)
  - **Query parameters** (`?key=value&key2=value2`)
- **Scheme** defines the protocol used (HTTP, HTTPS, FTP, etc.).

---

### HTTP Headers
- Provide additional information in requests and responses.
- Examples:
  - `Host`: target server
  - `User-Agent`: client details
  - `Cookie`: session data
  - `Content-Type`: type of returned data
- Headers control behavior like compression, authentication, and tracking.

---

### HTTP Verbs (Methods)
- Define actions performed on resources:
  - `GET` – retrieve data
  - `POST` – send/create data
  - `PUT` – update/replace data
  - `DELETE` – remove data
  - `PATCH` – partially update data
- Widely used in RESTful APIs.

---

### HTTP Response Codes
- Indicate server response status:
  - `200` – success
  - `301/302` – redirects
  - `400` – bad request
  - `403` – forbidden
  - `404` – not found
  - `500` – server error

---

### REST (Representational State Transfer)
- Uses URLs and HTTP methods to perform actions.
- Often used in APIs.
- Example: `/users/search/john` → search for user "john".

---

### Sessions & State
- HTTP is stateless; sessions track users across requests.
- Typically managed using **cookies** (e.g., session IDs).
- Secure session handling is critical to prevent hijacking.
- Alternatives include:
  - JWT (JSON Web Tokens)
  - ViewState

---

### Virtual Hosts
- A single server can host multiple applications.
- The `Host` header determines which application handles the request.

---

### URL Encoding
- Converts unsafe characters into a safe format using `%` and hex values.
  - Space → `%20`
  - `%` → `%25`
- Ensures safe data transmission.

---

### JavaScript
- Enables dynamic and interactive web content.
- Runs on the client side.
- Commonly involved in web-based attacks.

---

### Encryption (HTTPS & TLS)
- HTTP does not encrypt data.
- HTTPS uses **TLS (Transport Layer Security)** to secure communication.
- Protects data in transit from interception.

```mermaid
sequenceDiagram
    participant User
    participant Browser
    participant Server
    User->>Browser: Submit input;
    Browser->>Server: Send user input to server;
    Server->>Browser: Server asks browser to reload the notes page;
    Browser->>Server: Asks to fetch stylesheet, JS code and data;
    Server->>Browser: Sends data;
    Browser->>User: Loads new page;
        
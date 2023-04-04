```mermaid
sequenceDiagram
    participant User
    participant Browser
    participant Server
    User->>Browser: Sends input;
    Browser->>Server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa;
    Server-->>Browser: Status code 201, created;
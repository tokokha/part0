```mermaid
sequenceDiagram
    participant User
    participant Browser
    participant Server
    User->>Browser: Submit input;
    Browser->>Server: POST studies.cs.helsinki.fi/exampleapp/new_note;
    Server->>Browser: URL redirect to /notes;
    Browser->>Server: GET https://studies.cs.helsinki.fi/exampleapp/main.css;
    Server-->>Browser: Sends CSS file;
    Browser->>Server: GET https://studies.cs.helsinki.fi/exampleapp/main.js;
    Server-->>Browser: Sends JS file;
    Browser->>Server: GET https://studies.cs.helsinki.fi/exampleapp/data.json;
    Server-->>Browser: Sends data file;
    Browser->>User: Loads new page;
        
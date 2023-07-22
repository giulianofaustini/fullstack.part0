sequenceDiagram
    participant browser
    participant server

    browser->>server: https://studies.cs.helsinki.fi/exampleapp/spa
    activate server
    server-->>browser: HTML document (including main.css, spa.js, data.json)
    deactivate server
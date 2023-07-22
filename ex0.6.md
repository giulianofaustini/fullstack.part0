sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: 201 Created contains JSON data {content: "one two three four", date: "2023-07-22T13:57:29.728Z"}
    deactivate server
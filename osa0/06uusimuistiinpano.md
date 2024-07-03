```mermaid
sequenceDiagram

        participant browser
        participant server

        browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
        activate server

Note right of browser: The server gets the new note in a JSON format

        server->>browser: new note created (201)
        deactivate server

Note right of browser: The new note updates to the page without reloading it
```

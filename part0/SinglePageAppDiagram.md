```mermaid
sequenceDiagram

Note left of browser: Javascript prevents default browser behavior.
Note left of browser: new note is pushed to notes array, redrawNotes() is called.

Note right of browser: Request Content type is application/json
browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa 
activate server
server-->>browser: Status 201(new resource created)
deactivate server

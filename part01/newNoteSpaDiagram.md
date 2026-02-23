
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: JSON Response({message: "note created"})
    deactivate server
    
    Note right of browser: The Browser Uses javaScript to render the data on the application without redirecting.
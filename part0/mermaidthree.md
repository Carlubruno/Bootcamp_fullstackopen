```mermaid


sequenceDiagram
    participant USER
    participant BROWSER
    participant SERVER

    USER->>BROWSER: user write the note input and save
    
    
    BROWSER->>SERVER: send the note data get https://studies.cs.helsinki.fi/exampleapp/new_note_spa 
    
    
    note right of SERVER: The server receives the new data and save it
    SERVER->>BROWSER: Send content and date[{}]
    note left of SERVER: updates the note dynamically and dont refresh the page

    note left of BROWSER: render new note
    

    

    
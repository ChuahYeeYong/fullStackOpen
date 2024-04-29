sequenceDiagram
    participant browser
    participant server

    browser->>browser: Save new input push input to Notes array and redrawNotes() to re-render notes with new input
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    Note right of browser: Current SPA JavaScript does not send any new HTML requests
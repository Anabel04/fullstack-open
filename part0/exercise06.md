## Exercise 0.6

### Diagram:
```mermaid
sequenceDiagram
    participant browser
    participant server
    browser->>server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    Note right of browser: The user type in the text field and click on the Save button.
    server-->>browser: HTTP 302 Created
    deactivate server
    Note right of browser: The browser updates the page dynamically using JavaScript (DOM manipulation).

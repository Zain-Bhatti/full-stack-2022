```mermaid
sequenceDiagram
  participant user
  participant browser
  participant server

  user ->> browser: Writes a note (Testing...) and clicks Save
  browser ->> server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
  activate server
  server ->> server: Processing request
  server ->> browser: Responds with success
  deactivate server
```

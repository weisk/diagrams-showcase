# VANTIV UI FLOW

```mermaid
sequenceDiagram
  participant cli as Browser
  participant srv as Server
  participant data as Simfel

  Note over cli,srv: server renders reactapp

  cli ->> srv: get myapp.com/democicero
  srv ->> data: get retrieveSiteletteByURLkeyAndTemplate
  data ->> srv: saslData
  srv ->> cli: react app + saslData
  
  activate cli
  Note over cli: Browse
  Note over cli: checkout
  cli ->> srv: Place order
  deactivate cli

  
```

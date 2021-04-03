# VANTIV_ECOMMERCE

```mermaid
sequenceDiagram
  participant cli as Browser
  participant srv as Server
  participant data as Data
  participant 3rd as 3rdPartyProcessor

  Note over cli,srv: server renders reactapp
  Note left of data: Simfel
  Note right of 3rd: Vantiv

  cli ->> srv: get myapp.com/democicero
  srv ->> data: get retrieveSiteletteByURLkeyAndTemplate
  data ->> srv: saslData
  srv ->> cli: react app + saslData
  
  activate cli
  Note over cli: Populate page, fill cart
  Note over cli: checkout
  cli ->> srv: buy
  deactivate cli

  
```

# TSYS_ECOMMERCE

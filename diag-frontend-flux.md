# well

```bash
graph TD
  A[ Anyone ] -->|Can help | B( Go to github.com/yuzutech/kroki )
  B --> C{ How to contribute? }
  C --> D[ Reporting bugs ]
  C --> E[ Sharing ideas ]
  C --> F[ Advocating ]
```

```mermaid
graph LR
  c1[App]
  c2[Router Switch]
  c3[ProtectedRoutes..]
  c4[PublicRoutes..]
  c5[Layout]
  c6[page]

  c15[Layout]
  h1[BusinessData]
  h2{ window.__SASL_DATA__ ? }
  c16[HydrateReactApp]
  c17[AjaxReactApp]
  

  c1 --> c2
  c2 --> c3
  c2 --> c4
  c3 --> c5
  c4 --> c5
  c5 --> c6


  c15 --> |asks for| h1
  h1 --> h2
  h2 --> |yes| c16
  h2 --> |no| c17

  
```

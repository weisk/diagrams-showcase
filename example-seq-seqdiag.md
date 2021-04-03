# example seqdiag

```seqdiag
seqdiag {
  browser  -> phpserver [label = "GET /"];
  browser <-- webserver;
  browser  -> webserver [label = "POST /blog/comment"];
  webserver  -> database [label = "INSERT comment"];
  webserver <-- database;
  browser <-- webserver;
}
```

Arkly is developing using [Domain-Driven Design](https://en.wikipedia.org/wiki/Domain-driven_design) (DDD) principles. That includes establising a clear domain model in which the software system operates.


# Arkly domain diagram

```mermaid
flowchart TD;
      A[Agent] -->|performs| B(Event);
      A[Agent] -->|is responsible for| C(Function);
      C -->|consists of| B;
      B -->|creates| D(Archival material);
```

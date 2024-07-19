Arkly is developing using [Domain-Driven Design](https://en.wikipedia.org/wiki/Domain-driven_design) (DDD) principles. That includes establising a clear domain model in which the software system operates.


# Arkly domain diagram

## Version 1

```mermaid
flowchart TD;
      A[Agent] -->|performs| B(Event);
      A -->|is responsible for| C(Function);
      C -->|consists of| B;
      B -->|creates| D[Archival material];
```

## Version 2

```mermaid
flowchart TD;
      A[Agent] -->|performs| B(Event);
      A -->|is responsible for| C(Function);
      C -->|consists of| B;
      B -->|creates| D[Archival material];
      F[Creator] -->|is a type of| A;
      E[Researcher] -->|is a type of| A;
      E -->|requests| D;
```

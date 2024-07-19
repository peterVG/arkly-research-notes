Arkly is developing using [Domain-Driven Design](https://en.wikipedia.org/wiki/Domain-driven_design) (DDD) principles. That includes establising a clear domain model in which the software system operates.


# Arkly domain diagram

## Version 6

```mermaid
flowchart LR;
      A[Agent] -->|performs| B(Event);
      A -->|is responsible for| C(Function);
      C -->|consists of| B;
      B -->|creates| D[Archival material];
      F[Creator] -->|is a type of| A;
      E[Researcher] -->|is a type of| A;
      E -->|requests| D;
      G[Archival repository] -->|provides access to| D;
      G -->|is a type of| A;
      H[Archivist] -->|performs functions for| G;
      H -->|is a type of| A;
      H -->|describes| D;
      I[Donor] -->|donates| J(Accession);
      I -->|is a type of| A;
      J -->|is a type of| B;
      F -->|creates| D;
      H -->|appraises| J;
      J -->|adds archival materials to| G;
      K[Rightsholder] -->|claims| L[Rights];
      K -->|is a type of| A;
      L -->|restrics use of| D;
```



## Version 5

```mermaid
flowchart TD;
      A[Agent] -->|performs| B(Event);
      A -->|is responsible for| C(Function);
      C -->|consists of| B;
      B -->|creates| D[Archival material];
      F[Creator] -->|is a type of| A;
      E[Researcher] -->|is a type of| A;
      E -->|requests| D;
      G[Archival repository] -->|provides access to| D;
      G -->|is a type of| A;
      H[Archivist] -->|performs functions for| G;
      H -->|is a type of| A;
      H -->|describes| D;
      I[Donor] -->|donates| J(Accession);
      I -->|is a type of| A;
      J -->|is a type of| B;
      F -->|creates| D;
      H -->|appraises| J;
      J -->|adds archival materials to| G;
      K[Rightsholder] -->|claims| L[Rights];
      K -->|is a type of| A;
      L -->|restrics use of| D;
```

## Version 4

```mermaid
flowchart TD;
      A[Agent] -->|performs| B(Event);
      A -->|is responsible for| C(Function);
      C -->|consists of| B;
      B -->|creates| D[Archival material];
      F[Creator] -->|is a type of| A;
      E[Researcher] -->|is a type of| A;
      E -->|requests| D;
      G[Archival repository] -->|provides access to| D;
      G -->|is a type of| A;
      H[Archivist] -->|performs functions for| G;
      H -->|is a type of| A;
      H -->|describes| D;
      I[Donor] -->|donates| J(Accession);
      I -->|is a type of| A;
      J -->|is a type of| B;
      F -->|creates| D;
      H -->|appraises| J;
      J -->|adds archival materials to| G;
```


## Version 3

```mermaid
flowchart TD;
      A[Agent] -->|performs| B(Event);
      A -->|is responsible for| C(Function);
      C -->|consists of| B;
      B -->|creates| D[Archival material];
      F[Creator] -->|is a type of| A;
      E[Researcher] -->|is a type of| A;
      E -->|requests| D;
      G[Archival repository] -->|provides access to| D;
      G -->|is a type of| A;
      H[Archivist] -->|performs functions for| G;
      H -->|is a type of| A;
      H -->|describes| D;
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

## Version 1

```mermaid
flowchart TD;
      A[Agent] -->|performs| B(Event);
      A -->|is responsible for| C(Function);
      C -->|consists of| B;
      B -->|creates| D[Archival material];
```

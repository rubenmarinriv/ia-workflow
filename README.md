## Functional Layer

```mermaid
flowchart LR

A[Business] --> B(Create Ticket) --> C[Product Owner]
C --> D{Ready for Dev?}
D -->|No| E[Spike<br/>Product Owner + Business] --> C
D -->|Yes| F[Development]
```

```mermaid
sequenceDiagram
   # participant External Database
   # participant VR 

    participant LEA
    participant Recapp
    participant Taskbase
    participant LA Reporting
    participant Datawarehouse
    participant Moodle
    participant EdX-MOOCs
    participant CAS
    Moodle->>LEA: URL
    Moodle->>Recapp: iFrame
    Moodle->>Taskbase: LTI
    LA Reporting->>Datawarehouse: Raw Data
    Datawarehouse->>Moodle: Feedback/Interventions
    CAS->>Datawarehouse: Raw Data
    Moodle->>Datawarehouse: Raw Data
    Moodle->>EdX-MOOCs: LTI
  
```

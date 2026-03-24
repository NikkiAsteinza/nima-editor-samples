# Sequence Diagram Samples

## Notes, Activation And Control Blocks

```mermaid
sequenceDiagram
    autonumber
    actor User
    participant Web as Web App
    participant API as API Layer
    participant Worker as Async Worker
    participant DB as Database

    User->>Web: Open workspace
    Web->>API: GET /workspace
    activate API
    API->>DB: Load metadata
    activate DB
    DB-->>API: Metadata
    deactivate DB
    API-->>Web: Workspace payload
    deactivate API
    Web-->>User: Render editor

    Note over Web,API: Interactive editing begins

    User->>Web: Save document
    Web->>API: POST /documents
    API->>Worker: Queue snapshot

    alt Validation passed
        Worker->>DB: Persist version
        Worker-->>API: ok
        API-->>Web: Saved
    else Validation failed
        Worker-->>API: error list
        API-->>Web: Show errors
    end

    par Analytics
        Web->>API: Track usage
    and Notifications
        API-->>User: Send confirmation
    end

    opt Auto archive
        API->>DB: Mark previous revision as archived
    end
```

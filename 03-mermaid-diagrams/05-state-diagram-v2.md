# State Diagram v2 Samples

## Composite State And Choice

```mermaid
stateDiagram-v2
    state Result <<choice>>
    [*] --> Idle
    Idle --> Editing: open file
    Editing --> Saving: save
    Saving --> Result
    [*] --> Typing
    Typing --> Reviewing: inspect diff
    Reviewing --> Typing: continue editing
    Result --> Synced: ok
    Result --> Error: failed
    Error --> Editing: retry
    Synced --> [*]
```
# State Diagram v2 Samples

## Composite State And Choice

```mermaid
stateDiagram-v2
    [*] --> Idle
    Idle --> Editing : open file
    Editing --> Saving : save
    Saving --> Result

    state Editing {
        [*] --> Typing
        Typing --> Reviewing : inspect diff
        Reviewing --> Typing : continue editing
    }

    state Result <<choice>>
    Result --> Synced : ok
    Result --> Error : failed
    Error --> Editing : retry
    Synced --> [*]
```

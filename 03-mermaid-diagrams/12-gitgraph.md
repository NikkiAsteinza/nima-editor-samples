# GitGraph Samples

## Branches, Merge And Hotfix

```mermaid
gitGraph
    commit id: "A" tag: "v1.0.0"
    branch platform
    checkout platform
    commit id: "B"
    branch diagram_panels
    checkout diagram_panels
    commit id: "C"
    checkout platform
    commit id: "D"
    merge diagram_panels tag: "panels"
    checkout main
    merge platform tag: "v1.1.0"
    branch hotfix
    checkout hotfix
    commit id: "E"
    checkout main
    merge hotfix tag: "v1.1.1"
```

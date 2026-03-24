# Gantt Samples

## Sections, Milestones And Dependencies

```mermaid
gantt
    title Editor delivery roadmap
    dateFormat  YYYY-MM-DD
    axisFormat  %d %b

    section Discovery
    UX audit           :done,    d1, 2026-03-01, 3d
    Interaction model  :done,    d2, after d1, 4d

    section Build
    Shared panel shell :active,  b1, 2026-03-08, 4d
    Flowchart tabs     :active,  b2, after b1, 5d
    Object tree panel  :         b3, after b2, 4d

    section Validation
    Internal review    :         v1, after b3, 2d
    Release candidate  :milestone, rc1, after v1, 0d
```

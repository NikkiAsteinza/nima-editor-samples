# Wardley Map Sample

```mermaid
wardley
    title Diagram editing evolution
    anchor User [0.95, 0.70]
    anchor Markdown [0.82, 0.62]
    component Rich editor [0.72, 0.55]
    component Mermaid renderer [0.61, 0.48]
    component Visual panels [0.44, 0.42]
    component Export snapshots [0.36, 0.34]
    component AI assistance [0.22, 0.25]
    User->Markdown
    Markdown->Rich editor
    Rich editor->Mermaid renderer
    Mermaid renderer->Visual panels
    Visual panels->Export snapshots
    AI assistance->Visual panels
    evolution Genesis, Custom, Product, Commodity
```


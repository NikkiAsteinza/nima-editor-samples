# Packet Diagram Sample

Packet diagrams describe bit-level structures. This sample models the metadata envelope that could be attached to a saved editor operation.

```mermaid
packet
    0-3: "Version"
    4-7: "Operation"
    8-15: "Flags"
    16-31: "Workspace id"
    32-63: "Document revision"
    64-95: "Block id"
    96-127: "Checksum"
```

The ranges are bit positions. Larger fields make wide blocks, which is useful for testing zoom and horizontal scroll.


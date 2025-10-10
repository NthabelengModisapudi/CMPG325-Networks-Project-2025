#Bus Topology Schematic
# Network Topology

## Schematic Diagram

```mermaid
flowchart TD
    subgraph Core Layer
        Core_Switch["Core Switch"]
    end

    subgraph Access Layer 1
        Switch_1["Switch 1"]
    end

    subgraph Access Layer 2
        Switch_2["Switch 2"]
    end

    subgraph Server/Resource Pool
        R1["R1"]
        R2["R2"]
        R3["R3"]
        R_rest["... (R4-R741)"]
    end

    subgraph User Devices
        Laptop1["Laptop"]
        Laptop2["Laptop"]
        PC1["PC"]
        PC2["PC"]
    end

    Core_Switch <--> Switch_1
    Core_Switch <--> Switch_2
    Switch_1 <--> R1
    Switch_1 <--> R2
    Switch_1 <--> R3
    Switch_1 <--> R_rest
    Switch_2 <--> Laptop1
    Switch_2 <--> Laptop2
    Switch_2 <--> PC1
    Switch_2 <--> PC2
```

## Physical Layout
- **Coordinates**: x: 3590, y: 780
- **Total Resources**: 741 nodes (R1-R741)
- **Network Type**: Logical topology with physical positioning data

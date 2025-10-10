#Bus Topology Schematic
# Network Topology
```mermaid
flowchart TD
    subgraph A1 [Logical]
        subgraph B1 [Physical | x: 3590 y: 780]
            subgraph C1 [Data Tracking]
                R1["R1"]
                R2["R2"] 
                R3["R3"]
                R4["R4"]
                R5["R5"]
                R6["R6"]
                R_rest["... (R7-R741)"]
            end
        end
    end
    
    subgraph A2 [User Devices]
        Laptop1["💻 Laptop"]
        Laptop2["💻 Laptop"]
        PC1["🖥️ PC"]
        PC2["🖥️ PC"]
    end
    
    %% Direct connections as shown in original
    R1 --> Laptop1
    R2 --> Laptop2
    R3 --> PC1
    R4 --> PC2
```

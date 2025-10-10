#Bus Topology Schematic
graph TD
    subgraph "Management & Analysis Plane"
        UI[User Interface<br/>Screening Log]
        Log[Successful Connection Log<br/>PC5 -> PC23<br/>PC22 -> PC24<br/>PC25 -> PC4]
    end

    subgraph "Logical Network"
        PC1[PC5]
        PC2[PC23]
        PC3[PC22]
        PC4[PC24]
        PC5[PC25]
        PC6[PC4]
    end

    UI --> Log

    PC1 -- ICMP Ping --> PC2
    PC3 -- ICMP Ping --> PC4
    PC5 -- ICMP Ping --> PC6

    classDef pcStyle fill:#e1f5fe,stroke:#01579b,stroke-width:2px;
    classDef uiStyle fill:#f3e5f5,stroke:#4a148c,stroke-width:2px;
    classDef logStyle fill:#e8f5e8,stroke:#1b5e20,stroke-width:2px;
    
    class PC1,PC2,PC3,PC4,PC5,PC6 pcStyle;
    class UI uiStyle;
    class Log logStyle;

#Bus Topology Schematic
graph TB
    %% Main backbone nodes
    R1 --> R2
    R2 --> R3
    R3 --> R4
    R4 --> R5
    
    %% Skip many nodes for readability
    R5 --> R100
    R100 --> R200
    R200 --> R300
    R300 --> R400
    R400 --> R500
    R500 --> R600
    R600 --> R700
    
    %% Highlight repeated nodes
    R700 --> R728
    R728 --> R741
    R741 --> R748
    
    %% Show redundancy paths
    R728 -.-> R728
    R741 -.-> R741
    R748 -.-> R748
    
    %% Styling for repeated nodes
    class R728,R741,R748 redundant;
    classDef redundant fill:#f96;

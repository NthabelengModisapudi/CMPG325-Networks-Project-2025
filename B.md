graph LR
%% Highlight the repeated nodes area
    R705 --> R728
    R728 --> R729 --> R730 --> R731 --> R732 --> R733 --> R734 --> R735 --> R736
    
    %% Redundant node section
    R736 --> R741
    R741 --> R742 --> R743 --> R744 --> R745 --> R746
    
    R746 --> R748
    
    %% Show the redundancies as self-loops
    R728 -.-> R728
    R741 -.-> R741
    R748 -.-> R748
    
    class R728,R741,R748 redundant
    classDef redundant fill:#ff9999,stroke:#ff3333,stroke-width:2px

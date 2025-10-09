# Network Topology Documentation

## Star Topology
```mermaid
graph TD
    subgraph Star Topology
        S[Switch]
        S --> PC1[PC-PT PC1]
        S --> PC2[PC-PT PC2]
        S --> LTP1[Laptop-PT Laptop1]
        S --> PC3[PC-PT PC3]
    end

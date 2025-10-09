# Network Topology Documentation

## Star Topology
```mermaid
graph TD
    subgraph Star Topology
        S[Switch]
        S --> PC1[PC-PT PC7]
        S --> PC2[PC-PT PC8]
        S --> LTP1[Laptop-PT Laptop11]
        S --> PC3[PC-PT PC9]
        S --> LTP2[Laptop-PT Laptop1]
        S --> PC4[PC-PT PC6]

    end

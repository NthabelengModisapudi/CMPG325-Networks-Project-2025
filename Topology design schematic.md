# Network Topology Documentation
## Bus Topology
graph LR
    subgraph Point-to-Point Links
        PC5 -- ICMP --> PC23
        PC22 -- ICMP --> PC24
        PC25 -- ICMP --> PC4
    end

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

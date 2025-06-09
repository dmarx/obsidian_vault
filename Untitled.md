```mermaid
flowchart TD
    START([Start: Process K/V Tiles]) --> INIT[Initialize:<br/>M = -∞, L = 0, O = 0]
    
    INIT --> LOOP{For each K,V tile}
    
    LOOP --> LOAD[Load Q, K_i, V_i tiles]
    LOAD --> QK[Compute Q×K_i<br/>using tensor cores]
    QK --> SCALE[Scale by 1/√d]
    
    SCALE --> NEWMAX[Compute new row max:<br/>M_new = max(M_old, rowmax(QK_scaled))]
    
    NEWMAX --> RESCALE[Compute rescale factor:<br/>α = exp(M_old - M_new)]
    
    RESCALE --> SOFTMAX[Apply softmax to QK:<br/>P_i = exp(QK_scaled - M_new)]
    
    SOFTMAX --> ROWSUM[Compute row sum:<br/>L_new = α×L_old + rowsum(P_i)]
    
    ROWSUM --> UPDATE[Update output:<br/>O = α×O + P_i×V_i]
    
    UPDATE --> NEXT{More tiles?}
    NEXT -->|Yes| LOOP
    NEXT -->|No| FINAL[Final normalization:<br/>O = O / L_new]
    
    FINAL --> END([Output O])
    
    subgraph "Key Insight"
        INSIGHT[No need to store<br/>full attention matrix!<br/>Memory: O(N) not O(N²)]
    end
    
    style NEWMAX fill:#ffecb3
    style RESCALE fill:#ffecb3
    style UPDATE fill:#c8e6c9
    style INSIGHT fill:#f8bbd9
```

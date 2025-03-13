flowchart LR
    subgraph "Suppliers"
        A[Marpol]
        B[M-interio]
    end
    
    A --> W[Ambolo (Alwernia)\nWarehouse in Poland]
    B --> W
    
    W -- Ships Stock --> VM[Vitalmax Online (UK)]
    
    subgraph "Amazon"
        UK[Amazon UK]
        EU[Amazon EU]
        DE[Amazon DE]
        FR[Amazon FR]
        ES[Amazon ES]
        IT[Amazon IT]
    end
    
    VM -- Sells on --> UK
    VM -- Sells on --> EU
    EU --> DE
    EU --> FR
    EU --> ES
    EU --> IT

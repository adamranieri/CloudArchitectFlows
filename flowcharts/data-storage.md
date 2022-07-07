# Data Storage
Cloud Storage is the best storage option for most use cases. It should be the default option. It is
- Infinitely Scalable
- Cost Efficient
- Fully Managed by Google
- Reliable 
- Fast enough for most users 

# Choosing A storage Type
```mermaid

flowchart TD
    Start[I need to store unstructred data] --> Decision1{Any reason NOT to pick Cloud Storage}
    Decision1 -- No -->MobileDev{Is this for mobile Development}
    
    MobileDev --Yes--> Fire[Firebase Storage]
    MobileDev --No--> CloudStorage
    CloudStorage --> Frequency{Accessed more than onece per month}
    subgraph Storage Options
 
        Frequency -- yes --> Global{Globally Accessed?}
        Frequency -- no --> Often{Accessed less than once per year?}
        Often -- yes --> ColdLine
        Often -- no --> NearLine
        Global -- yes --> Multi[Multi-Regional Bucket]
        Global -- no --> Region[Regional Bucket]
    end

    Decision1-- Yes -->Decision2{What makes this data unique?}
    subgraph Other Options
        Decision2--file based? \n lift-shift? \n NAS? \n many writers to same instance-->CloudFileStore[Cloud File Store]
        Decision2-- max performance -->LocalSSD[Local SSD]
        Decision2-- GCE GKE storage -->PersistentDisk[Peristent Disk]
    end
```
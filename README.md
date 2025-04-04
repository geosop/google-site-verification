```mermaid
flowchart LR
    P["PAST"]
    C["PRESENT: Baseline Prediction Error ϵ₀"]
    F["FUTURE: Threshold Event P(F) > θ"]

    P -->|"Forward Causality"| C
    C -->|"Forward Causality"| F
    
    F ---|"Retrocausal Feedback <br/> Interference Term I(F) subtracts from ϵ₀ <br/> Modulates Neural State"| C


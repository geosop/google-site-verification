```mermaid
flowchart LR
    P[Past]
    C[Present (Baseline Prediction Error: ϵ₀)]
    F[Future (Threshold Event: P(F) > θ)]

    P -->|Forward Causality| C
    C -->|Forward Causality| F
    
    F ---|Retrocausal Feedback\n(Interference Term I(F) subtracts from ϵ₀)\nModulates neural state| C

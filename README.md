```mermaid
flowchart LR
    P[Past]
    C[Present\n(Baseline Prediction Error: ϵ₀)]
    F[Future\n(Threshold Event: P(F) > θ)]

    P -->|Forward Causality| C
    C -->|Forward Causality| F
    
    F ---|Retrocausal Feedback<br/>(Interference Term I(F) subtracts from ϵ₀)\nModulates neural state| C

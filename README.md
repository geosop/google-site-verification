```mermaid
flowchart LR
    P[Past]
    C[Present<br/>(Baseline Prediction Error: ϵ₀)]
    F[Future<br/>(Threshold Event: P(F) > θ)]

    P -->|Forward Causality| C
    C -->|Forward Causality| F
    
    F ---|Retrocausal Feedback<br/>(Interference Term I(F) subtracts from ϵ₀)<br/>Modulates neural state| C


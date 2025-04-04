```mermaid
graph LR
    P["Past"] -->|Forward Causality| C["Present\n(Baseline Prediction Error: ϵ₀)"]
    C -->|Forward Causality| F["Future\n(Threshold Event: P(F) > θ)"]
    F -.->|"Retrocausal Feedback\n(Interference Term I(F) subtracts from ϵ₀)\nModulates neural state"| C

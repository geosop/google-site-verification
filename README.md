```mermaid
graph LR
    P["Past"] -->|Forward Causality| C["Present\n(Baseline Prediction Error: ϵ₀)"]
    C -->|Forward Causality| F["Future\n(Threshold Event: P(F) > θ)"]
    F -.->|"Retrocausal Feedback\n(Interference Term I(F) subtracts from ϵ₀)\nModulates neural state"| C

flowchart LR
    %% Define nodes along a horizontal timeline
    P[Past]
    C[Present<br/>(Baseline Prediction Error: ϵ₀)]
    F[Future<br/>(Threshold Event: P(F) > θ)]
    
    %% Draw the standard forward causality arrow
    P -->|Forward Causality| C
    C -->|Forward Causality| F
    
    %% Draw the retrocausal feedback arrow (dashed for emphasis)
    F ---|Retrocausal Feedback<br/>(Interference Term I(F) subtracts from ϵ₀)<br/>Modulates neural state| C

```mermaid
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
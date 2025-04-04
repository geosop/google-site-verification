```mermaid
flowchart LR
    P[Past]
    C[Present (Baseline Prediction Error: ϵ₀)]
    F[Future (Threshold Event: P(F) > θ)]

    P -->|Forward Causality| C
    C -->|Forward Causality| F
    
    F ---|Retrocausal Feedback\n(Interference Term I(F) subtracts from ϵ₀)\nModulates neural state| C
✅ This version **removes** `<br/>` and instead **uses `\n`** to break the text into multiple lines.  

### **Steps to Fix the Issue on GitHub**
1. Open your `.md` file in an editor (VS Code, GitHub web editor, etc.).
2. Replace the Mermaid block with the corrected version above.
3. Save the file.
4. **Commit and Push the Changes:**
   ```sh
   git add README.md
   git commit -m "Fixed Mermaid diagram rendering"
   git push

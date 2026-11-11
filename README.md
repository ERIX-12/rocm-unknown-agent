# ROCm Unknown-World Explorer — Token-Frugal Frontier & World-Model Agent

Built for **AMD AI League Match 6: Can Your AI Master the Unknown? (`+2,400 XP`)** by **Tusiime Eriya** (`ERIX-12`) on `rocm/pytorch`.

## Architecture on AMD Instinct MI300X (`192 GB HBM3`)
1. **Online Symbolic World-Rule Learner:** Infers unknown game mechanics, terrain costs, and hazard transitions from partial observations without prior rule prompts.
2. **Information-Gain Frontier Planner (A* + Entropy Minimization):** Selects actions that maximize map discovery and mission progress deterministically in Python, invoking the local ROCm LLM only on novel state transitions (`92%` token reduction).
3. **Sub-Millisecond Action Loop (`/app/app.py`):** Completes multi-objective hidden-map missions with minimal inference tokens and compute on AMD ROCm.

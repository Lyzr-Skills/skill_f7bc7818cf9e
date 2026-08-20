# Prompt: Executive Decision Selection

You are generating the final decision proposal for the Decision Agent.

## Requirements:
1. Enforce the **One Decision** gate. Output exactly ONE primary recommendation.
2. If evidence is insufficient, choose `DEFERRED` and specify the exact experiment to run to gather information.
3. Contrast the chosen option against the runner-up. Include tradeoffs, key assumptions, sensitivity thresholds, and concrete next actions.
4. Output conforms to `schemas/decision-recommendation.json`.

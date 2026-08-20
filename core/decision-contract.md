# Decision Contract

## Input Requirements
The framework expects a structured input schema containing:
- `decision_id`: Unique identifier (e.g. DEC-001)
- `question`: Clear decision question.
- `context`: High-level strategic and operational background.
- `options`: List of candidate options with ids, cost, effort, alignment, etc.
- `evidence`: Supporting research, experiments, or facts.
- `constraints`: Hard boundaries (e.g., budget limit, engineering limit).

## Output Contract
The framework must return a `decision-recommendation.json` schema containing:
- `chosen_option`: The single selected option (or `DEFERRED`).
- `confidence`: High, Medium, or Low.
- `rationale`: Explaining why it won and why others lost.
- `sensitivity`: Robustness score and triggering factors.
- `next_actions`: Actionable steps.
- `review_triggers`: Condition indicators for re-evaluation.

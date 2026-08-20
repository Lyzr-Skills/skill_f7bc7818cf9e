# Decision Memory

Maintains historical logs of decisions to ensure long-term learning and optimization.

## Stored Fields:
- `decision_id`
- `question`
- `chosen_option`
- `context_at_decision_time`
- `expected_outcome`
- `actual_outcome`
- `was_correct` (Boolean / Null)
- `learnings_gained`

This structure allows GTMOS to audit and recognize systematic biases, such as: "We consistently overestimate the impact of paid acquisition."

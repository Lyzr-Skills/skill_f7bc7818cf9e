# Assumption Management

Assumptions must be logged and monitored to prevent silent failures.

## Fields:
- `assumption_id`: Unique identifier (e.g. ASM-001)
- `statement`: Plain text description.
- `impact_if_wrong`: High / Medium / Low.
- `confidence`: Score based on current evidence.
- `validation_method`: Concrete way to prove/disprove (e.g. "Run a 14-day experiment").

Assumptions with high impact and low confidence must be explicitly addressed in next actions.

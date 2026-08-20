# Usage Guide

## Invoking the Decision Framework
The framework operates as a subagent or reasoning tool inside GTMOS.

### Sample Input Payload
```json
{
  "decision_id": "DEC-101",
  "question": "Should we scale enterprise outbound or invest in partnership experiments?",
  "options": [
    {
      "option_id": "OPT-A",
      "name": "Scale Enterprise Outbound",
      "expected_impact": 8,
      "cost": 15000,
      "effort": 120,
      "reversibility": 4
    },
    {
      "option_id": "OPT-B",
      "name": "Partnerships Experiments",
      "expected_impact": 6,
      "cost": 2000,
      "effort": 30,
      "reversibility": 9
    }
  ]
}
```

### Command Execution
```bash
agy run decision-framework --input decision-input.json
```

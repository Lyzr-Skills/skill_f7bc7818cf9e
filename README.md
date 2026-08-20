# GTMOS Decision Framework

The Decision Framework is the core reasoning engine of GTMOS. Its primary job is not options generation, but taking a defined set of options, executing a structured decision process, accounting for uncertainty and constraints, and producing exactly one recommended decision or a specific deferred-decision action.

## Core Flow
```
Context → Decision Question → Available Options → Evidence → Evaluation Criteria →
Scoring → Trade-off Analysis → Risk/Reversibility Analysis → Decision → Rationale → Next Action
```

## Folder Structure
- `/core`: Reasoning principles, rules, logic, and state machine.
- `/config`: YAML/JSON files configuration for weights, profiles, and schemas.
- `/modules`: Specific analysis module guidelines.
- `/schemas`: Input/Output JSON data schemas.
- `/prompts`: LLM/Agent execution templates.
- `/tests`: Validation test suites.
- `/docs`: Usage and integration documentation.

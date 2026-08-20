# Decision Versioning

Rules for managing revisions when context changes.

## Schema Versioning Guidelines:
- Any update to assumptions, evidence, or constraints increments the minor version: `DEC-001 v1.0` → `DEC-001 v1.1`.
- Any shift in the chosen option or a restart of the decision pipeline increments the major version: `DEC-001 v1.0` → `DEC-001 v2.0`.
- Preserve the snapshot of evidence, scoring parameters, and assumptions for each version to guarantee auditability.

# Artifacts

> **Status:** Placeholder — not implemented in v0.1

## Purpose

The Artifacts layer defines the output schemas and delivery format for all documents produced by AI-AOS.

## Artifact Types

| Artifact | Description | Template |
|---|---|---|
| Executive Summary | High-level AI adoption narrative for leadership | `templates/executive-summary.md` |
| Pilot Plan | Structured plan for a Copilot pilot deployment | `templates/pilot-plan.md` |
| Training Plan | Role-based training schedule and content guidance | `templates/training-plan.md` |
| Governance Checklist | Policy and compliance requirements checklist | `templates/governance-checklist.md` |
| 90-Day Roadmap | Phased implementation roadmap | `templates/roadmap-90-days.md` |

## Future Implementation

In future releases, the Artifacts layer will include:

- JSON/YAML schema definitions for each artifact type
- Validation logic to ensure generated artifacts conform to expected structure
- Delivery formatters (Markdown, Word, PDF)
- Artifact manifest — a record of which artifacts were produced for a given input

## Related Files

- `templates/` — structural templates for each artifact type
- `output-examples/` — illustrative examples of generated artifacts

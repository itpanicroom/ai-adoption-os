# Readiness Agent

> **Status:** Placeholder — not implemented in v0.1

## Purpose

The Readiness Agent is responsible for the **Plan** and **Ready** phases of the Microsoft AI Cloud Adoption Framework. It assesses what the organization needs to have in place before deployment and produces a structured plan to close any gaps.

This Agent does not produce a maturity score. It produces a readiness checklist and a gap-closure plan — actionable next steps, not a rating.

## CAF Phase Coverage

**Plan · Ready**

## Inputs

- Organizational input profile (licenses, user count, departments, champions program status)
- Technical environment details (if provided)
- Cookbook: Plan and Ready phase guidance from applicable cookbook
- Scenario Pack: Technology-specific readiness requirements

## Outputs

- Technical readiness checklist
- Organizational readiness checklist
- Gap-closure action plan
- Training plan skeleton
- Champions program activation plan (if applicable)
- Pilot scope definition

## Responsibilities

1. Evaluate license availability and assignment readiness
2. Assess champions program presence and maturity
3. Identify technical prerequisites for deployment
4. Identify organizational prerequisites (governance, communications, training)
5. Produce a structured gap-closure plan aligned to CAF Plan phase
6. Define the scope and structure of the initial pilot
7. Generate the Training Plan and Pilot Plan artifacts

## Skills Invoked

- `technical-readiness.md` — Evaluate technical prerequisites
- `adoption-planning.md` — Structure the adoption plan
- `champions-program.md` — Plan the champions program activation
- `stakeholder-mapping.md` — Identify stakeholders for the rollout

## Future Implementation Notes

The Readiness Agent will produce structured checklists in v0.3. In v0.4, LLM integration will allow it to generate personalized gap-closure narratives based on what is missing from the organizational profile.

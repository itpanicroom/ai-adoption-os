# Strategy Agent

> **Status:** Placeholder — not implemented in v0.1

## Purpose

The Strategy Agent is responsible for the **Strategy phase** of the Microsoft AI Cloud Adoption Framework. It translates organizational context into a clear AI adoption strategy — establishing the business case, defining executive alignment, and setting the vision that all subsequent phases build upon.

## CAF Phase Coverage

**Strategy**

## Inputs

- Organizational input profile (company size, industry, executive sponsor status)
- Business objectives and priorities (if provided)
- Existing AI or digital transformation initiatives
- Cookbook: Phase-specific objectives from the Copilot Success Kit (or applicable cookbook)
- Scenario Pack: Business value context for the target technology

## Outputs

- AI adoption vision statement
- Business case summary
- Executive alignment plan
- Strategic objectives aligned to CAF Strategy phase
- Executive Summary artifact (routed to Artifacts layer)

## Responsibilities

1. Assess executive sponsor presence and engagement level
2. Define the business case for AI adoption in organizational context
3. Identify strategic objectives aligned to the AI CAF Strategy phase
4. Determine priority use cases based on organizational profile and Scenario Pack
5. Produce an executive alignment plan
6. Generate the Executive Summary artifact

## Skills Invoked

- `executive-alignment.md` — Structure the business case and executive narrative
- `stakeholder-mapping.md` — Identify key stakeholders for the strategy phase

## Future Implementation Notes

The Strategy Agent will use the organizational input profile to personalize the business case. In v0.4, LLM integration will allow the agent to generate narrative content grounded in the Cookbook and Scenario Pack.

# Orchestrator Agent

> **Status:** Placeholder — not implemented in v0.1

## Purpose

The Orchestrator Agent is the master coordinator of the AI-AOS system. It sits above all phase-specific agents and is responsible for the end-to-end execution of an adoption plan generation cycle.

Unlike the other agents (which own specific CAF phases), the Orchestrator Agent owns the entire lifecycle and delegates phase-specific work to the appropriate agents.

## CAF Phase Coverage

All phases: Strategy · Plan · Ready · Adopt · Govern · Manage

## Inputs

- Organizational input profile (JSON)
- Cookbook reference(s)
- Scenario Pack reference(s)
- Execution mode (full lifecycle vs. specific phase)

## Outputs

- Sequenced agent execution plan
- Consolidated artifact manifest
- Final assembled adoption plan (collection of all phase artifacts)

## Responsibilities

1. Validate the organizational input profile
2. Determine which CAF phases are in scope for this organization
3. Select the appropriate Cookbook(s) and Scenario Pack(s)
4. Invoke phase-specific agents in the correct sequence
5. Collect and assemble artifact outputs from all agents
6. Produce the final adoption plan

## Agent Interaction

The Orchestrator Agent invokes:
- Strategy Agent (Strategy phase)
- Readiness Agent (Plan + Ready phases)
- Adoption Agent (Adopt phase)
- Governance Agent (Govern phase)
- Measurement Agent (Manage phase)

## Future Implementation Notes

The Orchestrator Agent will be implemented as part of the v0.3 rules-based engine milestone. It will initially use deterministic sequencing logic, with LLM-based enrichment added in v0.4.

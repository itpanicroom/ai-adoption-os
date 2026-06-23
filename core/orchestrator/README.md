# Orchestrator

> **Status:** Placeholder — not implemented in v0.1

## Purpose

The Orchestrator is the coordination layer of AI-AOS. It receives an organizational input profile and determines which Agents to invoke, in what sequence, and with what parameters.

## Responsibilities

- Parse and validate organizational input
- Determine applicable CAF phases based on organizational context
- Invoke Agents in phase-appropriate sequence
- Route Cookbook and Scenario Pack references to Agents
- Collect Artifact outputs from all Agents
- Assemble the final adoption plan

## Future Implementation

In future releases, the Orchestrator will be implemented as:

1. A rules-based engine (v0.3) that applies deterministic logic to phase sequencing
2. An LLM-enhanced engine (v0.4) that uses AI to enrich and personalize adoption plans

## Related Files

- `core/agents/orchestrator-agent.md` — the Orchestrator Agent specification
- `docs/ARCHITECTURE.md` — full architectural context

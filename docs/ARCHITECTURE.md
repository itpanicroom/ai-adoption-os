# AI-AOS Architecture

## Overview

AI-AOS (AI Adoption Operating System) is built on a layered, modular architecture inspired by HVE-Core principles. Each layer has a single, well-defined responsibility. Layers communicate through defined inputs and outputs, making the system extensible without requiring changes to the core lifecycle.

---

## Architectural Principles

1. **Separation of Concerns** — Each layer (Orchestrator, Agents, Skills, Cookbooks, Scenario Packs) has an independent responsibility. No layer handles the concerns of another.

2. **Modularity** — New Cookbooks and Scenario Packs can be added without modifying the core orchestration logic.

3. **CAF Alignment** — All components map back to one or more phases of the Microsoft AI Cloud Adoption Framework.

4. **Input-Driven** — The system is driven by organizational context, not assumptions or fixed templates.

5. **Artifact-Oriented** — Every execution path ends in a concrete, usable artifact for the organization.

---

## Layer Diagram

```
┌─────────────────────────────────────────────┐
│                    INPUT                    │
│    Organizational context (JSON profile)    │
└────────────────────┬────────────────────────┘
                     │
┌────────────────────▼────────────────────────┐
│                ORCHESTRATOR                 │
│   Coordinates execution across agents and   │
│   CAF lifecycle phases                      │
└────────────────────┬────────────────────────┘
                     │
┌────────────────────▼────────────────────────┐
│                   AGENTS                    │
│   Phase-specific coordinators:              │
│   Strategy · Plan · Ready · Adopt           │
│   Govern · Manage                           │
└────────────────────┬────────────────────────┘
                     │
┌────────────────────▼────────────────────────┐
│                   SKILLS                    │
│   Reusable capabilities invoked by agents:  │
│   Executive Alignment · Stakeholder Mapping │
│   Technical Readiness · Champions Program   │
│   Communications · Role-Based Scenarios     │
│   Success Measurement · Optimization        │
└────────────────────┬────────────────────────┘
                     │
         ┌───────────┴───────────┐
         │                       │
┌────────▼────────┐   ┌─────────▼──────────┐
│   COOKBOOKS     │   │   SCENARIO PACKS    │
│                 │   │                     │
│ Knowledge assets│   │ Technology-specific │
│ aligned to CAF  │   │ adoption guidance   │
│ phases          │   │ scoped to roles and │
│                 │   │ use cases           │
└────────┬────────┘   └─────────┬──────────┘
         └───────────┬───────────┘
                     │
┌────────────────────▼────────────────────────┐
│                 ARTIFACTS                   │
│   Generated outputs consumed by users:      │
│   Plans · Checklists · Summaries · Roadmaps │
└─────────────────────────────────────────────┘
```

---

## Component Definitions

### Input

The Input layer represents the organizational profile — the context that drives all downstream decisions.

Inputs are structured JSON documents capturing:

- Company name and size
- License types (M365, Copilot, Azure, etc.)
- Executive sponsor presence
- Champions program status
- Departments in scope
- Deployment stage

See `sample-inputs/` for examples.

---

### Orchestrator

The Orchestrator is the coordination engine. It receives the Input and determines:

- Which Agents to invoke
- In what sequence
- With what parameters
- Against which Cookbooks and Scenario Packs

The Orchestrator enforces the CAF lifecycle order while allowing phases to be entered at different points depending on organizational maturity.

**Current status:** Placeholder — not implemented in v0.1.

See `core/orchestrator/` for structural definitions.

---

### Agents

Agents are phase-specific coordinators. Each Agent owns one or more CAF phases and is responsible for translating phase objectives into skill invocations.

| Agent | CAF Phase(s) | Responsibility |
|---|---|---|
| Orchestrator Agent | All | Cross-phase coordination |
| Strategy Agent | Strategy | Executive alignment, business case |
| Readiness Agent | Plan + Ready | Technical and organizational readiness |
| Adoption Agent | Adopt | Pilot design, rollout planning |
| Governance Agent | Govern | Policy, compliance, oversight |
| Measurement Agent | Manage | KPIs, success metrics, optimization |

See `core/agents/` for individual Agent specifications.

---

### Skills

Skills are reusable capabilities that can be invoked by any Agent. A Skill encapsulates a specific capability such as stakeholder mapping or communications planning.

Skills are intentionally decoupled from Agents — the same Skill may be relevant across multiple phases and used by multiple Agents.

See `core/skills/` for individual Skill specifications.

---

### Cookbooks

Cookbooks are knowledge assets aligned to specific Microsoft technologies or deployment patterns. Each Cookbook is structured around the six CAF phases and provides:

- Phase objectives
- Required inputs
- Checklist items
- Expected outputs
- Recommended next actions

**v0.1 Cookbook:** Copilot Success Kit (`cookbooks/copilot-success-kit/`)

---

### Scenario Packs

Scenario Packs provide technology-specific adoption guidance scoped to organizational roles and real-world use cases.

Where Cookbooks provide the structural framework, Scenario Packs provide the role-level detail — what Copilot does for a Sales rep versus a Finance analyst versus an HR business partner.

**v0.1 Scenario Pack:** Microsoft 365 Copilot (`scenarios/microsoft-365-copilot/`)

---

### Artifacts

Artifacts are the generated outputs of the system — the documents, plans, checklists, and roadmaps that organizations actually use.

| Artifact Type | Description |
|---|---|
| Executive Summary | High-level AI adoption narrative for leadership |
| Pilot Plan | Structured plan for a Copilot pilot deployment |
| Training Plan | Role-based training schedule and content guidance |
| Governance Checklist | Policy and compliance requirements checklist |
| 90-Day Roadmap | Phased implementation roadmap |

See `templates/` for structural templates and `output-examples/` for illustrative examples.

---

## CAF Lifecycle Backbone

The six phases of the Microsoft AI Cloud Adoption Framework are the permanent backbone of AI-AOS. No execution path exists outside this lifecycle.

```
Strategy → Plan → Ready → Adopt → Govern → Manage
```

This is not a linear waterfall. Organizations may enter at any phase and run phases concurrently. The Orchestrator manages sequencing based on organizational context.

---

## Extensibility Model

AI-AOS is designed for incremental extension:

| Extension Type | How to Add | Impact on Core |
|---|---|---|
| New Cookbook | Add directory under `cookbooks/` | None |
| New Scenario Pack | Add directory under `scenarios/` | None |
| New Skill | Add file under `core/skills/` | None |
| New Agent | Add file under `core/agents/` + register with Orchestrator | Minimal |
| New Artifact Template | Add file under `templates/` | None |

The core lifecycle — Orchestrator, Agents, Skills — does not need to change when new Cookbooks or Scenario Packs are added.

---

## Future Architecture Directions

See `docs/ROADMAP.md` for planned enhancements, including:

- LLM-based orchestration
- MCP (Model Context Protocol) integration
- Microsoft Graph integration
- Multi-tenant deployment patterns
- Continuous optimization feedback loops

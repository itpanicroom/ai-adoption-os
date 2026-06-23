# Time Capsule — AI-AOS v0.1

> This document records the scope decisions, design rationale, and intentional exclusions made at the v0.1 release boundary. It exists so that future contributors — and the future maintainers of this project — can understand exactly why v0.1 is what it is, and what it deliberately is not.

---

## Date

June 2025

---

## What v0.1 Is

v0.1 is the bootstrap release of AI-AOS. It establishes:

- A public repository with a clear, well-documented structure
- The architectural vision: Input → Orchestrator → Agents → Skills → Cookbooks → Scenario Packs → Artifacts
- The CAF lifecycle backbone (Strategy, Plan, Ready, Adopt, Govern, Manage) as the permanent framework
- A single Cookbook (Copilot Success Kit) covering all six CAF phases
- A single Scenario Pack (Microsoft 365 Copilot) with role-based use cases
- Placeholder definitions for six Agents and nine Skills
- Sample input and illustrative output examples
- Documentation for architecture, roadmap, and contribution guidelines

---

## What v0.1 Is Not

The following were explicitly and intentionally excluded from v0.1:

| Excluded Item | Reason for Exclusion |
|---|---|
| Orchestration engine | Premature to implement before the content layer is stable |
| LLM / AI implementation | The value is in the structure and knowledge, not the generation mechanism |
| MCP integration | Dependent on orchestration engine existing first |
| Microsoft Graph integration | Tenant-aware context adds complexity not needed for foundation |
| Dashboards | No data to display yet |
| Scoring engine | AI-AOS is explicitly not a scoring tool — this is a philosophical boundary |
| Maturity assessments | Same as above — the system answers "what next", not "how mature" |
| Application code | Premature — the knowledge layer must be proven first |
| APIs | No consumers yet |
| Databases | Nothing to persist yet |
| Authentication systems | No users to authenticate yet |
| Docker / infrastructure | Nothing to deploy yet |

---

## Key Design Decisions Made at v0.1

### 1. CAF as the permanent backbone

The six CAF phases (Strategy, Plan, Ready, Adopt, Govern, Manage) are the non-negotiable backbone of the framework. Every future component must map to these phases. This decision was made to ensure AI-AOS remains aligned with Microsoft's official guidance and is not a proprietary framework that will diverge over time.

### 2. Separation of Cookbooks and Scenario Packs

Cookbooks and Scenario Packs are intentionally different:

- **Cookbooks** are structured around the CAF lifecycle and provide phase-by-phase implementation guidance.
- **Scenario Packs** are structured around organizational roles and provide use-case-level detail.

Separating these two concerns allows each to evolve independently. A new Cookbook does not require a new Scenario Pack, and vice versa.

### 3. HVE-Core inspired layering

The architectural layering (Input → Orchestrator → Agents → Skills → ...) was chosen to enforce clean separation of concerns. This makes the system extensible without requiring core changes when new content is added.

### 4. Input-driven, not assumption-driven

AI-AOS is designed to be driven by organizational context. It does not make assumptions about where an organization is in its AI journey. The Input layer (organizational profile) is what drives all downstream decisions. This is a fundamental difference from fixed-template tools.

### 5. The system answers "what next", not "how mature"

This is the central philosophical decision. AI-AOS is not a maturity model. Maturity models are useful for benchmarking. AI-AOS is useful for planning. The two serve different purposes and should not be conflated.

---

## What the Future Should Build On

Future releases should:

1. Build the Orchestrator on top of the content layer established in v0.1 — do not redesign the content layer to fit the engine
2. Extend Cookbooks and Scenario Packs before adding complexity to the core
3. Validate the architecture against real organizational inputs before adding LLM capabilities
4. Preserve the CAF backbone — do not create phases or lifecycle stages that diverge from Microsoft's AI CAF
5. Keep the Artifact layer as the output target — every execution path should end in a usable document

---

## A Note to Future Contributors

If you are reading this in a future version of this project:

The reason v0.1 is so minimal is intentional. The goal was to prove the structure and the architecture before building the engine. If the structure is wrong, no amount of clever code will save it. If the structure is right, the engine becomes straightforward.

Build on the structure. Don't replace it.

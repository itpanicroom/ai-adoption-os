# AI-AOS Roadmap

> This roadmap outlines the planned expansion of AI-AOS across future releases. All items beyond v0.1 are directional — sequencing and scope may change based on community feedback and real-world adoption experience.

---

## Current Release: v0.1 — Foundation

**Status:** In development

**Scope:**
- Repository structure and documentation
- Single Cookbook: Copilot Success Kit
- Single Scenario Pack: Microsoft 365 Copilot
- Agent placeholder definitions (6 agents)
- Skill placeholder definitions (9 skills)
- Sample input and output examples
- No orchestration engine
- No AI implementation

**Goal:** Establish a credible, well-structured public foundation that communicates the vision and architecture clearly enough for contributors and early adopters to understand and extend it.

---

## v0.2 — Structured Output Generation

**Theme:** Make it produce something real.

**Planned additions:**
- Formalize the artifact schema (JSON or YAML definition of each artifact type)
- Create a prompt-based artifact generation layer (no LLM dependency — template-driven)
- Expand sample inputs for different organizational profiles (enterprise, SMB, public sector)
- Add a second scenario pack (candidate: Microsoft Azure OpenAI Service)
- Add a second cookbook (candidate: Azure AI Foundry)
- Expand role-based scenario coverage in M365 Copilot scenario pack

---

## v0.3 — Orchestration Engine (Non-AI)

**Theme:** Make it coordinate.

**Planned additions:**
- Implement a rules-based Orchestrator that reads an organizational input and produces a sequenced adoption plan
- Agent activation logic based on CAF phase and organizational context
- Skill invocation registry
- Output manifest (list of artifacts to produce for a given input)
- CLI entry point for running the Orchestrator against a sample input

---

## v0.4 — LLM Integration

**Theme:** Make it intelligent.

**Planned additions:**
- Replace template-driven generation with LLM-based artifact generation
- Prompt engineering for each artifact type, grounded in Cookbook content
- Support for multiple LLM backends (Azure OpenAI, OpenAI API)
- Structured output validation (generated artifacts validated against schemas)
- Context injection from Scenario Pack and Cookbook at generation time

---

## v0.5 — MCP Integration

**Theme:** Make it connectable.

**Planned additions:**
- MCP (Model Context Protocol) server interface for AI-AOS
- Expose Cookbooks and Scenario Packs as MCP resources
- Expose Agents as MCP tools
- Enable AI-AOS to be used as a context provider in Copilot Studio and similar platforms

---

## v0.6 — Microsoft Graph Integration

**Theme:** Make it context-aware.

**Planned additions:**
- Read organizational context from Microsoft Graph (license inventory, user counts, department structure)
- Pre-populate input profiles from Graph data
- Enrich adoption plans with tenant-specific recommendations

---

## v1.0 — Production-Ready Framework

**Theme:** Make it trustworthy.

**Planned additions:**
- Full test coverage for orchestration and generation logic
- Multi-tenant deployment patterns
- Security and compliance review
- Official documentation site
- Contribution pipeline for new Cookbooks and Scenario Packs
- Partner and community ecosystem foundations

---

## Beyond v1.0 — Long-Term Vision

- **Continuous optimization loops:** Feedback from deployed artifacts feeding back into the Orchestrator
- **Industry-specific scenario packs:** Healthcare, Financial Services, Manufacturing, Public Sector
- **Governance automation:** AI governance policy generation aligned to EU AI Act and NIST AI RMF
- **Measurement dashboards:** Adoption KPI tracking integrated with Viva Insights and M365 usage data
- **Community cookbook registry:** Open registry for community-contributed Cookbooks and Scenario Packs

---

## Version Summary

| Version | Theme | Key Capability |
|---|---|---|
| v0.1 | Foundation | Structure, docs, placeholders |
| v0.2 | Output Generation | Template-driven artifact creation |
| v0.3 | Orchestration Engine | Rules-based coordination |
| v0.4 | LLM Integration | AI-powered artifact generation |
| v0.5 | MCP Integration | Protocol-based connectivity |
| v0.6 | Graph Integration | Tenant-aware context |
| v1.0 | Production Ready | Full framework, tested and documented |

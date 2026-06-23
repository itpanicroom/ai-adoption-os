# Contributing to AI-AOS

Thank you for your interest in contributing to the AI Adoption Operating System. This document explains how contributions are structured and what kinds of contributions are most valuable.

---

## What We Welcome

AI-AOS is in bootstrap phase. The most valuable contributions at this stage are:

- **New Cookbooks** — implementation guidance for additional Microsoft AI technologies
- **New Scenario Packs** — role-based use case guidance for specific AI products
- **New Skill definitions** — reusable capability definitions that can be invoked across agents
- **Documentation improvements** — corrections, clarifications, and expansions to existing docs
- **Sample inputs** — new organizational profile examples representing different sizes, industries, and deployment stages
- **Output examples** — illustrative examples of generated adoption artifacts

We are **not** accepting contributions of application code, APIs, databases, authentication systems, or infrastructure deployments at this stage.

---

## Contribution Types

### Adding a Cookbook

Cookbooks live under `cookbooks/`. Each Cookbook represents a knowledge asset aligned to a specific Microsoft AI technology or deployment pattern.

**To add a Cookbook:**

1. Create a new directory under `cookbooks/` named after the technology (e.g., `cookbooks/azure-openai-service/`)
2. Add a `README.md` structured around the six CAF phases:
   - Strategy
   - Plan
   - Ready
   - Adopt
   - Govern
   - Manage

For each phase, document:
- **Objective** — What this phase achieves for this technology
- **Inputs** — What organizational information is required
- **Checks** — What readiness criteria must be met
- **Outputs** — What artifacts should be produced
- **Next Actions** — What happens after this phase

3. Open a pull request with a brief description of the technology and why this Cookbook is valuable.

---

### Adding a Scenario Pack

Scenario Packs live under `scenarios/`. Each Scenario Pack provides role-based adoption guidance for a specific AI product.

**To add a Scenario Pack:**

1. Create a new directory under `scenarios/` named after the product (e.g., `scenarios/azure-ai-foundry/`)
2. Add a `README.md` that documents:
   - The target product and deployment context
   - Role-based use cases (at minimum 4–5 organizational roles)
   - For each role: specific use cases, expected benefits, and adoption considerations

3. Open a pull request with context on why this Scenario Pack is needed.

---

### Adding or Updating a Skill

Skills live under `core/skills/`. Each Skill is a reusable capability invoked by Agents.

**To add a Skill:**

1. Create a new markdown file under `core/skills/` named after the capability (e.g., `data-governance.md`)
2. Include:
   - **Purpose** — What the Skill does
   - **CAF Phase** — Which CAF phase(s) this Skill applies to
   - **Expected Outputs** — What the Skill produces

3. Open a pull request with context on which Agent(s) would invoke this Skill.

---

### Improving Documentation

Documentation improvements are always welcome. This includes:

- Fixing typos or unclear language
- Expanding explanations
- Adding examples
- Improving structural clarity

For documentation-only changes, a pull request with a brief description is sufficient.

---

## Pull Request Guidelines

- Keep pull requests focused. One Cookbook, one Scenario Pack, or one logical change per PR.
- Include a clear description of what you are adding and why.
- Follow the existing structure and formatting of similar files.
- Do not include application code, build systems, or infrastructure files.

---

## Code of Conduct

Be respectful and constructive. This is an open framework designed to help organizations adopt AI successfully. Contributions should reflect that purpose.

---

## Questions

If you are unsure whether a contribution fits the scope of AI-AOS, open a GitHub Discussion before investing significant time in the contribution.

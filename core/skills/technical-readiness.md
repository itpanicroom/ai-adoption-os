# Skill: Technical Readiness

> **Status:** Placeholder — not implemented in v0.1

## Purpose

The Technical Readiness skill evaluates the technical prerequisites required for deploying an AI technology and produces a structured checklist of what must be in place before deployment begins.

This skill does not produce a maturity score. It produces a gap-closure checklist — a list of specific technical actions required to reach deployment readiness.

## CAF Phase

**Plan · Ready**

## Invoked By

- Readiness Agent

## Inputs

- Organizational input profile (license types, user count, Copilot license count)
- Cookbook: Ready phase technical prerequisites
- Scenario Pack: Technology-specific technical requirements

## Expected Outputs

- License readiness checklist (licenses assigned, Copilot seats allocated)
- Identity and access prerequisites checklist
- Data and content readiness checklist (SharePoint, OneDrive, Teams hygiene)
- Security and compliance prerequisites checklist
- Admin configuration checklist
- Technical gap-closure action plan with ownership and timelines

## Key Activities

1. Validate that required licenses are available and assigned correctly
2. Check identity prerequisites (Entra ID, MFA, conditional access)
3. Assess data and content hygiene (SharePoint architecture, sensitivity labels, permissions)
4. Validate security and compliance prerequisites
5. Identify admin configuration tasks required before deployment
6. Produce a prioritized gap-closure checklist

## Technical Prerequisites (M365 Copilot Reference)

| Area | Prerequisite |
|---|---|
| Licensing | Microsoft 365 E3/E5 or Business Premium + Copilot license |
| Identity | Entra ID, MFA enabled |
| Data | OneDrive, SharePoint, Exchange connected; sensitivity labels deployed |
| Security | Microsoft Purview configured; data loss prevention policies reviewed |
| Admin | Microsoft 365 Admin Center access; Copilot admin settings configured |

## Notes

Technical readiness is a prerequisite for a successful adoption experience. Organizations that skip this phase tend to have poor user experiences during pilot — which undermines adoption outcomes.

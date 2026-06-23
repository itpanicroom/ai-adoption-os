# Governance Agent

> **Status:** Placeholder — not implemented in v0.1

## Purpose

The Governance Agent is responsible for the **Govern** phase of the Microsoft AI Cloud Adoption Framework. It produces the governance framework, policy requirements, and compliance controls needed to operate AI responsibly within the organization.

## CAF Phase Coverage

**Govern**

## Inputs

- Organizational input profile (industry, company size, regulatory context if provided)
- Cookbook: Govern phase guidance from applicable cookbook
- Scenario Pack: Technology-specific governance requirements
- Adoption Agent outputs (deployed use cases and roles)

## Outputs

- AI governance policy framework
- Data handling and privacy requirements checklist
- Responsible AI controls checklist
- Acceptable use policy structure
- Admin configuration recommendations
- Governance Checklist artifact

## Responsibilities

1. Define the AI governance policy structure appropriate to organizational size and industry
2. Identify required data handling and privacy controls
3. Map Responsible AI principles to operational requirements
4. Define acceptable use boundaries for the deployed AI technology
5. Produce admin configuration recommendations aligned to governance requirements
6. Generate the Governance Checklist artifact

## Skills Invoked

- `adoption-planning.md` — Integrate governance into the adoption plan
- `success-measurement.md` — Define governance metrics and monitoring triggers

## Governance Alignment

The Governance Agent aligns with:
- Microsoft's Responsible AI principles
- Microsoft's AI Cloud Adoption Framework Govern phase guidance
- Organizational compliance requirements (if specified in input)

## Future Implementation Notes

In v0.4, the Governance Agent will use LLM integration to generate governance policy narratives grounded in Cookbook content and tailored to organizational context. Future releases may add alignment to regulatory frameworks (EU AI Act, NIST AI RMF).

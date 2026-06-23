# Adoption Agent

> **Status:** Placeholder — not implemented in v0.1

## Purpose

The Adoption Agent is responsible for the **Adopt** phase of the Microsoft AI Cloud Adoption Framework. It translates readiness outputs into a structured deployment and enablement plan — orchestrating the pilot, managing user enablement, and ensuring role-based scenarios are activated.

## CAF Phase Coverage

**Adopt**

## Inputs

- Organizational input profile (departments, user count, Copilot license count)
- Readiness Agent outputs (pilot scope definition, champions list)
- Cookbook: Adopt phase guidance from applicable cookbook
- Scenario Pack: Role-based use cases for target technology
- Training plan skeleton (from Readiness Agent)

## Outputs

- Pilot deployment plan
- User enablement schedule
- Role-based scenario activation guide
- Communications and launch plan
- Champions activation toolkit
- Pilot Plan artifact
- Training Plan artifact (completed)

## Responsibilities

1. Structure the pilot deployment based on departments and license count
2. Define the pilot user cohort and selection criteria
3. Map role-based scenarios from the Scenario Pack to pilot participants
4. Design the communications and launch sequence
5. Activate champions program touchpoints
6. Produce the Pilot Plan artifact
7. Finalize and produce the Training Plan artifact

## Skills Invoked

- `role-based-scenarios.md` — Map Scenario Pack use cases to pilot roles
- `communications-launch.md` — Design the launch communications plan
- `champions-program.md` — Activate champions during pilot
- `adoption-planning.md` — Structure phased adoption activities

## Future Implementation Notes

The Adoption Agent will use the Scenario Pack to generate role-specific activation content. In v0.4, LLM integration will allow the agent to draft communications templates and role-based scenario guides personalized to organizational context.

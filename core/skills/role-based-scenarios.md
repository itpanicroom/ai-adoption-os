# Skill: Role-Based Scenarios

> **Status:** Placeholder — not implemented in v0.1

## Purpose

The Role-Based Scenarios skill maps AI technology capabilities to specific organizational roles and real-world work activities. It translates generic product capabilities into concrete, believable use cases that employees in specific roles can immediately understand and try.

This is the skill that makes AI adoption feel relevant to individual employees — not just to the organization as a whole.

## CAF Phase

**Adopt · Manage**

## Invoked By

- Adoption Agent
- Measurement Agent

## Inputs

- Organizational input profile (departments in scope)
- Scenario Pack: Role-specific use cases for the target technology
- Adoption plan (which departments and roles are in scope for each phase)

## Expected Outputs

- Role-based scenario library (use cases mapped to each department/role)
- Quick reference cards for each role
- Training scenario examples for each role
- Champion talking points per role

## Key Activities

1. Map organizational departments to Scenario Pack role categories
2. Select the most relevant use cases for each role based on organizational context
3. Produce role-specific scenario descriptions in plain language
4. Create quick reference cards for pilot participants
5. Provide champions with role-specific talking points

## Role Mapping Reference (M365 Copilot)

| Organizational Department | Scenario Pack Role | Primary Use Cases |
|---|---|---|
| Sales | Sales | Meeting summaries, email drafting, CRM updates |
| HR | HR | Job description drafting, policy Q&A, onboarding materials |
| Finance | Finance | Report summarization, data analysis, presentation drafting |
| Operations | Operations | Process documentation, status reporting, cross-team coordination |
| Leadership | Executives | Briefing summaries, strategy documents, board presentation drafting |

## Notes

Role-based scenarios should be drawn from the active Scenario Pack. When a department is listed in the organizational input (e.g., `departments: ["Sales", "HR", "Finance"]`), the system should select scenarios relevant to those specific departments rather than generic capabilities.

# Skill: Communications and Launch

> **Status:** Placeholder — not implemented in v0.1

## Purpose

The Communications and Launch skill designs the internal communications strategy and launch experience for an AI deployment. It ensures that employees understand what is coming, why it matters, what to expect, and where to get help.

Poor communications is one of the leading causes of failed AI adoption. Employees who don't understand why they have a new tool don't use it — or use it poorly.

## CAF Phase

**Adopt**

## Invoked By

- Adoption Agent

## Inputs

- Organizational input profile (company size, departments, executive sponsor status)
- Stakeholder map (from Stakeholder Mapping skill)
- Adoption plan (from Adoption Planning skill)
- Scenario Pack: Role-specific value messaging for each department

## Expected Outputs

- Internal communications plan (timeline, channels, messages, owners)
- Pre-launch awareness communications (email templates, intranet content)
- Launch day communications (announcement, quick-start guide)
- Post-launch reinforcement communications (success stories, tips)
- Manager communications kit (how to support their team's adoption)
- Executive announcement message

## Key Activities

1. Define the communications timeline aligned to the adoption plan phases
2. Identify communications channels (email, Teams, intranet, town halls)
3. Develop role-specific value messaging sourced from the Scenario Pack
4. Design the pre-launch, launch, and post-launch communications cadence
5. Produce manager and executive communications kits
6. Define a feedback and questions channel for employees

## Communications Cadence

| Timing | Audience | Message |
|---|---|---|
| 4 weeks before launch | All employees | "Something is coming" awareness |
| 2 weeks before launch | Pilot cohort | Invitation and what to expect |
| Launch day | Pilot cohort | Welcome, quick-start, where to get help |
| Week 2 post-launch | Pilot cohort | Tips, use cases, early wins |
| Broad deployment | All licensed users | Launch announcement, getting started guide |
| Monthly | All users | Tips, success stories, new use cases |

## Notes

Executive-voiced communications significantly increase perceived importance and adoption. If an executive sponsor is present (as indicated by `executiveSponsor: true` in the input profile), communications should include an executive launch message.

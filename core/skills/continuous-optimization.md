# Skill: Continuous Optimization

> **Status:** Placeholder — not implemented in v0.1

## Purpose

The Continuous Optimization skill designs the feedback loop that keeps AI adoption improving after the initial deployment. It translates measurement data, user feedback, and new capabilities into updated adoption plans — ensuring AI adoption remains a living initiative rather than a one-time project.

## CAF Phase

**Manage**

## Invoked By

- Measurement Agent

## Inputs

- Measurement framework outputs (from Success Measurement skill)
- User feedback data (survey results, support tickets, champion feedback)
- New product capabilities (from vendor release notes, Scenario Pack updates)
- Organizational changes (new departments, new use cases, personnel changes)

## Expected Outputs

- Optimization review cadence plan
- Feedback collection mechanism design
- Use case expansion roadmap
- Optimization trigger criteria (what data points initiate a review)
- Updated adoption plan recommendations

## Key Activities

1. Design the feedback collection mechanism (surveys, usage analytics, champion feedback)
2. Establish the optimization review cadence (monthly, quarterly)
3. Define the optimization triggers — what data thresholds prompt a plan revision
4. Design the use case expansion pathway (how to add new scenarios after initial deployment)
5. Produce recommendations for the next adoption cycle based on current metrics

## Optimization Loop

```
Deploy → Measure → Collect Feedback → Review → Optimize → Deploy
```

This loop runs continuously after the initial deployment. Each cycle produces updates to the adoption plan and may trigger new phases or activities.

## Optimization Triggers

| Trigger | Action |
|---|---|
| Active user rate < 40% after 60 days | Champion re-activation, additional training |
| User satisfaction score < 3.5/5 | Use case review, support enhancement |
| Department not yet onboarded | Expansion planning |
| New product feature released | Scenario Pack update, champion briefing |
| Organizational restructure | Stakeholder map refresh |

## Notes

Continuous optimization is what separates organizations that sustain AI adoption from those that experience an initial spike and then decline. This skill should be activated no later than 30 days after initial deployment.

# Measurement Agent

> **Status:** Placeholder — not implemented in v0.1

## Purpose

The Measurement Agent is responsible for the **Manage** phase of the Microsoft AI Cloud Adoption Framework. It defines the success metrics, monitoring approach, and continuous optimization loop that keeps AI adoption on track after deployment.

## CAF Phase Coverage

**Manage**

## Inputs

- Organizational input profile
- Adoption Agent outputs (deployed use cases, pilot results)
- Cookbook: Manage phase guidance from applicable cookbook
- Scenario Pack: Technology-specific success metrics and KPIs

## Outputs

- Success metrics framework
- KPI definitions aligned to deployed use cases
- Monitoring and reporting cadence plan
- Optimization trigger criteria
- 90-Day Roadmap artifact
- Continuous optimization plan

## Responsibilities

1. Define success metrics appropriate to the deployed AI technology and organizational context
2. Establish KPIs for each deployed use case
3. Define the reporting cadence (weekly, monthly, quarterly)
4. Identify optimization triggers — what conditions prompt a review or change
5. Produce the 90-Day Roadmap artifact with measurement milestones
6. Define the feedback loop from measurement to next adoption cycle

## Skills Invoked

- `success-measurement.md` — Define and structure KPIs and metrics
- `continuous-optimization.md` — Design the optimization feedback loop
- `role-based-scenarios.md` — Map metrics to role-specific outcomes

## Measurement Philosophy

The Measurement Agent does not produce maturity scores. It produces:

- **Activity metrics** — Are users using the technology?
- **Outcome metrics** — Is it producing business value?
- **Adoption metrics** — Is adoption expanding over time?

These metrics feed back into the Orchestrator to inform the next adoption cycle.

## Future Implementation Notes

In v0.4, the Measurement Agent will generate personalized KPI frameworks based on the Scenario Pack and deployed use cases. Future integration with Microsoft Viva Insights and M365 usage analytics will enable pre-populated measurement baselines.

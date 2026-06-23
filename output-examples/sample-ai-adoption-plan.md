# Sample AI Adoption Plan — Contoso

> **Note:** This document is an illustrative example of the type of adoption plan AI-AOS is designed to generate. It was produced against the sample input in `sample-inputs/business-premium-smb.json`. In a production system, this document would be generated automatically by the Orchestrator, driven by the Copilot Success Kit Cookbook and the Microsoft 365 Copilot Scenario Pack.

---

**Organization:** Contoso  
**Total Users:** 120  
**License Tier:** Microsoft 365 Business Premium  
**Copilot Licenses:** 25 (initial pilot cohort)  
**Executive Sponsor:** Yes (confirmed)  
**Champions Program:** Not yet established  
**Departments in Scope:** Sales, HR, Finance  
**Plan Generated:** June 2025  
**AI-AOS Version:** v0.1  

---

## Executive Summary

Contoso is deploying Microsoft 365 Copilot to 25 users across its Sales, HR, and Finance teams. With an executive sponsor in place and a Business Premium license foundation, Contoso has the necessary foundations for a successful deployment.

The primary opportunity is productivity improvement across three high-value functions: accelerating the Sales cycle through faster communications and meeting follow-up; improving HR efficiency in document creation and policy Q&A; and enabling Finance to produce cleaner, faster reporting.

The primary risk is the absence of an established champions program. Building a champions network during the Plan phase is the single most important first action for Contoso to ensure sustainable adoption beyond the initial pilot.

The recommended approach is a 6-week pilot with all 25 licensed users (representing 21% of total workforce), followed by an assessment and decision on license expansion.

---

## Organizational Context Assessment

| Factor | Status | Implication |
|---|---|---|
| Executive sponsor | ✅ Present | Accelerates strategic alignment and communications impact |
| Champions program | ❌ Not established | Must be built during Plan phase — priority action |
| License availability | ✅ 25 Copilot licenses ready | Sufficient for a meaningful pilot |
| Departments in scope | Sales, HR, Finance | Strong use case coverage; high ROI potential |
| Company size | 120 users | SMB profile — lean governance approach appropriate |
| License tier | Business Premium | All required prerequisites included |

---

## Recommended CAF Phase Activities

### Phase 1: Strategy ✅ (Complete — based on input)

**Status:** Executive sponsor confirmed. Proceeding to Plan phase.

**Completed:**
- Business case established (productivity improvement in Sales, HR, Finance)
- Executive sponsor identified and committed
- Primary deployment technology confirmed (Microsoft 365 Copilot)

---

### Phase 2: Plan

**Priority actions for Contoso:**

1. **Build the champions program** — With no existing champions program, Contoso should recruit 1–2 champions from each department (Sales, HR, Finance) — approximately 4–5 champions for the pilot. These individuals should be identified and onboarded before the pilot starts.

2. **Scope the pilot cohort** — With 25 licenses available and 3 departments, recommend the following cohort:
   - Sales: 10 users (including 1 sales manager)
   - HR: 7 users (including HR lead)
   - Finance: 8 users (including finance manager)

3. **Design training by role** — Training should be structured around Sales, HR, and Finance scenarios (see Scenario Pack). Generic training is insufficient for SMB audiences with limited time.

4. **Define success metrics** — Establish baseline measurements before deployment (meeting volume, email volume, time on document creation) to enable post-deployment comparison.

**Outputs:**
- Pilot cohort list (25 users confirmed)
- Champions shortlist (4–5 candidates)
- Training curriculum outline
- Pilot timeline (recommended: 6 weeks from Plan phase completion)

---

### Phase 3: Ready

**Technical prerequisites for Contoso (Business Premium):**

All required licenses are included in Microsoft 365 Business Premium + Copilot add-on. Priority technical tasks:

| Task | Priority | Owner |
|---|---|---|
| Assign Copilot licenses to pilot cohort in Microsoft 365 Admin Center | Mandatory | IT / Admin |
| Verify MFA is enabled for all 25 pilot users | Mandatory | IT / Admin |
| Review SharePoint and OneDrive usage hygiene | Mandatory | IT / Admin |
| Confirm sensitivity labels deployed (at minimum Confidential / General) | Recommended | IT / Admin |
| Review Microsoft Purview DLP policies | Recommended | IT / Admin |

> **Note for Contoso:** As a Business Premium customer, Contoso has access to Microsoft Purview through its license. Setting up basic sensitivity labels before Copilot activation is strongly recommended to prevent unintended oversharing.

**Organizational prerequisites:**

| Task | Priority | Owner |
|---|---|---|
| Champion recruitment confirmed (4–5 individuals) | Mandatory | HR / Project Lead |
| Champion onboarding session delivered | Mandatory | Training Lead |
| Role-based training materials prepared for Sales, HR, Finance | Mandatory | Training Lead |
| Help desk briefed on expected Copilot support queries | Recommended | IT / Admin |

---

### Phase 4: Adopt

**Pilot Plan Summary — Contoso**

**Pilot Period:** 6 weeks  
**Pilot Cohort:** 25 users — Sales (10), HR (7), Finance (8)  
**Champions:** 1 per department (3–4 total)

**Week-by-Week Overview:**

| Week | Focus | Key Activities |
|---|---|---|
| Week 1 | Launch | Launch communications; welcome session; champions activate |
| Week 2 | First use | Tip of the week (meeting summaries); first feedback pulse |
| Week 3 | Role-based activation | Role-specific scenario workshops (Sales, HR, Finance) |
| Week 4 | Mid-pilot review | Usage data review; mid-pilot survey; champion community call |
| Week 5 | Optimization | Address top issues; share early wins |
| Week 6 | Assessment | Final survey; usage analysis; pilot report |

**Top Use Cases by Department:**

*Sales (10 users)*
- Meeting follow-up email drafting after client calls
- Proposal section drafting from client briefs
- Account briefing preparation before calls

*HR (7 users)*
- Job description drafting from role briefs
- Onboarding material creation
- Policy Q&A from SharePoint policy documents

*Finance (8 users)*
- Financial report narration (data to executive summary)
- Variance analysis talking points
- Contract and document summarization

---

### Phase 5: Govern

**Governance Framework — SMB Edition (Contoso)**

For a 120-person organization on Business Premium, a lightweight but complete governance framework is appropriate.

**Mandatory governance actions:**

1. **Acceptable use policy** — Draft a 1-page Copilot acceptable use policy. Key points:
   - Do not input personally identifiable information (PII) of customers or employees into Copilot prompts
   - Do not input confidential financial data in shared Copilot environments
   - Always review and validate Copilot outputs before sharing or acting on them
   - Do not use Copilot to make autonomous decisions about people (hiring, performance, etc.)

2. **Data handling guidance** — Communicate that Copilot does not store prompts or outputs outside Microsoft 365. Copilot accesses only content the user has permission to access.

3. **Admin configuration** — Review Copilot plugin settings in Microsoft 365 Admin Center. For Contoso's profile, default settings are appropriate with minor adjustments.

**Governance review cadence:** Quarterly for the first year.

---

### Phase 6: Manage

**90-Day Success Metrics — Contoso**

| Metric | Target at Day 90 | Measurement |
|---|---|---|
| Active weekly users | ≥18 of 25 licensed (72%) | M365 Admin Center |
| User satisfaction | ≥3.5/5 | Post-deployment survey |
| Training completion | 25 of 25 users (100%) | Training records |
| Use cases activated per user | ≥3 | Survey self-report |
| Champions retained | 3 of 3–4 (75%+) | Champion engagement log |

**Recommended expansion path after Day 90:**

1. Assess pilot results and user satisfaction
2. If targets met: recommend license expansion to additional 25–50 users
3. Prioritize departments not yet covered (Operations if applicable)
4. Activate advanced use cases for pilot users (Copilot in Word, PowerPoint, Excel deep-dive)
5. Begin planning for potential Microsoft Copilot Studio use cases (FY2 consideration)

---

## Champions Program Activation Plan (Priority Action)

Because Contoso does not have an existing champions program, this must be built from scratch.

**Step 1 — Identify candidates (Week 1 of Plan phase)**
- Ask each department head to nominate 1–2 colleagues who:
  - Embrace new technology enthusiastically
  - Are respected by their peers
  - Have time to support colleagues alongside their main role

**Step 2 — Onboard champions (Week 2 of Plan phase)**
- 90-minute virtual onboarding session covering:
  - What Microsoft 365 Copilot does and how to get value from it
  - Their role as a champion (peer support, not IT helpdesk)
  - Role-specific use cases for their department
  - How to handle common questions and where to escalate

**Step 3 — Activate during pilot**
- Champions are first to receive Copilot access (1 week before pilot launch)
- Champions reach out proactively to their department cohort in Week 1
- Champions host informal 30-minute "how are you getting on?" sessions in Week 2–3
- Champions participate in monthly community call

---

## Risk Register

| Risk | Likelihood | Impact | Mitigation |
|---|---|---|---|
| Low pilot adoption | Medium | High | Champions program + executive-voiced launch communications |
| No champions program established | Already identified | High | Prioritize champion recruitment as Week 1 Plan phase activity |
| Technical prerequisites delayed | Low | High | Begin IT prerequisites in parallel with Plan phase |
| User concern about AI replacing jobs | Medium | Medium | Transparent communications; emphasize augmentation not replacement |
| Governance gaps (data oversharing) | Low | Medium | Sensitivity labels + acceptable use policy before launch |

---

*This document was generated as a sample output illustrating the type of AI adoption plan AI-AOS is designed to produce. In production, all sections marked with `[placeholder]` in the templates would be populated from the organizational input profile, the Copilot Success Kit Cookbook, and the Microsoft 365 Copilot Scenario Pack.*

*Generated by AI-AOS v0.1 | Copilot Success Kit Cookbook + Microsoft 365 Copilot Scenario Pack*

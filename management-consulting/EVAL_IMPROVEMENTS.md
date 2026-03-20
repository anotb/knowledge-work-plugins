# Evaluation Improvements: Management Consulting Skills

Compiled from execution evals (17 skills) and review-style evals (13 skills reviewed).
Generated 2026-03-20.

---

## Cross-Cutting Improvements (Apply to Multiple Skills)

These patterns appeared across nearly every skill evaluation. Implementing them would produce the highest aggregate quality improvement.

### 1. Add Worked Examples [HIGH]

**Applies to:** ALL 17 skills
**Source:** Every eval (execution and review) flagged this.

No skill currently includes a worked example. Every eval recommended adding at least one end-to-end example (even abbreviated) showing the framework applied to a specific scenario. This is the single highest-leverage improvement across the entire skill set.

For each skill, add a brief (10-30 line) worked example showing:
- Input: a realistic prompt/scenario
- Output: what good looks like, annotated with which part of the framework drives each section

The execution evals showed that the WITH-skill outputs were significantly better than WITHOUT, but the model still had to compose the steps together from description alone. An example anchors quality.

### 2. Add "So What?" / Synthesis Discipline [HIGH]

**Applies to:** problem-solving, strategic-frameworks, implementation-planning, financial-modeling, exec-presentation, report-generation

Multiple skills produce rigorous analysis but don't force synthesis. Add explicit guidance:
- Synthesis is NOT summary ("we found X" vs "X means Y, which changes our recommendation to Z")
- Lead with the answer (Pyramid Principle)
- Each framework/section should end with a 1-2 sentence "so what?" stating the single most important implication

### 3. Add Output Calibration / Depth Guidance [HIGH]

**Applies to:** strategic-frameworks, implementation-planning, report-generation, exec-presentation, proposal-development

Skills produce one output at maximum depth. Add guidance on calibrating depth to audience/use case:
- Executive summary (500-800 words)
- Working analysis (2,000-4,000 words)
- Deep dive (4,000-8,000 words)

### 4. Add Data Confidence Markers [HIGH]

**Applies to:** strategic-frameworks, financial-modeling, due-diligence, report-generation, implementation-planning

When working without access to proprietary client data or real-time market data:
- Flag estimates with confidence level: "~$30B (industry estimate, +/- 15%)"
- Distinguish between directionally certain and precisely uncertain
- Identify the 2-3 data points that would most change recommendations
- Recommend specific data sources the client should validate against

### 5. Trim Human-Only Content [MEDIUM]

**Applies to:** problem-solving, financial-modeling, engagement-setup

Remove or reframe content that applies to human analysts but not to Claude:
- problem-solving: "Fact-Finding Best Practices" section (interviews, "listen more, talk less")
- financial-modeling: "Model Standards" section (spreadsheet hygiene, cell-level comments), "Forecasting Techniques" (ML-based forecasting), Monte Carlo (reframe as "describe the simulation design")
- engagement-setup: Interview logistics that assume physical presence

### 6. Add Cross-References Between Skills [MEDIUM]

**Applies to:** All skills

Several skills naturally connect but don't reference each other:
- org-design should reference change-management
- implementation-planning should reference change-management ("change management hooks")
- pricing-strategy should reference proposal-development
- project-governance should include self-contained closure guidance (not just punt to project-closeout)
- engagement-setup should reference proposal-development SOW section ("Start with the SOW")

### 7. Add Industry-Specific Guidance [MEDIUM]

**Applies to:** proposal-development, engagement-setup, change-management, due-diligence, process-excellence

Even a brief table mapping industry to "emphasize these considerations" would help:
- Healthcare: HIPAA, clinical quality, patient safety
- Financial services: regulatory requirements, data security, vendor risk
- Government/public sector: procurement rules, past performance, small business participation
- Technology/SaaS: SaaS metrics (NRR, LTV/CAC, CAC payback, Rule of 40)

### 8. Add Key Assumptions Section [MEDIUM]

**Applies to:** strategic-frameworks, financial-modeling, implementation-planning, due-diligence

When client context is incomplete, explicitly list 3-5 assumptions at the top of the analysis. Flag which assumptions most affect the conclusions (sensitivity).

### 9. Add Artifact / Output Templates [MEDIUM]

**Applies to:** project-governance, org-design, pricing-strategy, report-generation

Skills describe what sections to include but don't specify the artifact format (e.g., "produce a 2-page project charter" or "produce a 1-page pricing summary for the proposal"). More explicit artifact specs would make outputs directly usable as client deliverables.

---

## Per-Skill Improvements

Skills are ordered by eval delta (largest improvement opportunity first).

---

### Problem Solving

**Eval scores:** WITH avg 8.75, WITHOUT avg 6.0, delta +2.75. Weakest dimension: Depth (+2.3).

#### HIGH Priority

1. **Add "Day 1 Hypothesis" prompt in Step 4.** Push for forming a Day 1 answer (initial hypothesis of the final recommendation). Include: a complete sentence answering the original question, confidence level (low/medium/high), and the 1-2 analyses that would most change your mind.

2. **Add quantification guidance in Step 1 (Problem Definition).** "Size the problem. What is the financial impact of the status quo? What is the value of solving it? Anchor all subsequent prioritization to these numbers."

3. **Expand the synthesis section (Step 6) with Pyramid Principle guidance.** Current section is too thin. Add: synthesis structure (Answer > 3 supporting arguments > Evidence), anti-patterns to avoid (restating findings without interpretation, burying the answer, presenting in analysis order rather than argument order).

4. **Add worked example.** One problem going through all 7 steps, even abbreviated. (See cross-cutting #1.)

5. **Add "structuring mode" vs. "analysis mode" guidance.** Clarify how to be useful when no data is available (structuring the analysis) vs. when data is provided (running the analysis). This is the most common use case and the skill doesn't acknowledge the constraint.

#### MEDIUM Priority

6. **Add "Validate the premise" as explicit step.** "Is the data reliable? Is the comparison fair? Is the stated problem actually a problem, or a solution looking for justification?"

7. **Add more issue tree templates.** Expand the table with: Cost reduction (MECE cost waterfall), Build vs. buy (Strategic fit + Economics + Execution risk), Pricing strategy, Org effectiveness, M&A evaluation.

8. **Deepen prioritization step.** Add 2x2 impact/feasibility method or "rank branches by estimated impact and data availability."

9. **Add "root cause analysis" and "diagnostic" to description trigger terms.**

#### LOW Priority

10. **Clarify when to use Hypothesis Tree vs. Logic Tree.** Add one sentence distinguishing the two.

11. **Cut "Fact-Finding Best Practices" section** (interviews, "listen more, talk less" are irrelevant to LLM). Or reduce to 3-4 items specific to analytical work.

12. **Cut or reduce "Key Principles" section** (mostly restates the process).

---

### Strategic Frameworks

**Eval scores:** WITH avg 8.7, WITHOUT avg 5.3, delta +3.4. Best dimension: Consulting-grade (+4.7).

#### HIGH Priority

1. **Add explicit quantification examples (3-4 templates).** Market share, Risk, Timing, Investment. The single example in Behavioral Principles isn't enough.

2. **Add a "So What?" forcing function to each framework section.** "End each framework with a 1-2 sentence 'So What?' that states the single most important implication."

3. **Add "Risks and Mitigations" to Framework Synthesis template.** Risk description, Likelihood, Impact, Mitigation, and identification of the "single point of failure."

4. **Add depth-calibration note.** "For standalone framework analysis, aim for 4-6 factors per dimension with 2-3 sentences of reasoning each. For multi-framework synthesis, keep individual analyses tighter."

#### MEDIUM Priority

5. **Add "Key Assumptions" section requirement.** When client context is incomplete, list 3-5 assumptions prominently, flag sensitivity.

6. **Strengthen Strategy Canvas section with explicit ERRC table format.** Eliminate / Reduce / Raise / Create grid with Rationale column.

7. **Add "Don't Use" column to Framework Selection Guide.** Prevent redundant or misleading framework combinations.

8. **Add Platform Strategy to Framework Selection Guide table.** Currently missing despite being covered in the skill.

9. **Add Data Confidence Markers section.** (See cross-cutting #4.)

#### LOW Priority

10. **Cut "Context Adaptation" section.** Redundant with Behavioral Principles.

11. **Deduplicate Market Sizing with problem-solving skill.** Cross-reference instead.

---

### Financial Modeling

**Eval scores:** WITH avg 9.25, WITHOUT avg 5.25, delta +4.0. Strongest dimension: Structure (+5).

#### HIGH Priority

1. **Add a worked numerical example.** A 3-year NPV calculation with 5-6 line items showing expected output format with tables.

2. **Add SaaS-specific metrics section.** NRR, LTV/CAC, CAC payback period, Rule of 40, gross margin by revenue type. These are table stakes for SaaS valuations and the skill doesn't mention them.

3. **Expand DCF section.** Include: revenue projection methodology (growth rate decay), UFCF calculation from EBITDA, terminal value calculation mechanics.

4. **Add "Phased Investment" pattern.** Phase 1 (Pilot) with success criteria > Gate Decision with metrics/thresholds > Phase 2 (Scale). Show NPV for both "Phase 1 only" and "Full program."

5. **Strengthen "Do Nothing" baseline as structural element.** Ongoing costs, cost escalation, risk costs, opportunity costs. Every business case must quantify the cost of inaction.

#### MEDIUM Priority

6. **Add guidance on interpreting client inputs.** "When clients provide percentage improvements, clarify the base. Distinguish rate vs. cost vs. outcome improvements."

7. **Strengthen recommendation section template.** Decision (Go/No-Go/Conditional) + Conditions + Immediate next steps + Decision reversibility + Timeline/urgency.

8. **Add capex vs. opex distinction.** Matters for financial statements and CFO evaluation. Cloud migration cases often justified partly on capex-to-opex shift.

9. **Add explicit guidance on table formatting for financial outputs.** Consulting financial models are table-heavy; Claude defaults to prose.

#### LOW Priority

10. **Cut "Model Standards" section or reframe for text-based output.** Spreadsheet hygiene is irrelevant to Claude.

11. **Cut or rework "Forecasting Techniques" section.** ML and anomaly detection lines are not actionable.

12. **Reframe Monte Carlo as "describe the simulation design"** rather than "run simulations."

13. **Trim description.** At 50+ words, it's slightly overloaded and may dilute signal.

---

### Proposal Development

**Eval scores:** WITH avg 9.0, WITHOUT avg 5.75, delta +3.25.

#### HIGH Priority

1. **Add pricing strategy sub-stage.** When to use fixed fee vs. T&M vs. blended. How to position pricing relative to evaluation weight. Rate card construction. How to handle "budget not disclosed."

2. **Add "Red Team / Quality Review" guidance.** Score your own proposal against evaluation criteria. Identify weakest section. Check compliance gaps. Test executive summary standalone. Verify cross-section consistency.

3. **Add oral presentation / defense guidance.** How to structure 30/45/60-minute presentations. Who presents which sections. Q&A handling (preparation, team roles, parking lot technique). Rehearsal guidance.

#### MEDIUM Priority

4. **Strengthen client responsibilities guidance in SOW.** Data access timelines/SLAs, decision-making authority/turnaround times, internal resource commitment levels (% dedication not just names), consequences when client dependencies aren't met.

5. **Add "proposal recovery" guidance for losing positions.** How to reframe evaluation criteria. When/how to propose alternative scope. Using pricing structure to de-risk client's decision.

6. **Tighten Value Proposition validation.** If Differentiation fails: checklist of potential differentiators. If Belief fails: hierarchy of evidence strength (quantified case study > named reference > methodology certification > team credentials > assertion).

7. **Address customization vs. reuse.** What must be customized every time, what can be adapted, what should never be boilerplate, common tells that scream "boilerplate."

8. **Trim Section 2b (Messaging Hierarchy).** Stakeholder-level messages table is generic. Merge or reduce.

#### LOW Priority

9. **Add multi-party / teaming guidance.** When to team vs. go solo, how to present teaming, subcontractor roles.

10. **Add industry-specific guidance hooks.** Note that certain industries have unique proposal requirements.

11. **Add post-submission follow-up/debrief process.**

---

### Engagement Setup

**Eval scores:** WITH avg 8.75, WITHOUT avg 5.0, delta +3.75. Review score: 9/10 (highest of batch).

#### HIGH Priority

1. **Add "Day 1 checklist."** The 10 things you do on literal Day 1: confirm sponsor, get billing codes, set up shared drive, draft data request, schedule kickoff, pull prior work on this client.

2. **Add "Sales-to-Delivery Transition" section.** What did the partner promise? What's in the SOW? What did the client hear that isn't in the SOW? Interview the sales lead. Check for scope gaps.

3. **Add hypothesis-driven discovery framing.** "Enter discovery with 2-3 initial hypotheses. Use interviews to test these, not confirm them."

4. **Add "Discovery Readout" presentation structure.** Client-facing presentation: how to structure it, how to handle findings the client won't want to hear, how to transition from findings to recommendation.

#### MEDIUM Priority

5. **Add budget/resourcing guidance.** Team staffing, hours allocation, burn rate tracking. Engagement economics are a common source of failure.

6. **Strengthen discovery synthesis with analytical frameworks.** How to identify root causes vs. symptoms. How to triangulate across interviews. How to prioritize findings by impact.

7. **Add "Red Flags" diagnostic for discovery.** Signs the engagement is scoped wrong. Signs the real problem isn't what the client thinks. Signs the client isn't ready for recommendations.

8. **Add guidance for "when discovery is blocked."** Some clients resist access. Escalation, workarounds, what it signals.

9. **Add kickoff misalignment guidance.** "If the kickoff reveals fundamental disagreement on scope between sponsor and working team, stop and resolve. This is a blocker, not a risk."

10. **Expand working arrangements for remote/hybrid.** Plan 25% more time for remote kickoffs, breakout rooms, schedule informal 1:1s.

#### LOW Priority

11. **Consolidate resistance/alignment tables.** Merge resistance type diagnosis into a column on the current-vs-desired position table.

12. **Reduce external stakeholders table granularity.**

---

### Implementation Planning

**Eval scores:** WITH avg 9.0, WITHOUT avg 5.5, delta +3.5.

#### HIGH Priority

1. **Add "So What" synthesis section at end of business case.** Distill: (a) the single most important number, (b) the single biggest risk, (c) the one thing that must go right.

2. **Add confidence levels for financial projections.** Tag each line item: "high confidence, based on actual data" vs. "medium confidence, dependent on negotiation outcomes."

3. **Add change management hooks.** Subsection in Stage 4: "Change Management Touchpoints" listing where communication plans, training, stakeholder engagement plug into the implementation timeline. Cross-reference change-management skill.

4. **Add benefits realization tracking template.** Metric, Baseline, Target, Actual, Variance, Action Required.

#### MEDIUM Priority

5. **Add stakeholder impact/alignment section.** Who's affected, what they care about, current stance, desired stance, actions to move them.

6. **Add "Day 1 / Week 1 / Month 1" mobilization plan.** What happens in the first few days after recommendation is approved.

7. **Strengthen "Do Nothing" baseline analysis.** Same financial projection rigor as other options (3-5 year projected costs, competitive deterioration, opportunity cost).

8. **Add competitive/market context prompts for market entry scenarios.**

9. **Flesh out or fold the scenario testing section.** Add how to run sensitivity analysis, identify break-even thresholds, document which assumptions the recommendation is most sensitive to.

#### LOW Priority

10. **Shorten the description.** Current version is too long and reads like a feature list.

11. **Remove "Information That Flows Forward" table** (duplicates "Connecting the Stages" bullets).

12. **Cut or compress the Strategy-to-Execution ASCII diagram.**

---

### Change Management

**Eval scores:** WITH avg 9.0, WITHOUT avg 6.25, delta +2.75. Review score: 7.5/10.

#### HIGH Priority

1. **Add worked example.** Individual Adoption Model applied to a specific scenario (e.g., ERP rollout), even 10 lines.

2. **Explain how Individual Adoption Model and Transformation Execution Framework connect.** Simple mapping: "Phase 1 Mobilize primarily addresses Understanding and Motivation stages."

3. **Add change team sizing guidance.** Ratio of champions to affected population (1:30-50), typical budget allocation as % of project cost, 1 change manager per 500-1,000 affected employees.

4. **Add change saturation assessment.** Referenced in measurement section but never explained.

#### MEDIUM Priority

5. **Add "failed prior attempt" / "second attempt" module.** Trust rebuilding, explicit failure acknowledgment, earned credibility rather than assumed.

6. **Add change readiness assessment tool.** Structured pre-assessment survey or scorecard for each stakeholder group.

7. **Add digital transformation specifics.** Common resistance patterns for cloud tools, data migration anxiety.

#### LOW Priority

8. **Trim "Choosing the Right Approach" table.** "Supporting Elements" column is vague.

---

### Due Diligence

**Eval scores:** WITH avg 9.25, WITHOUT avg 7.0, delta +2.25. Review score: 9.5/10 (highest overall quality).

#### HIGH Priority

1. **Add industry-specific overlays.** Sector-specific DD considerations even if brief. EdTech: FERPA/COPPA, stimulus dependency. Healthcare: HIPAA, reimbursement. Manufacturing: environmental, union.

2. **Add unit economics framework.** CAC, LTV, LTV:CAC, payback period, gross margin analysis for SaaS DD.

3. **Add management interview guide.** 5-10 key questions per DD type, triangulation techniques, red flags in management responses.

4. **Add cohort analysis framework.** For SaaS businesses, vintage/cohort analysis is the single most revealing analysis.

5. **Add "minimum viable DD" information request list.** For time-constrained situations (PE secondary, small bolt-on acquisitions).

#### MEDIUM Priority

6. **Add exit scenario modeling guidance for PE deals.** Bull/base/bear exit scenarios with IRR estimates.

7. **Add "100-day plan" template for PE context.** Referenced but not structured.

8. **Strengthen management assessment criteria.** Track record scoring, domain expertise evaluation, PE readiness assessment.

9. **Bridge to valuation.** How DD findings translate to valuation methodology selection and multiple adjustments.

10. **Add data room review workflow.** How to prioritize 500+ documents, what to cross-reference, how to flag discrepancies.

#### LOW Priority

11. **Remove inconsistent horizontal rules between sections.**

---

### Executive Presentation

**Eval scores:** WITH avg 9.0, WITHOUT avg 3.5, delta +5.5.

#### HIGH Priority

1. **Add sensitivity analysis formatting guidance.** Tornado charts, scenario tables.

2. **Add "leave-behind vs. presentation" distinction.** Different density guidelines for read-ahead documents vs. spoken presentations.

3. **Add board-specific dynamics section.** Fiduciary duty framing, governance committee expectations.

#### MEDIUM Priority

4. **Add worked example of a completed slide outline.**

---

### Workshop Facilitation

**Eval scores:** WITH avg 9.75, WITHOUT avg 3.25, delta +6.5 (largest delta of any skill).

#### HIGH Priority

1. **Add strategy offsite-specific template.** Multi-day format with more explicit decision-making architecture.

2. **Add guidance on managing the CEO's role.** When they should and shouldn't speak. HiPPO management.

#### MEDIUM Priority

3. **Add hybrid/remote workshop guidance.** Managing 1-2 remote participants in an otherwise in-person offsite.

4. **Add worked example of a completed workshop design.**

---

### Process Excellence

**Eval scores:** WITH avg 9.75, WITHOUT avg 4.5, delta +5.25. Review score: 9/10.

#### HIGH Priority

1. **Add industry-specific benchmarks as reference tables.** Common processes: O2C, P2P, R2R with industry benchmark ranges.

2. **Add Lean vs. Six Sigma decision guide.** "Lean focus (waste/flow problems) vs. Six Sigma focus (variation/defect problems) vs. combined."

3. **Add process mining extraction guidance.** How to scope and execute process mining analysis for O2C-specific ERP extraction.

#### MEDIUM Priority

4. **Add sigma level calculation walkthrough.** Referenced but not demonstrated.

5. **Add project charter fill-in template.**

6. **Add text-based value stream map example.** Anchor the VSM section with a concrete representation.

7. **Flesh out Theory of Constraints / bottleneck analysis.** Takt time is mentioned but not fully developed.

#### LOW Priority

8. **Fold SIPOC into Measure phase** rather than standing alone.

---

### Project Governance

**Eval scores:** WITH avg 9.0, WITHOUT avg 5.25, delta +3.75. Review score: 8.5/10.

#### HIGH Priority

1. **Add stakeholder mapping section.** Power/interest grid, particularly for large multi-geography engagements.

2. **Add communication plan template.** Beyond meeting cadence: who gets what message, via what channel, at what frequency.

3. **Add cross-workstream dependency management.** Dependency matrix, integration points, shared resources, interface agreements.

4. **Expand Hybrid Delivery Framework.** How sprint reviews feed into stage gates, how to aggregate agile metrics into waterfall-style status reports.

#### MEDIUM Priority

5. **Add benefits realization tracking framework.** Not just "benefits tracking in place" at closure, but ongoing measurement.

6. **Add brief self-contained closure guidance.** Don't fully punt to project-closeout skill; include enough to be useful standalone.

7. **Define abbreviations on first use** (EM, PMO).

#### LOW Priority

8. **Compress Working Sessions entry in meeting cadence** (doesn't add much beyond "meet as needed").

---

### Org Design

**Eval scores:** WITH avg 9.5, WITHOUT avg 6.5, delta +3.0.

#### HIGH Priority

1. **Add change management / cultural transformation section.** Product-to-customer is cultural, not just structural. Add cultural assessment framework.

2. **Add compensation and incentive redesign guidance.** Moving from product P&Ls to segment P&Ls requires realigning incentive structures. Make-or-break issue.

3. **Add customer segmentation methodology.** The skill assumes segments are defined; in practice, defining segments is a critical design input.

#### MEDIUM Priority

4. **Add systems and process redesign section.** CRM migration, reporting realignment, P&L accounting changes that make or break structural shifts.

---

### Pricing Strategy

**Eval scores:** WITH avg 10.0, WITHOUT avg 5.75, delta +4.25 (highest avg WITH score).

#### HIGH Priority

1. **Add actual rate benchmarks or ranges.** Even broad ranges ("$8,000-15,000/day for partners at top-tier firms") would ground the output.

2. **Add procurement negotiation tactics.** RFP scoring, competitive bidding, preferred vendor panels, rate benchmarking.

3. **Add phased engagement economics.** How to price land-and-expand (Phase 1 diagnostic with contingent Phase 2 design) vs. full commitment upfront.

#### MEDIUM Priority

4. **Add proposal structure section.** How to present pricing within a proposal document (executive summary of value, options table, appendix with rate card).

---

### Thought Leadership

**Eval scores:** WITH avg 9.0, WITHOUT avg 5.0, delta +4.0.

#### HIGH Priority

1. **Add word count targets per section within each asset type.** PoV structure is given but without proportional guidance.

2. **Add examples of strong vs. weak thesis statements** specific to each asset type.

3. **Add "hooks" library.** Opening techniques beyond "lead with insight."

---

### Project Closeout

**Eval scores:** WITH avg 9.5, WITHOUT avg 5.0, delta +4.5.

#### HIGH Priority

1. **Add closeout effort estimation guidance.** What percentage of total engagement cost should be allocated for different program sizes.

2. **Add RACI matrix template for closeout activities.**

3. **Add regulated-industry guidance.** Financial services, healthcare, government have specific compliance requirements affecting closeout process.

#### MEDIUM Priority

4. **Add stakeholder communication plan template.** Who gets told what, when, and by whom during closeout.

---

### Report Generation

**Eval scores:** WITH avg 9.5, WITHOUT avg 5.25, delta +4.25.

#### HIGH Priority

1. **Add scenario analysis guidance.** What if the first market underperforms? Trigger points for accelerating or decelerating.

2. **Add sensitivity analysis for financial projections.**

3. **Add executive presentation template.** 10-slide version of the report for board presentations.

4. **Add guidance on handling data gaps.** The "[X]" placeholder pattern for draft vs. final versions.

---

## Summary: Top 10 Improvements by Impact

| # | Improvement | Skills Affected | Effort |
|---|---|---|---|
| 1 | Add worked examples to every skill | All 17 | High |
| 2 | Add "So What?" synthesis discipline | 6+ skills | Medium |
| 3 | Add output depth calibration | 5+ skills | Low |
| 4 | Add data confidence markers | 5+ skills | Low |
| 5 | Add Day 1 Hypothesis to problem-solving | 1 skill (flagship) | Low |
| 6 | Add SaaS metrics to financial-modeling and due-diligence | 2 skills | Low |
| 7 | Add pricing strategy to proposal-development | 1 skill | Medium |
| 8 | Add cross-skill references | All 17 | Low |
| 9 | Trim human-only content | 3 skills | Low |
| 10 | Add industry-specific overlays | 5+ skills | Medium |

---

## Eval Score Summary

| Skill | WITH Avg | WITHOUT Avg | Delta | Strongest Dimension |
|---|---|---|---|---|
| workshop-facilitation | 9.75 | 3.25 | **+6.5** | All dimensions |
| executive-presentation | 9.0 | 3.5 | **+5.5** | All dimensions |
| process-excellence | 9.75 | 4.5 | **+5.25** | Consulting-grade |
| project-closeout | 9.5 | 5.0 | **+4.5** | Consulting-grade, Depth |
| pricing-strategy | 10.0 | 5.75 | **+4.25** | Depth |
| report-generation | 9.5 | 5.25 | **+4.25** | Consulting-grade |
| thought-leadership | 9.0 | 5.0 | **+4.0** | Consulting-grade |
| financial-modeling | 9.25 | 5.25 | **+4.0** | Structure |
| project-governance | 9.0 | 5.25 | **+3.75** | Actionability, Depth |
| engagement-setup | 8.75 | 5.0 | **+3.75** | Consulting-grade |
| implementation-planning | 9.0 | 5.5 | **+3.5** | Actionability |
| strategic-frameworks | 8.7 | 5.3 | **+3.4** | Consulting-grade |
| proposal-development | 9.0 | 5.75 | **+3.25** | Structure |
| org-design | 9.5 | 6.5 | **+3.0** | Depth |
| problem-solving | 8.75 | 6.0 | **+2.75** | Consulting-grade |
| change-management | 9.0 | 6.25 | **+2.75** | All dimensions |
| due-diligence | 9.25 | 7.0 | **+2.25** | Structure |

Average delta across all skills: **+3.75 points** on a 10-point scale.

Key finding: The biggest consistent gap is "consulting-grade" quality. The skills' primary value is making outputs look and feel like actual consulting work product rather than smart-but-informal analysis. The smallest gap is "depth," suggesting the skills guide format and process better than analytical thinking.

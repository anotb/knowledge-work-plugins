---
name: problem-solving
description: Apply hypothesis-driven, MECE problem solving methodology. Use when structuring complex problems, building issue trees, developing testable hypotheses, designing analytical workplans, decomposing problems into mutually exclusive collectively exhaustive components, performing root cause analysis, or running diagnostics. Covers the full consulting problem-solving arc from problem definition through structured decomposition, prioritization, hypothesis development, analysis, synthesis, and actionable recommendations.
---

# Problem Solving

Apply hypothesis-driven methodology to structure complex problems, develop testable hypotheses, and guide systematic analysis to reach actionable recommendations.

Two modes of operation:
- **Structuring mode** (no data provided): Build the issue tree, form hypotheses, design the analytical workplan, and specify what data would prove or disprove each hypothesis. The output is a roadmap for the analysis.
- **Analysis mode** (data provided): Run the analysis, test hypotheses against the data, synthesize findings, and deliver recommendations. The output is answers.

Default to structuring mode unless the user provides data to analyze.

---

## The Consulting Problem-Solving Process

### Step 1: Define the Problem

Before any analysis, rigorously define the problem. Get outcome clarity and constraints upfront.

A good problem definition covers:

- **The Question**: What exactly are we trying to solve? State in one sentence.
- **The Context**: Industry dynamics, company position, timeframe, technology landscape.
- **Quantification**: Size the problem. What is the financial impact of the status quo? What is the value of solving it? Anchor all subsequent prioritization to these numbers. If exact figures aren't available, estimate the order of magnitude.
- **Success Criteria**: What does a successful solution look like? How will we measure it? What are the constraints? What is the decision timeline?
- **Out of Scope**: What are we NOT solving for? What boundaries exist?

**Validate the premise before proceeding:**

- Is the data behind this problem statement reliable? How was it measured?
- Is the comparison fair? (Apples-to-apples scope, same definitions, same time periods)
- Is the stated problem actually a problem, or is it a solution looking for justification?
- Are we solving symptoms or root causes?
- What would happen if we did nothing?

### Step 2: Structure the Problem

Apply MECE decomposition (Mutually Exclusive, Collectively Exhaustive) to break the problem into non-overlapping, complete branches.

**Issue tree templates by problem type:**

| Problem Type | Recommended Structure |
|---|---|
| Profitability decline | Revenue (price x volume) + Cost structure |
| Market entry | Market size x Achievable share + Entry requirements |
| Operational inefficiency | Throughput x Yield + Cycle time |
| Customer churn | Acquisition x Retention x Lifetime value |
| Growth strategy | Core business + Adjacent opportunities + Transformational bets |
| Digital transformation | Current state + Capability gaps + Technology options |
| Cost reduction | MECE cost waterfall by value chain stage + overhead |
| Build vs. buy | Strategic fit + Economics (TCO) + Execution risk |
| Pricing strategy | Value to customer + Cost to serve + Competitive positioning |
| Org effectiveness | Structure + Processes + People + Technology |
| M&A evaluation | Strategic rationale + Valuation + Integration feasibility |

**MECE in practice:**

NOT MECE (overlapping):
- North America, Europe, Emerging markets, Developed markets

MECE:
- North America, Europe, Asia-Pacific, Latin America, Middle East & Africa

NOT MECE (inconsistent categories):
- Product revenue, Service revenue, License revenue, Software

MECE:
- Product revenue, Service revenue, License revenue, Other revenue

For digital businesses, consider alternative MECE cuts:
- Recurring revenue (subscriptions, SaaS), Transaction revenue (usage-based, marketplace), Professional services, Ecosystem/partner revenue

### Step 3: Prioritize Issues

Not all branches deserve equal attention. Rank branches by estimated impact and data availability.

Use a 2x2 prioritization:

|  | High Data Availability | Low Data Availability |
|---|---|---|
| **High Expected Impact** | Analyze first | Design data collection, analyze in parallel |
| **Low Expected Impact** | Quick scan, move on | Deprioritize |

Decision criteria:
- Where is the biggest lever? (Quantify: "This branch represents ~$Xm of the gap")
- Where is the data available?
- What can we test quickly with minimum viable analysis?
- What is the time sensitivity?

### Step 4: Develop Hypotheses

Form testable hypotheses early. This focuses analysis and prevents boiling-the-ocean data collection.

#### Day 1 Answer

Before any analysis, state your best guess at the final answer based on available information. This is not a commitment. It is a focusing device.

The Day 1 answer should be:
- A complete sentence answering the original question
- Your current confidence level (low/medium/high)
- The 1-2 analyses that would most change your mind

This forces intellectual honesty. If you can't form even a tentative answer, you don't understand the problem well enough.

#### Hypothesis Development

A good hypothesis:
- Is specific and concrete
- Is testable with available data
- Implies a recommended action if proven true
- States "we believe X because Y"
- Has a quick validation path

For each hypothesis, define:
- **Current belief**: What we think is true
- **Evidence needed**: What would prove or disprove it
- **Data source**: Where to find the evidence
- **Quick test**: Fastest way to validate or invalidate
- **If true, then**: What we'd recommend

### Step 5: Conduct Analysis

Structure analysis to test hypotheses, not to generate data for its own sake.

For each analysis workstream, define:
- Which hypothesis it tests
- The analytical method
- Data inputs required
- Expected output and what it tells us

Analytical approaches by situation:

| Situation | Recommended Analysis |
|---|---|
| Profit driver identification | Bridge analysis, variance analysis |
| Market sizing | Top-down, bottom-up, triangulated |
| Competitive assessment | Relative positioning, scenario analysis |
| Financial projections | Scenario modeling, sensitivity analysis |
| Process optimization | Root cause analysis, process mining, time studies |
| Customer insights | Segmentation, cohort analysis, journey mapping |
| Cost gap analysis | Cost bridge/waterfall decomposition |

For each analysis, document assumptions, check sensitivity (which inputs matter most), and actively seek disconfirming evidence.

### Step 6: Synthesize Findings

Synthesis is NOT summary. Summary says "we found X." Synthesis says "X means Y, which changes our recommendation to Z."

**Lead with the answer (Pyramid Principle):**

1. **The Answer** (1 sentence): Direct response to the original question
2. **Three supporting arguments**: The key reasons behind the answer, ordered by importance
3. **Evidence for each argument**: The specific data that proves each point

**Anti-patterns to avoid:**
- "We found many interesting things" (no hierarchy, no answer)
- Restating findings without interpretation
- Burying the answer at the end
- Presenting analysis in the order it was conducted rather than the order that supports the argument
- Confusing "thorough" with "useful" (every finding must connect to the answer)

**Test your synthesis:** Can someone read only the first paragraph and understand the answer and why? If not, restructure.

### Step 7: Develop Recommendations

Translate findings into action. Each recommendation needs:
- **Rationale**: Why this addresses the problem
- **Impact**: Expected outcome, quantified
- **Effort**: Resources required
- **Timing**: When to act (quick wins vs. structural changes)
- **Implementation approach**: How to execute
- **Risks**: What could go wrong and how to mitigate

---

## Issue Trees

### Hypothesis Tree

Use when you have competing theories about what's happening.

```
                    [Ultimate Question]

        ┌───────────────┼───────────────┐
        ▼               ▼               ▼
   [Hypothesis 1]  [Hypothesis 2]  [Hypothesis 3]
        │               │               │
   ┌────┴────┐     ┌────┴────┐     ┌────┴────┐
   ▼         ▼     ▼         ▼     ▼         ▼
  [Proof 1] [Proof 2] [Proof 1] [Proof 2] [Proof 1] [Proof 2]
        │               │               │
   [Quick Test]    [Quick Test]    [Quick Test]
```

Start with the ultimate question. Branch into competing hypotheses. Under each hypothesis, identify the proof points needed and the quickest way to test them.

### Logic Tree

Use when you need to decompose a problem into its component drivers (cause and effect, not competing theories).

```
                 [Problem Statement]

        ┌───────────────┼───────────────┐
        ▼               ▼               ▼
   [Driver A]    [Driver B]     [Driver C]
        │               │
   ┌────┴────┐     ┌────┴────┐
   ▼         ▼     ▼         ▼
 [Factor 1] [Factor 2] [Factor 3] [Factor 4]
        │               │
   [Root Cause]    [Root Cause]
```

Decompose the problem into its causal drivers. Keep branching until you reach actionable root causes.

---

## Common Pitfalls

| Pitfall | Why It's Problematic | Solution |
|---|---|---|
| Defining the problem too broadly | Diffuses analysis, no clear success criteria | Narrow scope iteratively, quantify the problem |
| Skipping the Day 1 answer | Analysis drifts without a point of view | Force a tentative answer before analysis begins |
| Jumping to solutions | Misses root causes | Follow the process: define, structure, hypothesize, then solve |
| Collecting all data | Wastes time on low-value analysis | Prioritize by hypothesis, apply 80/20 |
| Confirming existing beliefs | Biases analysis | Actively seek disconfirming evidence |
| Summarizing instead of synthesizing | No actionable insight | Lead with the answer, then support it |
| Presenting findings without recommendations | Leaves client without action | Always translate findings to actions |

---

## Worked Example

**Prompt**: "Our SaaS company's enterprise churn rate jumped from 8% to 14% last quarter. Help me structure an analysis to understand why."

**Step 1: Define the Problem**

- **Question**: Why did enterprise churn increase from 8% to 14% last quarter, and what can we do to reverse it?
- **Quantification**: A 6-point jump in one quarter is acute (not gradual drift), suggesting a triggering event. At 14% annualized, if average enterprise ACV is $200K and we have 300 enterprise accounts, we're losing ~$8.4M ARR/year vs. ~$4.8M at baseline. The incremental exposure is ~$3.6M ARR.
- **Premise check**: Is 14% calculated consistently with the prior 8%? Same denominator (beginning-of-period accounts)? Same definition of "churn" (logo vs. revenue, gross vs. net)?
- **Success criteria**: Identify the 2-3 root drivers, quantify their contribution, and develop interventions to return churn to <10% within 2 quarters.
- **Out of scope**: SMB/mid-market churn, new logo acquisition, pricing overhaul (unless directly implicated).

**Step 2: Structure (MECE)**

Three branches (mutually exclusive, collectively exhaustive... every churn event is driven by one of these):

1. **We caused it** (Product/service failures): Feature regressions, support quality decline, CSM turnover
2. **Competitors caused it** (Market shift): New entrant, price undercut, feature parity shift
3. **Customer circumstances changed** (External): Budget cuts, M&A, leadership turnover

**Step 3: Prioritize**

| Branch | Expected Impact | Data Availability | Priority |
|---|---|---|---|
| Product/Service | HIGH (most common SaaS churn driver) | HIGH (usage data, tickets, NPS) | Analyze first |
| Competitive | MEDIUM | MEDIUM (win/loss, exit surveys) | Parallel track |
| Customer-side | MEDIUM | LOW (requires outreach) | Quick scan of top 10 churned accounts |

**Step 4: Day 1 Answer & Hypotheses**

Day 1 answer: "Enterprise churn spiked because a Q3 product release degraded the enterprise experience, compounded by CSM turnover that left accounts without a relationship anchor during the disruption." Confidence: Medium. The analysis that would most change my mind: usage data overlay with churn timing.

H1: A product release degraded the enterprise experience.
- Quick test: Overlay churn dates with release dates. Compare support ticket volume in churned vs. retained accounts.

H2: A competitor made a significant move.
- Quick test: Pull exit survey verbatims, count competitor mentions.

H3: CSM changes left accounts unanchored.
- Quick test: Compare churn rate for accounts with CSM reassignment vs. stable CSM coverage.

H4: Enterprise customers are cutting vendor spend due to macro pressure.
- Quick test: Check top 10 churned accounts for public signals (layoffs, earnings warnings).

**Step 5: Analytical Workplan**

| Workstream | Tests | Method | Timeline |
|---|---|---|---|
| Churn cohort analysis | H1-H4 | Segment churned accounts by tenure, size, industry, usage | Week 1 |
| Product usage analysis | H1 | Usage metrics (DAU, feature adoption) in churned vs. retained, 90 days pre-churn | Week 1 |
| Exit interview coding | H1, H2 | Code exit survey verbatims, 5-8 win-back interviews | Week 1-2 |
| CSM coverage analysis | H3 | Churn rate by CSM tenure, reassignment events | Week 1 |
| External signal scan | H4 | Cross-reference churned accounts with public filings, layoff news | Week 1 |

**Step 6: Synthesis (structure, not yet populated)**

"Enterprise churn spiked from 8% to 14% because [root cause], accounting for [X%] of the incremental churn. [Secondary driver] contributed [Y%]. We recommend [top 3 actions] to return churn to <10% by [quarter]."

Three supporting arguments would follow, each backed by specific data from the workstreams above.

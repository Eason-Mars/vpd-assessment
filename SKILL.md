---
name: vpd-assessment
description: Use when diagnosing a project's value proposition quality and business model strength using the Strategyzer VPD framework. Triggers: "does this product have a market?", "do customers really need this?", consulting project DD/feasibility, new project VP-market fit risk assessment.
---
# vpd-assessment — Value Proposition Diagnosis Framework
Version: 1.1.0
Authors: Eason Zhang, Mars
Based on: Strategyzer Value Proposition Design (Osterwalder, Pigneur, Bernarda, Smith)
Modes: deep | medium | quick

## What This Skill Does
Diagnoses a project's value proposition quality and business model strength using the Strategyzer VPD framework. Output: structured diagnosis report with fit assessment, BM quality scores, and next-step experiment recommendations.

This is NOT about filling in a canvas. This is about answering:
- Does this product solve a real, important customer problem?
- Is the value proposition addressing the right jobs/pains/gains?
- Is the business model strong enough to sustain the VP?
- What assumptions need to be tested first?

## When to Use
- Exploration 🌌: Consulting project DD / feasibility — diagnose whether client's VP is sound
  - deep: full DD for serious consulting engagements
  - medium: initial project evaluation, pre-proposal diagnosis
- Spirit 🌟: New project evaluation — quick VP-Market Fit risk assessment (use quick mode)
- Mars 🔴: Advisory group Q&A — 3-min directional diagnosis (use quick mode)
- Any time someone asks: "Does this product have a market?" / "Do customers really need this?"

## How It Differs from YC / Superpowers Frameworks
- YC: Investor lens — is this worth betting on?
- Superpowers: Competitive strategy — what are your moats?
- VPD Assessment: Product-customer research lens — are you solving the RIGHT problem for the RIGHT customer?
- Unique value: Mechanism-level diagnosis + built-in "what to test next" action plan
- Use order: VPD Assessment → Superpowers → YC (VPD is the foundation layer)

## Two Modes

### deep mode (Exploration — full 5-step, consulting DD)
Estimated time: 90-120 min analysis

**Step 1: Customer Profile Scan**
Read: `{SKILL_DIR}/references/customer-jobs-trigger-questions.md`
Read: `{SKILL_DIR}/references/customer-pains-trigger-questions.md`
Read: `{SKILL_DIR}/references/customer-gains-trigger-questions.md`
- Use trigger questions to surface Functional / Social / Emotional jobs
- Enumerate Pains (9 trigger questions) and Gains (9 trigger questions)
- Rank by importance — identify Top 3 most unmet needs
- Distinguish: verified facts vs. assumptions

**Step 2: Value Map Analysis**
Read: `{SKILL_DIR}/references/pain-relievers-trigger-questions.md`
Read: `{SKILL_DIR}/references/gain-creators-trigger-questions.md`
- List all products & services
- Map each Pain Reliever → which Pains does it address?
- Map each Gain Creator → which Gains does it create?
- Coverage analysis: Are Top Pains and Gains covered? What's missing?

**Step 3: Fit Diagnosis (3 levels)**
- Problem-Solution Fit: Is this Pain real or assumed? What evidence exists?
- Product-Market Fit: Is the product addressing Pain #1 or Pain #4?
- Business Model Fit: Can the VP be sustained by the underlying BM?

**Step 3b: Competitive VP Comparison**
List 2-3 main competitors. For each competitor, assess:
- Pain Coverage: which customer pains does their VP address?
- Gain Coverage: which gains does their VP deliver?
- Differentiation highlights: where do they stand out?

Output: comparison matrix (Our VP vs Competitor A vs Competitor B) with columns:
| Dimension | Our VP | Competitor A | Competitor B |
| Pain Coverage | ... | ... | ... |
| Gain Coverage | ... | ... | ... |
| Differentiation | ... | ... | ... |

Conclusion:
- Differentiation advantages: where our VP is clearly stronger
- Overlap risks: where our VP competes head-to-head with no differentiation

If competitive data is not provided: state "Insufficient data — recommend competitive research" and skip the matrix.

**Step 4: Business Model Quality Score (7 dimensions × 0-10)**
Read: `{SKILL_DIR}/references/7-questions-bm-quality.md`
Score each dimension 0-10, identify weakest dimension, provide specific improvement recommendation.

**Step 5: Next Steps**
Read: `{SKILL_DIR}/references/six-ways-to-innovate.md`
- Recommend 1-2 innovation directions
- Identify most critical + most uncertain assumption
- Design 1-2 Test Cards (Hypothesis → Test method → Success criterion)

Output format: HTML report (Eason Consulting brand: primary #8B3A2A, accent #C5963A, warm white background)
Output template: `{SKILL_DIR}/assets/output-template-deep.md`
QC standard: `{SKILL_DIR}/references/10-characteristics-vp-checklist.md` (all 10 must be addressed)

---

### medium mode (Exploration — Steps 1-3 + BM Score, initial project evaluation)
Estimated time: 45-60 min analysis
Use when: initial project evaluation, pre-proposal consulting diagnosis

**Step 1: Customer Profile Scan**
Read: `{SKILL_DIR}/references/customer-jobs-trigger-questions.md`
Read: `{SKILL_DIR}/references/customer-pains-trigger-questions.md`
Read: `{SKILL_DIR}/references/customer-gains-trigger-questions.md`
- Use trigger questions to surface Functional / Social / Emotional jobs
- Enumerate Pains (9 trigger questions) and Gains (9 trigger questions)
- Rank by importance — identify Top 3 most unmet needs
- Distinguish: verified facts vs. assumptions

**Step 2: Value Map Analysis**
Read: `{SKILL_DIR}/references/pain-relievers-trigger-questions.md`
Read: `{SKILL_DIR}/references/gain-creators-trigger-questions.md`
- List all products & services
- Map each Pain Reliever → which Pains does it address?
- Map each Gain Creator → which Gains does it create?
- Coverage analysis: Are Top Pains and Gains covered? What's missing?

**Step 3: Fit Diagnosis (3 levels)**
- Problem-Solution Fit: Is this Pain real or assumed? What evidence exists?
- Product-Market Fit: Is the product addressing Pain #1 or Pain #4?
- Business Model Fit: Can the VP be sustained by the underlying BM?

**Step 3b: Competitive VP Comparison**
List 2-3 main competitors. For each competitor, assess:
- Pain Coverage: which customer pains does their VP address?
- Gain Coverage: which gains does their VP deliver?
- Differentiation highlights: where do they stand out?

Output: comparison matrix (Our VP vs Competitor A vs Competitor B) with columns:
| Dimension | Our VP | Competitor A | Competitor B |
| Pain Coverage | ... | ... | ... |
| Gain Coverage | ... | ... | ... |
| Differentiation | ... | ... | ... |

Conclusion:
- Differentiation advantages: where our VP is clearly stronger
- Overlap risks: where our VP competes head-to-head with no differentiation

If competitive data is not provided: state "Insufficient data — recommend competitive research" and skip the matrix.

**Step 4: Business Model Quality Score (7 dimensions × 0-10)**
Read: `{SKILL_DIR}/references/7-questions-bm-quality.md`
Score each dimension 0-10, identify weakest dimension, provide specific improvement recommendation.

_(Step 5 Next Steps is NOT included in medium mode — use deep mode for full innovation direction analysis)_

Output format: Markdown report (max 500 words), including BM Score table
Output template: `{SKILL_DIR}/assets/output-template-quick.md` (adapt for medium: expand to 500 words, include BM Score table)

---

### quick mode (Spirit — Steps 1-3 + conclusion, ~30 min)

**Step 1: Customer Profile (compressed)**
- Top 3 Jobs / Top 3 Pains / Top 3 Gains only
- Source: same trigger questions, but stop at Top 3 per category

**Step 2: Value Map (coarse)**
- Coverage rating: High / Medium / Low for Pain Relief and Gain Creation

**Step 3: Fit Diagnosis**
- Problem-Solution Fit: 🟢 Green / 🟡 Yellow / 🔴 Red + one-line reason
- Product-Market Fit: 🟢 / 🟡 / 🔴 + one-line reason
- Business Model Fit: 🟢 / 🟡 / 🔴 + one-line reason

Output:
- 1 paragraph core finding (max 100 words)
- Top 3 risks
- 1 priority assumption to test

Output format:
- Default: Markdown (max 300 words)
- If requested for client delivery: HTML (Eason Consulting brand: primary #8B3A2A, accent #C5963A)

Output template: `{SKILL_DIR}/assets/output-template-quick.md`

## Quality Standards
- All diagnosis conclusions must be grounded in provided information — no fabrication
- Fit conclusions MUST distinguish between "verified facts" and "unverified assumptions"
- 10 Characteristics checklist is mandatory QC for deep mode
- If information is insufficient to assess a dimension, state it explicitly as "Insufficient data"

## References Index
- `references/customer-jobs-trigger-questions.md` — 9 trigger questions for customer jobs
- `references/customer-pains-trigger-questions.md` — 9 trigger questions for customer pains
- `references/customer-gains-trigger-questions.md` — 9 trigger questions for customer gains
- `references/pain-relievers-trigger-questions.md` — 9 trigger questions for pain relievers
- `references/gain-creators-trigger-questions.md` — 9 trigger questions for gain creators
- `references/7-questions-bm-quality.md` — 7-dimension BM quality scoring framework
- `references/10-characteristics-vp-checklist.md` — 10 characteristics of great VPs
- `references/six-ways-to-innovate.md` — 6 innovation directions from customer profile

## Assets Index
- `assets/output-template-deep.md` — deep mode report structure (HTML, full 5-step)
- `assets/output-template-quick.md` — quick mode report structure (Markdown, also baseline for medium mode)
- medium mode: uses `assets/output-template-quick.md` as baseline, expanded to 500 words with BM Score table

## Skill Connections
- **Prerequisite**: None (VPD is the foundation layer)
- **After VPD deep**: → `company-financial-analysis` (complete DD = VP diagnosis + financial analysis)
- **After VPD quick/medium**: → `consulting-report` (package findings into client-ready report)
- **Parallel**: `venture-dd` (investor perspective complements VPD's product-customer lens)
- **Use order**: VPD Assessment → Superpowers → YC (foundation → strategy → investment)

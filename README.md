# Enterprise AI Consulting Skills

Ten Claude skills that replicate the analytical work Tier-1 consulting firms charge $1.5M to $2M to deliver during an enterprise AI initiative.

Each skill takes the discovery artifacts an enterprise already has (org charts, SOPs, schemas, audit findings, financial baselines, vendor pricing) and produces the kind of analysis a senior consultant would put in front of a steering committee. The output is specific to the documents you provide. Generic AI strategy advice is the failure mode these skills are designed to avoid.

## What's in here

| # | Skill | What it does | Big-4 equivalent |
|---|---|---|---|
| 1 | ai-readiness-assessment | Ruthless gap analysis across data, security, and org structure | $75k to $150k |
| 2 | workflow-acceleration-analysis | SOP vs. reality comparison with automation candidate scoring | $150k to $250k |
| 3 | ai-use-case-prioritization | 4-bucket framework that kills distractions and funds Lighthouse Pilots | $200k to $300k |
| 4 | build-vs-buy-framework | 3-year TCO comparison with a hard recommendation | $100k to $200k |
| 5 | ai-payback-business-case | Single conservative scenario, 30% Change Management Tax, payback in months | $150k to $250k |
| 6 | target-operating-model-design | Role evolution, handoff map, and human-in-the-loop protocol | $150k |
| 7 | data-readiness-and-gap-analysis | Schema-level audit ending in 3 prioritized engineering tasks | $200k |
| 8 | ai-threat-modeling-and-risk-assessment | Threat vectors, compliance exposure, and required guardrails | $175k |
| 9 | ai-business-case-and-roi-model | Full NPV, IRR, three scenarios, and CFO objection handling | $100k |
| 10 | ai-pilot-implementation-roadmap | Sprint Zero plus a 12-week pilot plan with critical path dependencies | $150k |

## Skill details

### 1. ai-readiness-assessment

**Goal:** Tell you whether your organization can deploy AI today, or what foundational work has to happen first.

**Inputs:**
- Current organizational chart
- Technical architecture documentation
- Recent IT audit summaries
- Data strategy overview

**Outputs:** Data infrastructure reality check, security and governance red flags, organizational silos, and 3 foundational fixes with owner and timeline.

### 2. workflow-acceleration-analysis

**Goal:** Compare official SOPs against how the work actually happens, surface shadow IT, and identify the highest-ROI automation candidates.

**Inputs:**
- Official Standard Operating Procedures (numbered or sectioned)
- Raw transcripts of frontline employees describing the real workflow

**Outputs:** The delta grouped by SOP section, named shadow IT instances with risks, top 5 time-wasters ranked by weekly FTE hours, and 5-8 automation candidates scored 1-10 on feasibility.

### 3. ai-use-case-prioritization

**Goal:** Sort a backlog of candidate AI use cases into what to fund, delay, and kill, with the top Lighthouse Pilots justified by business metrics.

**Inputs:**
- Raw list of potential AI use cases
- Bottleneck analyses or workflow assessments
- Top strategic goals for the year (OKRs, board priorities, or named initiatives)

**Outputs:** The Sandbox, the Distractions, the Incremental Wins, and 2-4 Lighthouse Pilots with metric-backed justification.

### 4. build-vs-buy-framework

**Goal:** A hard recommendation on building, buying, or running a hybrid for a specific AI pilot.

**Inputs:**
- The chosen Lighthouse Pilot
- Internal engineering capacity
- Feature and pricing data for off-the-shelf vendor solutions

**Outputs:** Commodity vs IP-defensible component split, 3-year TCO for both paths, and a hard recommendation in the first sentence of the final section.

### 5. ai-payback-business-case

**Goal:** A single conservative payback story designed to clear budget review without a fight.

**Inputs:**
- Baseline costs of the current manual workflow
- Estimated costs and time savings of the AI-automated replacement

**Outputs:** Single conservative scenario with soft savings excluded from the math, a 30% Change Management Tax applied to budget and timeline, and the top 3 aggressive CFO challenges with data-backed answers.

### 6. target-operating-model-design

**Goal:** Specify exactly how the org changes when an AI agent ships into a workflow.

**Inputs:**
- Current state workflow
- Existing roles involved in that workflow
- The specific AI agents being introduced

**Outputs:** Role evolution from execution to validation, net-new roles required, an AI-to-human and human-to-AI handoff map, and a human-in-the-loop escalation protocol for edge cases and failures.

### 7. data-readiness-and-gap-analysis

**Goal:** Audit the data estate against the AI workflow's real needs and surface what data engineering has to do before production.

**Inputs:**
- Current data estate documentation (schemas, API endpoints)
- Target workflow
- Data inputs required by the proposed AI agents

**Outputs:** Missing data the AI cannot access, structure deficits where unstructured data must be made machine-readable, latency risks that break real-time processing, and the top 3 data engineering tasks required before production.

### 8. ai-threat-modeling-and-risk-assessment

**Goal:** Surface the security, compliance, and hallucination risks of a specific AI workflow plus the controls needed before deployment.

**Inputs:**
- Proposed AI workflow
- System architecture
- Data types processed

**Outputs:** LLM and agent threat vectors, compliance exposure across GDPR, CCPA, and industry regulations, hallucination blast radius for silent failure at the highest-risk step, and the required guardrails, access controls, and logging mechanisms.

### 9. ai-business-case-and-roi-model

**Goal:** Full financial model with scenarios and CFO objection handling for capital expenditure review.

**Inputs:**
- Current baseline costs of the manual workflow
- Estimated costs and time savings of the AI-automated replacement

**Outputs:** NPV, IRR, and payback period in months; Conservative, Base, and Aggressive scenarios; hard vs soft ROI separated explicitly; and the top 3 skeptical CFO objections with specific responses.

### 10. ai-pilot-implementation-roadmap

**Goal:** Put the chosen pilot on a calendar with sprint-level deliverables, dependencies, and resource allocation.

**Inputs:**
- Target workflow
- Data gaps (output of skill 7)
- Risk controls (output of skill 8)
- Operating model changes (output of skill 6)

**Outputs:** Sprint Zero prerequisites for the 2 weeks before any code, a 12-week pilot plan in 6 two-week sprints with deliverables and success criteria, critical path dependencies that will block the project if delayed, and resource allocation per sprint.

## How to use

Each skill is a `.skill` file. Install it once in Claude and it triggers automatically when you ask for that type of analysis. You provide the input documents; the skill produces the report.

The skills are designed to chain. The output of one is often the input to the next. Run them in sequence for a full enterprise AI initiative, or use any of them standalone.

Recommended sequence for a full engagement:

1. Readiness Assessment tells you if you can deploy AI at all
2. Workflow Analysis finds the bottlenecks worth attacking
3. Prioritization picks the Lighthouse Pilots
4. Build vs. Buy, Operating Model, Threat Modeling, and Data Readiness inform the architecture decision
5. The two financial cases serve different rooms (payback case for budget approval; full ROI model for capital expenditure review)
6. Implementation Roadmap puts the plan on a calendar

## What these skills won't do

These are decision-support tools, not decision-makers. A skill can model risk. It can't absorb legal liability or be fired.

## Output conventions

All 10 skills share the same writing rules: active voice, short paragraphs, no filler vocabulary, sentence-case headers, digits for numbers, and ruthless specificity to the documents provided. The skills won't pad analysis with generic advice, won't soften findings to spare feelings, and won't pretend hard problems are easy.

Output defaults to inline markdown. Each skill can produce a saved `.md` artifact for executive review. The financial skills (5 and 9) can produce `.xlsx` with editable assumptions. Any skill can produce `.docx` on request.

## Installation

1. Download the `.skill` files from this repo
2. In Claude, go to Settings → Capabilities → Skills
3. Upload each `.skill` file
4. Skills will trigger automatically on relevant prompts, or you can call them by name

## Repo structure

```
.
├── ai-readiness-assessment.skill
├── workflow-acceleration-analysis.skill
├── ai-use-case-prioritization.skill
├── build-vs-buy-framework.skill
├── ai-payback-business-case.skill
├── target-operating-model-design.skill
├── data-readiness-and-gap-analysis.skill
├── ai-threat-modeling-and-risk-assessment.skill
├── ai-business-case-and-roi-model.skill
├── ai-pilot-implementation-roadmap.skill
└── README.md
```

## License

MIT

## Credits

Built with Claude. Skill framework via Anthropic's skill-creator. Adapted from [The Craft of AI](https://www.thecraftofai.com/).

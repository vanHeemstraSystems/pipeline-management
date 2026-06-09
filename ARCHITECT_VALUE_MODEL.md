# Architect Value Model – PIPE Layer (Product Increment Planning & Execution)

> *“Before you make a decision, ask yourself first: does this fit my business model?”*
> This document connects quarterly tactical themes to sprint-level initiative decisions.

See parent: [`tactical-planning-management / ARCHITECT_VALUE_MODEL.md`](https://github.com/vanHeemstraSystems/tactical-planning-management/blob/main/ARCHITECT_VALUE_MODEL.md)

-----

## Purpose of This Document

At the PIPE layer (1 quarter / 6 sprints), the key question is:

> **“Which initiatives should I include in this product increment — and how do I ensure each one reflects architectural judgment, not just execution?”**

-----

## Initiative Intake Filter

Before accepting any initiative into a PIPE, score it on both the **Strategic Five Pillars** (from `task-management`) and the **Architect Practice lens** (from your Business Model).

### Part A — Strategic Five Pillars Score

```
Initiative: ________________________________

[ ] Core Pain Point    (0–5): How significant is the problem being solved?  ___
[ ] Underlying Need    (0–5): How essential is this need?                   ___
[ ] Stakeholder Impact (0–5): How many people benefit?                      ___
[ ] Context Clarity    (0–5): How well-defined is the scope?                ___
[ ] Outcome Value      (0–5): How measurable is the value delivered?        ___

STRATEGIC SCORE: ___ / 25

Threshold:
  20–25 → Strategic priority
  15–19 → Include in this PIPE
  10–14 → Backlog — revisit next quarter
   0–9  → Decline or reframe
```

### Part B — Architect Practice Lens

```
[ ] architect_value_type:
    ( ) judgment        — I am deciding/advising/reviewing trade-offs
    ( ) execution       — I am implementing
    ( ) knowledge-build — building my own expertise
    ( ) relationship    — strengthening a key connection
    ( ) admin           — necessary overhead
    ( ) misaligned      — should be declined

[ ] Am I being engaged as architect (judgment) or resource (execution)?
    If execution: what is the reframe path?  ______________________________

[ ] Will my input on this initiative actually be acted on?
    Yes / No / Uncertain — if uncertain: clarify before committing
```

**Combined decision:**

|Strategic Score|Architect Type            |Decision                      |
|---------------|--------------------------|------------------------------|
|≥15            |judgment / knowledge-build|✅ Include                     |
|≥15            |execution                 |⚠️ Include with reframe trigger|
|≥15            |misaligned                |❌ Decline                     |
|<15            |any                       |❌ Backlog or decline          |

-----

## Initiative Metadata (add to your PIPE records)

```yaml
initiative:
  title: ""
  pipe_quarter: ""                    # e.g. Q3-2026
  strategic_score: 0                  # 0–25 from Five Pillars
  architect_value_type: ""            # judgment | execution | knowledge-build | relationship | admin | misaligned
  value_drivers_served:
    - ""                              # risk-reduction | clarity | independent-judgment |
                                      # mistake-prevention | decision-acceleration | knowledge-transfer
  judgment_or_resource: ""            # judgment | resource
  reframe_trigger: ""                 # If resource: what triggers a reframe conversation?
  recommendation_uptake_expected: ""  # high | medium | low | unknown
  adr_required: true/false            # Does this initiative warrant an Architecture Decision Record?
```

-----

## PIPE Retrospective — Architect Practice Questions

At the end of each product increment, add these to your standard retrospective:

**Value delivered:**

- Which initiatives produced `judgment` work vs `execution` work?
- Were my architectural recommendations acted on? For which initiatives — and why not for others?
- Did any initiative produce an ADR or lasting architectural artifact?

**Practice health:**

- Did any initiative drift from `judgment` to `execution` mid-increment? What caused it?
- Was I brought in before or after the key decisions on each initiative?
- What would have made me more effective in this increment?

**Forward look:**

- Which initiatives in the next PIPE are highest-leverage for my architectural practice?
- Is there an engagement pattern I need to renegotiate before the next increment?

-----

## Links Across the Hierarchy

|Direction|Level                |Document                                                                                                                           |
|---------|---------------------|-----------------------------------------------------------------------------------------------------------------------------------|
|↑ Up     |Tactical (6 quarters)|[`ARCHITECT_VALUE_MODEL.md`](https://github.com/vanHeemstraSystems/tactical-planning-management/blob/main/ARCHITECT_VALUE_MODEL.md)|
|↓ Down   |Sprint Planning      |[`ARCHITECT_VALUE_MODEL.md`](https://github.com/vanHeemstraSystems/sprint-planning-management/blob/main/ARCHITECT_VALUE_MODEL.md)  |

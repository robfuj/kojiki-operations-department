# 09 — Operations

> Part of the **Kojiki Decision System**. This repo is the
> **Operations** line. It references the shared ontology in
> [`00-kojiki-ontology`](https://github.com/robfuj/kojiki-ontology) for the
> canonical schemas, taxonomy, decision-rights, and handoff standards.

## Primary question
> How do we reliably deliver the work?

## Purpose
Execute and improve recurring work while reducing friction, cost, errors, and complexity.

## Sub-functions
Business Operations, Process Management, Service Operations, Quality, Continuous Improvement, Workforce Management, Operational Analytics, Exception Management

## Typical roles
COO, VP Operations, Operations Director, Operations Manager, Business Operations Manager, Process Improvement Manager, Quality Manager

## Inputs
Processes, demand, capacity, people, systems, service levels, exceptions.

## Outputs
Completed work, service levels, process improvements, controls, operational reports.

## Learning focus
Bottlenecks; root causes; exception patterns; automation opportunities; quality drivers; capacity constraints.

## Operating tree
```text
NORMAL PROCESS →
    OBSERVATION →
    DEVIATION →
    DETECTION →
    CLASSIFICATION →
    DIAGNOSIS →
    CONTAINMENT →
    CORRECTION →
    VERIFICATION →
    ROOT CAUSE →
    PROCESS UPDATE
```

## Decision states
```text
NORMAL → DEVIATION → DETECTED → CLASSIFIED → CONTAINED → CORRECTED → VERIFIED → ROOT-CAUSED → REDESIGNED
```

## Decision outputs
`Resolve · Contain · Escalate · Automate · Redesign · Monitor`

## Critical prompts (what this function thinks about)
> What should normally happen?
> What actually happened?
> Where did the deviation occur?
> When did it begin?
> Is this isolated or recurring?
> What caused it?
> What is the immediate risk?
> What must be contained?
> What is the permanent correction?
> How do we verify resolution?
> Why did the control fail?
> Can this be automated?
> What control should prevent recurrence?
> Should the process change?
> What should be added to organizational memory?

## Canonical record schema (docx Learning Ledger + Decision Object Fields)
Every decision in this line is recorded as:
- a **Decision Object** (docx S9) — see `schema/decision-object.json`
- a **Learning Ledger** entry (docx S7) — see `schema/learning-ledger.json`

and the agent must run the **Orientation Protocol** first (see `AGENT.md`).

## How to use
1. Read `AGENT.md` — the first-run Orientation Protocol.
2. Read `SCHEMA.md` — how this line maps to the universal schema.
3. Read `data/09-operations.json` — the machine-readable spec.
4. See `data/example.json` — one fully worked decision (Decision Object + Ledger).
5. Use `decision-graph.mmd` — agent-decodable operating tree + state model.
6. Validate new records: `python3 tools/validate.py data/<name>.json`

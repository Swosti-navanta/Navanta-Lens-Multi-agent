# Navanta Agent Experience

Two connected experiences for the Navanta multi-agent supply-chain platform, built on the
[Navanta design system](https://github.com/Navanta-AI/design-system) tokens.

## Run it

Open `index.html` in a browser. No build step, no dependencies — a single self-contained file.

```bash
open index.html
```

## The two experiences

### 1. Control Tower — "is everything under control?"

The manager's window. Risk comes before agent health, always.

- **Status view** — what's at risk, the three agents side by side with live activity,
  health, autonomy level and a pause switch each; then the needs-action queue,
  systems read/write counters, override feed and value by agent.
- **Workflow view** — the whole operation as stage lanes (Detect → Learn) with live
  instances sitting in each stage and handoff strips between agents.
- Clicking an agent card jumps to the Workflow view filtered to that agent.

### 2. Orchestrator — "what do I need to see?"

The doer's boss. Motive-driven: you arrive with a reason, and the flow is built for it.

**Entry** — ask in your own words, or pick one of five starting points:

| Motive | The question it answers |
|---|---|
| See what needs me *(default)* | What's moving, and what's waiting on my decision |
| Understand a case | What each agent did, stage by stage, and what it chose not to do |
| Question a decision | The rule, the evidence, and who was allowed to make it |
| Try a change safely | What would happen if a limit moved — replayed against real history |
| Prove what happened | A closed case as an evidence bundle |

**Workspace** — three columns:

- **Left panel (expandable)** — switch motive, pick a case
- **Centre** — the flow as stage cards: each card holds its own steps, grey branch
  cards below explain the routes *not* taken, handoff pills sit between agents
- **Right panel (expandable)** — actions for the current case, what's waiting, quick facts

Every step opens a detail drawer. Decisions, approvals and proposals happen in place.

## What it demonstrates

- One accountable case followed across three specialist agents
- Handoffs as inspectable contracts (what moved, what stayed, who accepted)
- The safe stop — acts inside limits, stops above them, and says which rule stopped it
- Verified write-back: "done" means the target system confirmed it
- Overrides captured **with the reason**, feeding governed learning proposals
- Failure recovery: a retrying write with a duplicate guard and a rollback option

## Scenario data

Built on the Navanta reference case: a vendor lead-time increase (EX-4471) that
splits into a coverage gap held for a planner (EX-4472) and a damaged-delivery
claim (EX-4474), handled by Mercer (buying), Iris (planning) and Christy (service).

## Related research

Competitive analysis and the experience model live in
`../Navanta Agents Experience/`.

# Genesis Differentiation Framework (GDF)

A pre-engineering discipline and diagnostic vocabulary for human and AI agents.

**GDF is not derived from any specific software project.** While the framework was refined through practical engineering work and AI-assisted development, it is intended as a general-purpose differentiation framework applicable to software systems, research environments, and autonomous agents.

**Version:** v0.1

---

## 1. What is GDF?

GDF is a small set of **differentiation acts** — questions that make boundaries visible before building, changing, or operating a system becomes meaningful.

It is **not** project management. It does not replace Agile, Waterfall, DevOps, Scrum, or Domain-Driven Design. It operates **before implementation**.

GDF is primarily a **diagnostic language**: a shared way to name boundary-class problems (`D2 layer collapse`, `D4 temporal failure`, `D6 authority gap`).

---

## 2. Core principles

**Form emerges through differentiation.**

Stable systems arise when boundaries, layers, scope, time, flows, authority, and limits are **distinguishable** — not when more output is produced faster.

**Most engineering failures involve a missing, collapsed, or insufficient differentiation.**

**Every engineering confusion can be investigated through differentiation.**

Common collapses:

| Collapse | Acts involved |
|----------|----------------|
| Assumption treated as fact | D1 |
| Observation treated as action | D2, D6 |
| Research treated as production | D2 |
| Signal treated as permission | D5, D6 |
| Possibility treated as scope | D3 |
| Stale artifact treated as current truth | D4 |
| Ongoing work treated as done | D7 |

*Compound cases may involve multiple acts. GDF names the **dominant** differentiation gap.*

**Important:** GDF classifies *boundary-class* issues. Model errors, metric semantics, economics, capacity, and coordination may require other disciplines in parallel.

---

## 3. Seven acts

Each act is a **question**, not a calendar stage.

| Act | Question | Rule |
|-----|----------|------|
| **D1 — Reality** | What actually exists? | Do not implement before reality is visible. |
| **D2 — Layers** | What must not be mixed? | Operate within one layer at a time. |
| **D3 — Territory** | What is inside the boundary? | No task is admissible until scope is defined. |
| **D4 — Time** | How does this exist through time? | Every artifact must have a temporal model. |
| **D5 — Flow** | What moves through the system? | Flows inform action; they do not authorize it. |
| **D6 — Authority** | Who has the right to act? | Capability is not authority. |
| **D7 — Limit** | Where must activity stop? | A system that cannot stop cannot stay stable. |

### D1 — guardrail

**D1 names epistemic state, not root cause.**

Use D1 for: known, unknown, assumption, evidence, risk, constraint.

Do **not** use D1 as a substitute for model, metric, mechanism, or economics analysis. If boundaries are correct but the world-model is wrong, that is not solved by labeling the case "D1."

---

## 4. Build mode

Use when **creating or changing** something.

Pass through D1 → D7 before substantive implementation. If an act cannot be answered explicitly, treat it as **UNDEFINED** and hold.

*Before code — separate. Before action — name. Before execution — assign authority. Before the next change — stop.*

---

## 5. Diagnostic mode

Use when **something is wrong or unclear** — not only after failure.

| Symptom | Likely act |
|---------|------------|
| «We don't understand what's happening» | D1 |
| «Layers are mixed» | D2 |
| «Wrong things were changed» | D3 |
| «Decisions on stale data» | D4 |
| «Noise looks like insight» | D5 |
| «System acted without approval» | D6 |
| «Never finishes / endless churn» | D7 |

See [`EXAMPLES/`](EXAMPLES/) for worked cases.

Optional label format:

```text
Dominant differentiation gap: D4 (Time)
Secondary gaps: D7 (Limit)
```

---

## 6. Non-goals

GDF does **not**:

- prescribe sprints, ceremonies, or delivery pipelines
- replace testing, code review, or observability
- prove a system is correct — it makes **boundaries** visible
- claim to be a complete taxonomy of all engineering failure modes

Project-specific mappings belong in implementing projects, not in GDF core.

---

## License

MIT — see [LICENSE](LICENSE).

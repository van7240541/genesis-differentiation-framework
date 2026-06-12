# GDF Visual Canon v0.1

**Status:** Authoritative for all GDF public visuals  
**Source of truth:** [`README.md`](../README.md) v0.1  
**Version:** v0.1

---

## Asset roles

| Asset | Role | Authority |
|-------|------|-----------|
| Dense infographic / concept poster | Illustration, orientation | **Non-canonical** — may simplify; do not treat poster text as normative if it diverges from this file |
| **`docs/VISUAL_CANON.v0.1.md`** | Exact strings for designers and exports | **Canonical** |
| **`assets/gdf-social-banner.png`** | GitHub social preview, LinkedIn, posts | **Canonical** — generated from strings in this file |

**Rule:** If a visual disagrees with this document, the visual is wrong.

---

## Title block

```
Genesis Differentiation Framework (GDF)
```

```
A pre-engineering discipline and diagnostic vocabulary for human and AI agents.
```

```
Version: v0.1
```

```
github.com/van7240541/genesis-differentiation-framework
```

---

## One-line positioning (social / elevator)

```
GDF is a language for talking about boundary-class failures.
```

Optional (longer):

```
Compact diagnostic vocabulary for boundary-class failures — especially in AI-assisted development.
```

---

## Core principles (verbatim)

```
Form emerges through differentiation.
```

```
Stable systems arise when boundaries, layers, scope, time, flows, authority, and limits are distinguishable — not when more output is produced faster.
```

```
Most engineering failures involve a missing, collapsed, or insufficient differentiation.
```

```
Every engineering confusion can be investigated through differentiation.
```

---

## Boundary-class caveat (verbatim — required on dense visuals)

```
GDF classifies boundary-class issues. Model errors, metric semantics, economics, capacity, and coordination may require other disciplines in parallel.
```

Short form (posters, small type):

```
Boundary-class issues only. Model errors, metric semantics, economics, capacity, and coordination may require other disciplines.
```

---

## Footer slogan (verbatim — do not paraphrase)

```
Before code — separate.
Before action — name.
Before execution — assign authority.
Before the next change — stop.
```

---

## Seven acts (verbatim)

| Act | Question | Rule |
|-----|----------|------|
| D1 — Reality | What actually exists? | Do not implement before reality is visible. |
| D2 — Layers | What must not be mixed? | Operate within one layer at a time. |
| D3 — Territory | What is inside the boundary? | No task is admissible until scope is defined. |
| D4 — Time | How does this exist through time? | Every artifact must have a temporal model. |
| D5 — Flow | What moves through the system? | Flows inform action; they do not authorize it. |
| D6 — Authority | Who has the right to act? | Capability is not authority. |
| D7 — Limit | Where must activity stop? | A system that cannot stop cannot stay stable. |

Intro line:

```
Each act is a question, not a calendar stage.
```

---

## D1 guardrail (verbatim)

```
D1 names epistemic state, not root cause.
```

```
Use D1 for: known, unknown, assumption, evidence, risk, constraint.
```

```
Do not use D1 as a substitute for model, metric, mechanism, or economics analysis. If boundaries are correct but the world-model is wrong, that is not solved by labeling the case "D1."
```

---

## Common collapses (verbatim)

| Collapse | Acts involved |
|----------|----------------|
| Assumption treated as fact | D1 |
| Observation treated as action | D2, D6 |
| Research treated as production | D2 |
| Signal treated as permission | D5, D6 |
| Possibility treated as scope | D3 |
| Stale artifact treated as current truth | D4 |
| Ongoing work treated as done | D7 |

Footnote:

```
Compound cases may involve multiple acts. GDF names the dominant differentiation gap.
```

---

## Diagnostic mode (verbatim)

Intro:

```
Use when something is wrong or unclear — not only after failure.
```

| Symptom | Likely act |
|---------|------------|
| We don't understand what's happening | D1 |
| Layers are mixed | D2 |
| Wrong things were changed | D3 |
| Decisions on stale data | D4 |
| Noise looks like insight | D5 |
| System acted without approval | D6 |
| Never finishes / endless churn | D7 |

Label format:

```
Dominant differentiation gap: D4 (Time)
Secondary gaps: D7 (Limit)
```

Example labels:

```
D2 layer collapse
D3 territory violation
D4 temporal failure
D6 authority gap
```

---

## Build mode (verbatim)

```
Use when creating or changing something.
```

```
Pass through D1 → D7 before substantive implementation. If an act cannot be answered explicitly, treat it as UNDEFINED and hold.
```

---

## Non-goals (verbatim)

```
GDF does not:
```

- `prescribe sprints, ceremonies, or delivery pipelines`
- `replace testing, code review, or observability`
- `prove a system is correct — it makes boundaries visible`
- `claim to be a complete taxonomy of all engineering failure modes`

```
Project-specific mappings belong in implementing projects, not in GDF core.
```

---

## What is GDF — short bullets (posters)

```
GDF is a small set of differentiation acts — questions that make boundaries visible before building, changing, or operating a system becomes meaningful.
```

```
It is not project management. It does not replace Agile, Waterfall, DevOps, Scrum, or Domain-Driven Design. It operates before implementation.
```

```
GDF is primarily a diagnostic language: a shared way to name boundary-class problems (D2 layer collapse, D4 temporal failure, D6 authority gap).
```

---

## Forbidden paraphrases (do not use on official visuals)

| Wrong | Use instead |
|-------|-------------|
| Before building — separate and name the acts | Before code — separate. |
| Before action — understand scope and reality | Before action — name. |
| Before the next change — define limits | Before the next change — stop. |
| Every engineering failure can be traced to a failed differentiation | Most engineering failures involve a missing, collapsed, or insufficient differentiation. |
| model, metric, economic analysis (without mechanism) | model, metric, mechanism, or economics analysis |
| replace testing or observability | replace testing, code review, or observability |
| act, adapt, and stop (footer goal) | *(not in README — do not invent)* |

---

## Social banner spec (`assets/gdf-social-banner.png`)

- **Size:** 1280 × 640 px
- **Format:** PNG
- **Must include (verbatim):** title, one-line positioning, four footer lines, version, repo URL
- **Regenerate:** when this canon file changes for v0.1 strings

---

## License

MIT — same as repository.

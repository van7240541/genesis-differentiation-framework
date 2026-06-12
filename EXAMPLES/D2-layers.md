# Example: D2 — Layer collapse

## Situation

A research notebook runs queries against the production database. An exploratory join becomes a nightly job. The team cites notebook metrics in SLA reports and incident reviews.

## Without differentiation

«We need better analytics.» Engineering adds dashboards, alerts, and more queries on production.

## Investigation

Three roles collapsed:

- **Research** (hypothesis, exploratory)
- **Production data path** (operational truth)
- **Reporting** (operational commitments)

Each layer was technically "working." The failure was **mixing layers**, not missing logic.

## Verdict

**Root differentiation failure: D2 (Layers)** — research ≠ production collapse.

## Fix direction

Separate lanes: sandbox data for exploration; promoted queries only through reviewed pipeline; reporting reads from governed sources only.

# Example: D4 — Temporal failure

## Situation

Checkout prices are wrong intermittently. The database shows correct prices. The bug appears most often the day after deployment.

## Without differentiation

«Fix pricing logic.» Team refactors calculation code and adds tests. Flakiness remains.

## Investigation

A cache layer serves prices without a defined freshness model. After deploy, stale entries persist until TTL expiry. The database is current; the **serving path** is temporally wrong.

No one asked: *When does this price stop being true?*

## Verdict

**Root differentiation failure: D4 (Time)** — stale artifact treated as current truth.

## Fix direction

Define temporal model first: source-of-truth timestamp, TTL, invalidation on deploy, observability on staleness age — then adjust code if needed.

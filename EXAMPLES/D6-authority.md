# Example: D6 — Authority gap

## Situation

An analytics service reads market signals and trade recommendations. An engineer adds «small auto-execute for testing.» The flag is left enabled in production.

## Without differentiation

«Security incident — disable the flag.» Postmortem blames one engineer.

## Investigation

The analytics path had **capability** (API access to the exchange) but no separated **permission** model (who may execute, who approves, audit trail for execution rights).

Observation and execution lived in the same component without an explicit gate.

## Verdict

**Root differentiation failure: D6 (Authority)** — capability ≠ authority.

## Fix direction

Read-only analytics credentials; execution only through a dedicated service with explicit approval gates and immutable audit logging.

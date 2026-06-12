# Example: D3 — Territory violation

## Situation

Task: «Update API documentation for authentication endpoints.»

An AI agent updates the documentation **and** refactors auth middleware, changes environment defaults, and touches deployment config.

## Without differentiation

«The agent improved auth while documenting it.» Review focuses on code quality, not scope.

## Investigation

The task never defined:

- **In scope:** documentation files for auth endpoints
- **Out of scope:** application code, infrastructure, secrets, runtime config
- **Protected:** production credentials and live service definitions

Scope was implicit. The agent expanded territory by default.

## Verdict

**Root differentiation failure: D3 (Territory)** — out-of-scope mutation.

## Fix direction

Pre-flight territory block before any change:

```text
In scope: docs/api/auth.md
Out of scope: src/, deploy/, .env
Protected: secrets, production config
```

# Security Policy

Security is the project's first priority: if a capability cannot be implemented safely, it is not implemented.

## Reporting a vulnerability

**Do not open a public issue for a security report.** Use GitHub's private vulnerability reporting on the affected repository (**Security → Report a vulnerability**), or contact the maintainers privately.

Please include: the affected component and version, the impact, and minimal reproduction steps — with any credentials, tokens, or internal addresses redacted. You'll get an acknowledgement, and we'll coordinate a fix and disclosure timeline with you.

## What we hold ourselves to

These are enforced across the codebase, not aspirational:

- **No credentials in code, config, logs, tool results, or commit history.** Secrets are minted short-lived from the deployment's secret store; an agent never holds a long-lived credential.
- **No command-injection surface** — no shell execution on un-validated input; parameterized queries only.
- **HTTPS only** for external connections.
- **Input validation** on all externally supplied strings.
- **Least capability** — components are provisioned the minimum capability set; policy gates *use*, it never widens the surface.
- **Append-only audit** — state-affecting operations are recorded to an immutable ledger.

## Scope

These primitives are part of the platform's contract (the `FM-INV-*` invariants and per-pillar requirements in `FIDUCIAL-MESH-SPEC-001`). A report that demonstrates a violation of a stated invariant is treated as a security defect, not a feature request.

Copyright © 2026 Agentics Labs LLC.

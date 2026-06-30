# Fiducial Mesh

**Cradle-to-grave traceability for AI-assisted engineering — as substrate-pluggable, open-source primitives.**

Autonomous agents are entering regulated engineering environments faster than the trust, audit, and lifecycle disciplines those environments require. Without a substrate that binds **every agent action to a verified principal**, **every policy decision to a recorded determination**, **every knowledge citation to its source**, and **every state-affecting operation to an append-only audit ledger**, the output of an agentic system cannot pass the certification gates that FAA-certified avionics, FDA-regulated devices, nuclear control systems, and the EU AI Act impose.

Fiducial Mesh is the open-source platform that supplies those primitives — and keeps them **portable across the operator's own choice of substrate** (secret store, directory, database, isolation runtime, telemetry backend), so sovereignty is a property of the architecture, not a vendor lock-in.

## The shape

Eight pillar contracts plus a pluggable host frame. Each pillar specifies *what capability it requires from substrate*, not *which product provides it* — and conformance is mechanically verified against a named profile set before any plugin reaches production.

| Pillar | | Plane |
|--------|--|-------|
| **IBX** | Inbox Exchange — agent message/work queue | State |
| **IAM** | Identity & Access Management — sovereign agent identity lifecycle | Issuance + Control |
| **PGE** | Policy Guardrail Engine — deterministic, owned policy enforcement | Control |
| **ACT** | Agent Cognitive Telemetry — append-only audit + observability | State |
| **AKB** | Agent Knowledge Base — grounded, citable knowledge retrieval | State |
| **PCS** | Plugin Control System — plugin/workflow lifecycle + conformance + registry | Control |
| **CRB** | Compute Resource Broker — workload dispatch | Control |
| **DPG** | Deterministic Proving Ground — ephemeral execution isolation | Compute |
| **MCC** | Mesh Control Center — the host frame that composes the pillars (not a pillar) | — |

The load-bearing structural commitment is the **Management + Control dyad**: runtime control (admission, dispatch, isolation, enforcement) is structurally separated from management (identity lifecycle, telemetry/audit, knowledge, conformance) — *exhibited by the contract structure itself*, not maintained by operator discipline.

## Canonical documents

The Specification is what you build to; the Handbook is what you read to understand it.

- **`FIDUCIAL-MESH-SPEC-001`** — the normative requirements (RFC 2119, numbered `FM-*` IDs, per-pillar Conformance Profiles). Current: **v1.2.1**.
- **`FIDUCIAL-MESH-HDBK-001`** — the companion narrative: design history, the dialectical-review record, worked examples.

Both are developed in the open through a **multi-agent dialectical review chain** (author → adversarial review → first-principles review → human integrator) — a method that is itself part of the credited design.

## Licensing

- **Mesh software** — GPL-3.0
- **Specification & Handbook** — CC-BY-4.0

Copyright © 2026 **Agentics Labs LLC**.

## Status

Early and active. The Specification is at v1.2.1; the reference implementation is being built and proven against the lab that produced the Specification — the lab *is* the reference implementation. Repositories flip public per-module as each clears its security and provenance gates.

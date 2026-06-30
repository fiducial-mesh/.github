# Contributing to Fiducial Mesh

Thanks for your interest. Fiducial Mesh is developed in the open under a discipline worth knowing before you start.

## The one rule everything else serves

**The Specification is what you build to.** `FIDUCIAL-MESH-SPEC-001` (with its companion `HDBK-001`) is authoritative. Drift between an implementation and the Specification is a *finding*, not a feature — and it gets fixed at the source, not papered over in code.

When you propose or change anything, the standing question is: *is this consistent with the current Specification?* Cite the requirements you touch by ID (`[FM-…]`), and verify each cite against the document text rather than recalling it.

## How work flows

1. **Open an issue first** for anything non-trivial — a [spec gap](https://github.com/fiducial-mesh/.github/issues/new?template=spec_gap.yml) or a [bug](https://github.com/fiducial-mesh/.github/issues/new?template=bug_report.yml). Discussion-stage ideas go to [Discussions](https://github.com/orgs/fiducial-mesh/discussions).
2. **Branch, don't commit to `main`.** `main` is a reviewed/release branch.
3. **Open a PR** using the template. Keep the scope tight; deliberate deferrals are fine if you name them and say why.
4. **Independent review is required** — the author is never the sole reviewer. Substantive changes get an adversarial pass and, for normative spec changes, a first-principles pass before merge. This multi-perspective review is deliberate: no single reviewer, however expert, reliably sees the blind spot in their own work.
5. **Normative spec changes** bump the version and update the Revision History / changelog. A normative change is never merged as a silent patch.

## Conformance

A change to a pillar or plugin is not done until the affected conformance/validation passes. The Specification fixes *what a substrate seam must satisfy*, not *which product provides it* — keep contributions substrate-neutral at the contract layer and prove them against the named profile set.

## Security & secrets

Never introduce a credential, token, key, or routable internal address into code, config, logs, tests, or commit history. See [SECURITY.md](SECURITY.md). Security concerns are reported privately, not in public issues.

## Licensing

By contributing you agree your contributions are licensed under the repository's license: **GPL-3.0** for mesh software, **CC-BY-4.0** for the Specification and Handbook. Copyright © 2026 Agentics Labs LLC.

## Conduct

Participation is governed by our [Code of Conduct](CODE_OF_CONDUCT.md).

# Contributing to AXL Protocol

AXL Protocol is a community-stewarded language for AI agent communication. The protocol kernel, the public tooling, and the documentation are all Apache 2.0 and developed in the open. Contributions of code, prose, RFC participation, and experiment reports are all welcome.

This document is the org-level default. Individual repos may add a `CONTRIBUTING.md` of their own that supplements (but does not contradict) this one.

## Where to discuss

The canonical conversation venue is **[GitHub Discussions on axlprotocol/community](https://github.com/axlprotocol/community/discussions)** (also surfaces at the [org-level page](https://github.com/orgs/axlprotocol/discussions) for cross-repo discoverability). The website portal at [axlprotocol.org/community/](https://axlprotocol.org/community/) links into the same conversation.

For repo-specific bug reports and feature requests, file an issue in the repo where the change would land.

## Proposing a substantive change

The bar scales with the blast radius of the change.

| Change class | Process |
|---|---|
| Editorial fix, typo, doc clarification | Direct PR. Any maintainer can merge. |
| Minor extension (new module in v4 router, alias, additive helper) | Open a Discussion to gauge interest, then PR with one maintainer review. |
| Breaking change (kernel grammar, packet format, semantic operation set) | RFC required. 14-day public comment window. Founding-steward approval. |
| Governance, foundation, or trademark change | RFC required. 30-day public comment window. Founding-steward approval. |

RFCs live under `/community/` on the website. The format is loose - a clear motivation, a proposal, considered alternatives, and a migration story is enough. See `GOVERNANCE.md` for the full decision matrix.

## Bug reports

File in the repo where the bug lives, using the bug-report issue form. Include:

- A minimal reproduction (commands, code, input)
- Expected behavior vs. actual behavior
- Environment (OS, Python version, package version, LLM if relevant)
- Logs or output if available

If the bug is a security vulnerability, do **not** file it publicly. See `SECURITY.md`.

## Feature requests

File in the repo where the feature would land, using the feature-request issue form. State the user story and the proposed solution. Indicate whether you can contribute the implementation.

If the request is substantive (touches the kernel, the packet format, or the semantic operation set), open a Discussion first. An RFC is likely required.

## Commit messages

- Short summary line, ideally under 70 characters
- Blank line, then a body that explains *why*
- No emoji prefixes
- Conventional Commits is welcome but not required

## Co-author attribution

Use the `Co-Authored-By: Name <email@example.com>` trailer for pair-programmed work or AI-assisted contributions. Multiple trailers are fine.

## Testing

Code repos add tests for new behavior. The discipline marker is `axl-research`'s 217/217 test suite - public repos should aim for the same posture as they mature. Documentation-only PRs are exempt.

Run tests locally before opening a PR. CI gates the merge.

## License posture (read carefully)

AXL Protocol uses **Apache 2.0 inbound = outbound**. By submitting a contribution you agree that your work is licensed under Apache 2.0 to the project and to anyone who receives the project under that license. There is **no CLA** to sign. There is no relicensing path that would let the project later strip the Apache 2.0 grant from your contribution.

If you are contributing on behalf of an employer, ensure you have authority to do so under your employment agreement. Contributions under aliases are accepted; consider what that means for your future ability to claim the work.

## Trademark

The name "AXL Protocol" is reserved. Forks should rename to avoid confusion with the upstream project. Trademark formalization is pending foundation incorporation - see `GOVERNANCE.md`.

## Code review

The founding steward (Diego Carranza) currently has tie-breaker authority for the first 12 months of the community pivot. After that, decision-making moves to a Technical Steering Committee model as documented in `GOVERNANCE.md`. In practice: substantive PRs receive at least one maintainer review, breaking changes go through RFC, and most of the day-to-day flow is collaborative review with consensus.

## Questions

Open a Discussion at [axlprotocol.org/community/](https://axlprotocol.org/community/) or email admin@axlprotocol.org.

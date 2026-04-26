# AXL Protocol Governance

## Status

DRAFT, effective 2026-04-25. This is the v0 governance document for the community pivot. It will be ratified or revised through the public RFC process within 90 days (target: 2026-07-25).

## Founding steward

Diego Carranza is the founding steward of AXL Protocol. The founding steward:

- Holds Apache 2.0 trademark / brand stewardship for the "AXL Protocol" name
- Has tie-breaker authority for the first 12 months on contested decisions
- Maintains the spec freeze cadence (currently quarterly)
- Curates the canonical research repo (`axl-research`, currently private during productization gates)

This is a transitional model. The founding steward role exists to make decisions cleanly during the period before formal governance structures are in place. It is not a permanent fixture; the foundation arc (below) replaces it.

## Decision-making

Substantive changes go through the public RFC process at [/community/](https://axlprotocol.org/community/). Categories of change and their process:

| Class | Process | Comment window |
|---|---|---|
| Editorial / typo / clarification | Direct PR, any maintainer can merge | none |
| Minor extension (new module in v4 router, new operation alias, additive helper) | PR + 1 maintainer review | none |
| Breaking change (kernel grammar, packet format, semantic operation set) | RFC required, founding-steward approval | 14 days |
| Governance / foundation / trademark | RFC required, founding-steward approval | 30 days |

RFCs are filed as Discussions in the community venue with the `RFC` label. The comment window starts when the RFC is marked `RFC: open`. Approval requires the founding-steward sign-off (in the first 12 months) or simple maintainer majority (after the 12-month window).

## Maintainers

Initial maintainer: Diego Carranza (founding steward).

**Path to maintainership:** contribute substantively for 6 or more months (commits, RFC participation, code review). The founding steward nominates. New maintainers are added with a public announcement on /community/ Announcements.

Maintainer authority: merge access on the repos they steward, vote on RFCs (after the 12-month founding-steward window closes), participation in maintainer sync (cadence TBD).

Removal: voluntary, or by founding-steward decision (with public reason) during the first 12 months, or by simple maintainer majority after.

## License posture

**Apache 2.0 in perpetuity** for the protocol spec and the public tooling:
- `axl-core` (PyPI: axl-core)
- `axl-mcp-tools`
- `axl-compress` backend (when published)
- `compress.axlprotocol.org` (the project landing repo)
- `bridge.axlprotocol.org`
- `docs` (the Mintlify content repo)
- `ark`, `axl-silo`, `axl-battlegrounds`, `axl-swarm`, `axl-sophon` (research repos)

No commercial relicensing. No copyleft. No CLA required (Apache 2.0 inbound = outbound is sufficient).

Private research repos (`axl-research`, `axl-compress` backend pre-publication) may remain private during productization gates but ship to public mirror under Apache 2.0 when promoted.

## Foundation arc

**Goal:** incorporate AXL Protocol Foundation as a 501(c)(3) or equivalent within 24 months (target: 2028-04-25).

The foundation will:
- Hold trademark for the "AXL Protocol" name
- Manage donations and sponsorship infrastructure
- Serve as the legal home for the project
- Govern via a Technical Steering Committee

At foundation incorporation:
- The founding steward steps back to a Technical Steering Committee role
- Decisions transition from founding-steward tie-breaker to TSC majority
- Trademark transfers from individual stewardship to the foundation

## Trademark

The "AXL Protocol" name is reserved during the founding-steward period. Forks should rename. Trademark formalization is pending foundation incorporation; until then, the name is informally protected by the founding steward's stewardship.

After foundation incorporation, the foundation holds the mark and will publish a trademark policy with permitted-use guidelines.

## Conflict of interest

Founding steward must publicly disclose any commercial AXL-related work in /community/ Announcements. Maintainers must recuse from RFC decisions where they have a material conflict.

Disclosure includes: paid consulting that uses AXL, equity stakes in companies that depend on or compete with AXL, employment relationships that create alignment or pressure on AXL decisions.

## Amendment

This document can be amended via the governance-class RFC process (30-day comment window, founding-steward approval) until foundation incorporation. After incorporation, amendments go through the foundation's bylaws.

The 90-day ratification window from 2026-04-25 means this document is provisional until 2026-07-25; substantive changes during that window only require maintainer review (not founding-steward approval) since the document is not yet ratified.

## Contact

- General questions: [/community/](https://axlprotocol.org/community/)
- Founding steward: admin@axlprotocol.org
- Security: see [SECURITY.md](SECURITY.md)

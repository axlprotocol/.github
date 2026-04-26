# Security Policy

## Reporting a vulnerability

We take security seriously. Please report vulnerabilities privately, not in public issues or Discussions.

**Preferred channel:** [GitHub Security Advisories on axlprotocol/security](https://github.com/axlprotocol/security/security/advisories/new) (private repo, advisories accept reports from anyone)

**Email:** admin@axlprotocol.org

**Machine-readable contact:** https://axlprotocol.org/.well-known/security.txt (RFC 9116)

## Response SLA

| Stage | Target |
|---|---|
| Initial acknowledgment | within 72 hours |
| Triage and severity assessment | within 7 days |
| Fix or mitigation plan (high/critical) | within 30 days |
| Fix or mitigation plan (medium/low) | within 90 days |

## Scope

**In scope:**
- All public repos under [github.com/axlprotocol](https://github.com/axlprotocol)
- All public AXL Protocol services:
  - axlprotocol.org
  - compress.axlprotocol.org
  - bridge.axlprotocol.org
  - docs.axlprotocol.org
  - lang.axlprotocol.org
- The `axl-core` PyPI package
- The `axl-mcp-tools` MCP integrations

**Out of scope:**
- Third-party services we depend on (GitHub, PyPI, Cloudflare, etc.) - report directly to them
- Social engineering attempts targeting contributors - report to the contributor and to us
- Physical attacks against AXL Protocol infrastructure operators

## Disclosure

After a fix is shipped:
- Public CVE filed (if applicable to severity)
- Public advisory posted on the affected repo
- Acknowledgment in release notes (with reporter consent)

## Bounty

No formal bounty program currently. AXL Protocol is community-stewarded and has no commercial revenue stream that would fund a bounty pool. Reporters are acknowledged publicly (with consent) and may be invited to maintainer status if their contribution is sustained.

## Hall of fame

Contributors who responsibly disclose vulnerabilities are acknowledged at:
- https://axlprotocol.org/security/acknowledgments/ (page reserved; populated as disclosures arrive)

## Public-key encryption

If you want to encrypt your report:
- PGP key: TBD (the project does not yet publish a PGP key; for now, GitHub Security Advisories provides transport-layer privacy)

## Coordinated disclosure

We follow a 90-day coordinated disclosure window for severe issues, extendable by mutual agreement. If we have not shipped a fix or mitigation within 90 days of a verified report, the reporter may publish their findings.

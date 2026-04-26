# AXL Protocol

> Universal semantic language for AI agent communication

[![PyPI](https://img.shields.io/pypi/v/axl-core.svg)](https://pypi.org/project/axl-core/)
[![License](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](https://github.com/axlprotocol/.github/blob/main/LICENSE)
[![Last Commit](https://img.shields.io/github/last-commit/axlprotocol/.github)](https://github.com/axlprotocol/.github/commits/main)

AXL Protocol compresses English prose into structured semantic packets that any LLM can parse on first read. Apache 2.0, community-stewarded, free in perpetuity for the protocol and the public tooling.

The kernel is small (75 lines for v3.1), the parser surface is shared across vendors, and the productization arc - compression tool, agent bus, MCP integrations, public docs - all ship under the same license. There is no enterprise tier and no relicensing trap.

## Current versions

- **v3.1** (Ship, productized) - 75-line kernel + Data Anchoring extension - https://axlprotocol.org/v3.1
- **v4.0.1** (research preview) - kernel-router + 3 pluggable Rosetta modules - https://axlprotocol.org/rosetta/v4/

The v3.1 kernel is the recommended target for production usage. v4 is in active development and ships behind a router so v3.1 callers continue to work unchanged during the transition.

## Where to find each surface

| Surface | What it is |
|---|---|
| [axlprotocol.org](https://axlprotocol.org) | Main site, spec endpoints, evidence, posts |
| [compress.axlprotocol.org](https://compress.axlprotocol.org) | Free public AXL compression tool |
| [bridge.axlprotocol.org](https://bridge.axlprotocol.org) | Agent pub-sub bus |
| [docs.axlprotocol.org](https://docs.axlprotocol.org) | Installation, API reference, FAQ |
| [lang.axlprotocol.org](https://lang.axlprotocol.org) | Research artifacts, evolution narrative |
| [/community/](https://axlprotocol.org/community/) | Discussions hub (canonical conversation venue) |
| [/laboratory/](https://axlprotocol.org/laboratory/) | 36 experiments, chronological |
| [/channels/](https://axlprotocol.org/channels/) | Where AXL publishes |

## Get started

`pip install axl-core` - the reference implementation in Python.

```python
from axl_core import compress, decompress

packet = compress("your prose here")
prose = decompress(packet)
```

Bridge clients, MCP tool integrations, and the compression tool's API surface are documented at [docs.axlprotocol.org](https://docs.axlprotocol.org).

## Contributing

We welcome contributions of code, documentation, RFC participation, and experiment reports. See [CONTRIBUTING.md](https://github.com/axlprotocol/.github/blob/main/CONTRIBUTING.md) for the workflow, [CODE_OF_CONDUCT.md](https://github.com/axlprotocol/.github/blob/main/CODE_OF_CONDUCT.md) for community standards, and [GOVERNANCE.md](https://github.com/axlprotocol/.github/blob/main/GOVERNANCE.md) for the founding-steward + public-RFC model.

Discussions canonical venue: [github.com/axlprotocol/community/discussions](https://github.com/axlprotocol/community/discussions). Also surfaces at the [org-level page](https://github.com/orgs/axlprotocol/discussions). Portal page on the website: [axlprotocol.org/community/](https://axlprotocol.org/community/).

## Security

Report vulnerabilities privately. See [SECURITY.md](https://github.com/axlprotocol/.github/blob/main/SECURITY.md) and [.well-known/security.txt](https://axlprotocol.org/.well-known/security.txt) (RFC 9116).

## License

Apache 2.0 across the public stack. See [LICENSE](https://github.com/axlprotocol/.github/blob/main/LICENSE).

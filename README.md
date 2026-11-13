# hunt-iocs

Indicators and search queries for infrastructure I track. One plain-text file per tracker.

| Tracker | What it covers | Queries | IPs |
|---|---|---|---|
| [AntiFox](AntiFox.md) | Exposed AntiFox consoles (AI pentest platform, fork of ARTEX). | Shodan | 160 |
| [ARTEX behind basic auth](ARTEX-Basic-Auth.md) | ARTEX-family consoles hidden behind an HTTP basic-auth prompt whose realm names the product. | Shodan | 13 |
| [ARTEX family](ARTEX-Family.md) | Exposed consoles of ARTEX and its forks/rebrands (AntiFox, ScopeWeaver, renamed builds). Run both Shodan queries and union the results. | Shodan | 2060 |
| [ScopeWeaver](ScopeWeaver.md) | Exposed ScopeWeaver consoles (English/Korean rebrand of ARTEX). IPs are hosts with ScopeWeaver in the page title. The favicon query is broader and also matches other builds, so check those hits before relying on them. | Shodan | 54 |

## File format

Each tracker is a Markdown file. Every section is a fenced code block with one item per line, so entries can be copied or extracted without Markdown noise. Sections used: `Shodan`, `Censys`, `FOFA`, `IPs`, `Domains`, `URLs`. Empty sections are omitted. A query is listed only after it has been run and checked on that platform.

## Read this before using the data

- An entry means the host matched the tracker at collection time. It does not mean the host is malicious, compromised, or operated by any particular actor. Offensive-security tools are also run by testers, students and labs.
- Cloud addresses are reassigned. Check a host yourself before blocking or reporting it.
- Lists are point-in-time and are replaced, not appended, on each update. Use the git history for earlier snapshots.
- Nothing here is attribution.

## Contact

- Blog: <https://medium.com/@straw_hat_intel>
- Email: <keith@strawhatintel.com>

Last updated: 2026-11-13

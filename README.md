# Partha Dhar

Backend and platform engineer. Kolkata, India.\
I build things that run unattended, and I write down where they break.

## Selected work

| Project | What it is | Notable |
|---|---|---|
| [listenbrainz-widget](https://github.com/ParthaDhar/listenbrainz-widget) | Self-hosted now-playing SVG cards for ListenBrainz, MIT. [Live](https://lb.parthadhar.com/widget/PaulDr/c108c6b11cd6eda37aed766da58e6f33b7c0b0f9a1ba8da88158c848a54ea5e4?theme=dark&layout=default&palette=classic&count=1) | Display-privacy flags are bound to the token at issue time, so editing the URL cannot widen them. ETag plus a soft-refresh parameter to beat a proxy that cached the fallback art. |
| [Audio_Quality_Profiling](https://github.com/ParthaDhar/Audio_Quality_Profiling) | Audio library quality and duplicate scanner: Python, ffprobe, mutagen | A lossy codec at a high sample rate is an upsample: flagged at 0.9 confidence, score halved. Every scoring path returns its evidence, not a bare number. Ran clean on a 4,100-file library. |
| [iswap-contracts](https://github.com/ParthaDhar/iswap-contracts) | Uniswap-V2-style AMM contracts ported to TRON, deployed snapshot | A distinct CREATE2 init-code hash per network, and both Base58 and hex forms of every deployed address. Get the hash wrong and every pair address silently resolves to nothing. |
| [wb-electoral-data](https://github.com/partha-dhar/wb-electoral-data) | Bulk text-recovery pipeline for deliberately garbled government PDFs | Text came out as shifted garbage until a character-identifier (CID) mapping was built to decode the embedded fonts. 7,936 PDFs downloaded and validated, extraction logged at about 7.6 s per PDF, cross-check API calls self-throttled to 2 req/s under a published 50 req/s limit. |

## Also shipped, not here

Client work, under NDA:

- Cryptocurrency exchange infrastructure handling real money, with BTC, ETH and TRON full
  nodes in production.
- A legacy AWS and ColdFusion estate whose database holds records back to 1994, modernised
  incrementally with no staging environment to practise on.
- A serverless invoice ingestion pipeline on AWS Lambda, 51 of 52 commits mine: 48 gated
  migrations, a read-only preflight, a snapshot before anything irreversible. 15,244 invoices
  re-transformed with zero errors.
- A self-hosted SonarQube and GitLab CI quality gate that files findings back as
  de-duplicated issues, adopted into three client pipelines.

Public, under an organisation account rather than mine:

- 146 commits across three interfaces of a multi-chain AMM, as second committer, from the
  organisation's first week. Live since 2022.

## How I work

- Measure before deciding, and keep the measurement next to the decision.
- End with the limits: what I did not check, and which of my own earlier conclusions were wrong.
- Guardrail before feature. Dry run by default. Make the dangerous operation structurally
  unable to do the wrong thing, rather than adding a confirmation.
- Smallest thing that works. A new dependency is a conversation, not an edit.

## Stack

Python - PHP / Laravel - Node - TypeScript - Bash - Solidity\
AWS - Docker - GitLab CI - GitHub Actions - nginx - Apache - systemd\
Postgres - MySQL - SQLite - DuckDB - Redis\
SonarQube - opengrep - grype - trivy - fail2ban - iptables / ipset

## Elsewhere

[cv.parthadhar.com](https://cv.parthadhar.com) - [LinkedIn](https://www.linkedin.com/in/parthadhar/) - [parthadhar@hotmail.com](mailto:parthadhar@hotmail.com)

![GitHub stats](https://github-readme-stats.vercel.app/api?username=ParthaDhar&show_icons=true&count_private=true)

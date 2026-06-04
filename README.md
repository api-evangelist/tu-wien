# TU Wien (tu-wien)

TU Wien (Vienna University of Technology) is Austria's largest science and technology university, founded in 1815, with more than 30,000 students and eight faculties, and ranked #190 in the QS World University Rankings 2025. This repository catalogs TU Wien's public, documented developer/API footprint as an [APIs.json](https://apisjson.org) profile. That footprint centers on research infrastructure — a research data repository REST API and OAI-PMH metadata interfaces — rather than a single unified developer portal.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/tu-wien/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=tu-wien-api-evangelist&utm_content=repo

## Type

- Index
- Consumer
- 3rd-Party

## Tags

Education, Higher Education, University, Research Data, Open Access, Repository, OAI-PMH, InvenioRDM, Austria, Europe

## APIs

- **TU Wien Research Data REST API** — Public InvenioRDM REST API for records, metadata, search and file content; reads are public, writes require a bearer token. Docs: https://researchdata.tuwien.ac.at/tuw/about/api (base: `https://researchdata.tuwien.ac.at/api`)
- **TU Wien Research Data OAI-PMH** — OAI-PMH metadata harvesting for the Research Data repository. Endpoint: `https://researchdata.tuwien.ac.at/oai2d`
- **reposiTUm OAI-PMH** — OAI-PMH metadata harvesting for the reposiTUm open-access institutional repository (DSpace-CRIS). Endpoint: `https://repositum.tuwien.at/oai/openaire`. Docs: https://www.it.tuwien.ac.at/en/services/research-projects-publications/repositum

## Plans

See [plans/tu-wien-plans-pricing.yml](plans/tu-wien-plans-pricing.yml).

## Rate Limits

See [rate-limits/tu-wien-rate-limits.yml](rate-limits/tu-wien-rate-limits.yml).

## FinOps

See [finops/tu-wien-finops.yml](finops/tu-wien-finops.yml).

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.tuwien.at/en/
- GitHub: https://github.com/tuwien-csd
- LinkedIn: https://www.linkedin.com/school/tuwien
- Plans: plans/tu-wien-plans-pricing.yml
- Rate Limits: rate-limits/tu-wien-rate-limits.yml
- FinOps: finops/tu-wien-finops.yml
- Review: review.yml

## Notes

All APIs and URLs were probed live on 2026-06-03; no endpoints were fabricated. The Research Data REST API and both OAI-PMH endpoints returned valid responses. The bare `https://repositum.tuwien.at/oai/request` path returned HTTP 500 when called without an OAI verb, so the working OpenAIRE endpoint is cataloged instead. TISS (study/course system) and TUWEL (Moodle) are live but expose no public, documented developer API. There is no single official university-wide GitHub organization; open-source code is fragmented across departmental orgs such as `tuwien-csd` and `TUWBIB`. The university has no general-purpose public developer portal — its documented API surface is research-repository oriented.

## Maintainers

- Kin Lane — kin@apievangelist.com

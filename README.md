# openEHR

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

openEHR is the open specification family for electronic health records, and the main structural alternative to HL7 FHIR. It is governed by two UK not-for-profit entities: the openEHR Foundation, a company limited by guarantee that holds the intellectual property, and the openEHR Community Interest Company, trading as openEHR International, which has run day-to-day operations since 10 May 2019. Its defining idea is two-level modelling — a small, stable Reference Model that software implements once, plus a large, separately governed body of clinician-authored archetypes and templates expressed in the Archetype Definition Language and queried through the Archetype Query Language. The specification site publishes 68 specifications across 14 components at three maturity levels of openEHR's own declaring: Stable (AM, BASE, CDS, ITS-REST, ITS-XML, LANG, QUERY, RM, TERM), Development (CNF, ITS-BMM, ITS-JSON, SM) and Paused (PROC). The ITS-REST component ships real OpenAPI 3.0 for six API surfaces — EHR, Query, Definition and System are STABLE, Demographic and Admin are DEVELOPMENT — under a Creative Commons Attribution-NoDerivs 3.0 licence, with the tooling repositories under Apache-2.0. The coalition is unusually legible: 59 named people across the CIC Board, Foundation Board and the Specification, Clinical and Education program boards, with employers published beside 37 of them. What this repo holds are SPECIFICATIONS, not services — every contract here has the templated server https://{baseUrl}/v1 and describes what a conformant implementation must offer, so none of it is a callable API and it must never be read as one.

**Areas:** openEHR · Healthcare · Electronic Health Records · Health Informatics · Standards · Specification · Interoperability · Information Model · Archetypes · AQL · ADL · Clinical Modelling

## openEHR on APIs.io

Everything profiled for openEHR is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/openehr/](https://apis.io/providers/openehr/)** — or go straight to one of the APIs or properties below.

### APIs (16)

- [openEHR ADL1.4 API](https://apis.io/apis/openehr/openehr-adl1-4-api/) — Management of [AOM and ADL 1.4](https://specifications.openehr.org/releases/AM/latest) Operational Templates (OPTs). These templates can be created using…
- [openEHR ADL2 API](https://apis.io/apis/openehr/openehr-adl2-api/) — Management of [AOM2](https://specifications.openehr.org/releases/AM/latest/AOM2.html#_templates) templates. See also [ADL2 Template…
- [openEHR AGENT API](https://apis.io/apis/openehr/openehr-agent-api/) — Management of the [AGENT](https://specifications.openehr.org/releases/RM/latest/demographic.html#_agent_class) class.
- [openEHR COMPOSITION API](https://apis.io/apis/openehr/openehr-composition-api/) — Management of [COMPOSITION](https://specifications.openehr.org/releases/RM/latest/ehr.html#_composition_class) and…
- [openEHR CONTRIBUTION API](https://apis.io/apis/openehr/openehr-contribution-api/) — Management of [CONTRIBUTION](https://specifications.openehr.org/releases/RM/latest/common.html#_contribution_class) class.
- [openEHR DIRECTORY API](https://apis.io/apis/openehr/openehr-directory-api/) — Management of the [directory](https://specifications.openehr.org/releases/RM/latest/ehr.html#_directory)…
- [openEHR EHR API](https://apis.io/apis/openehr/openehr-ehr-api/) — Admin management of [EHRs](https://specifications.openehr.org/releases/RM/latest/ehr.html#_ehr_class).
- [openEHR EHR STATUS API](https://apis.io/apis/openehr/openehr-ehr-status-api/) — Management of [EHR_STATUS](https://specifications.openehr.org/releases/RM/latest/ehr.html#_ehr_status_class) and…
- [openEHR GROUP API](https://apis.io/apis/openehr/openehr-group-api/) — Management of the [GROUP](https://specifications.openehr.org/releases/RM/latest/demographic.html#_group_class) class.
- [openEHR ITEM TAG API](https://apis.io/apis/openehr/openehr-item-tag-api/) — Management of [ITEM_TAG](https://specifications.openehr.org/releases/RM/development/common.html#_item_tag_class) resources.
- [openEHR Options API](https://apis.io/apis/openehr/openehr-options-api/) — The Options API from openEHR — 1 operation(s) for options.
- [openEHR ORGANISATION API](https://apis.io/apis/openehr/openehr-organisation-api/) — Management of the [ORGANISATION](https://specifications.openehr.org/releases/RM/latest/demographic.html#_organisation_class) class.
- [openEHR PERSON API](https://apis.io/apis/openehr/openehr-person-api/) — Management of the [PERSON](https://specifications.openehr.org/releases/RM/latest/demographic.html#_person_class) class.
- [openEHR Query API](https://apis.io/apis/openehr/openehr-query-api/) — Management of stored (registered) queries in the system, including creation of new versions and retrieval by qualified name and version. These endpoints…
- [openEHR ROLE API](https://apis.io/apis/openehr/openehr-role-api/) — Management of the [ROLE](https://specifications.openehr.org/releases/RM/latest/demographic.html#_role_class) class.
- [openEHR VERSIONED PARTY API](https://apis.io/apis/openehr/openehr-versioned-party-api/) — Management of the [VERSIONED_PARTY](https://specifications.openehr.org/releases/RM/latest/demographic.html#_versioned_party_class) class.

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Agentic access (1)

Which operations an agent can call, which act, and which need a human in the loop.

- [Openehr Agentic Access](https://apis.io/agentic-access/openehr/openehr-agentic-access/)

#### JSON Schema (3)

The data models the API reads and writes.

- [Openehr Rm 1.0.3 All](https://apis.io/schemas/openehr/openehr-rm-1.0.3-all/)
- [Openehr Rm 1.0.4 All](https://apis.io/schemas/openehr/openehr-rm-1.0.4-all/)
- [Openehr Rm 1.1.0 All](https://apis.io/schemas/openehr/openehr-rm-1.1.0-all/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://openehr.org/)
- [Documentation](https://developer.openehr.org/implementation/)
- [API reference](https://specifications.openehr.org/releases/ITS-REST/latest/)
- [Changelog](https://specifications.openehr.org/releases)
- [Blog](https://openehr.org/blog/)
- [GitHub](https://github.com/openEHR)

## API Evangelist rating

**Kin Score 28.1** — thin · rubric 0.24.0 · scored 2026-10-17

| Facet | Score |
|---|---|
| Discoverability | 70.5 |
| Contract quality | 54.1 |
| Contract governance | 13.6 |
| Operational transparency | 18.4 |
| Developer ergonomics | 28.6 |
| Access clarity | 0.0 |

**Agent readiness 17.3** — agent-aware

| Agent-readiness dimension | Result |
|---|---|
| Spec Presence | yes |
| Agentic Access | derived (partial credit) |
| Reversibility Documented | — |
| MCP Server | — |
| Auth Clarity | — |
| Idempotency | — |
| Error Semantics | — |
| OpenAPI Examples | partial |
| Rate Limit Signal | — |
| Event Surface Described | — |
| Agent Skills | — |
| Well Known Catalog | — |
| Consent Identity | — |
| Agent Card | — |
| Dry Run Mode | — |
| Delegated Identity | — |
| Protected Resource Metadata | — |
| Dynamic Client Registration | — |
| Agentic Commerce | — |

**Regulatory alignment 2.0** — Health

The rubric is published at [github.com/api-evangelist/kin-score](https://github.com/api-evangelist/kin-score). The per-check breakdown behind these numbers — which checks were earned, partial or missed — along with score history and how this provider compares to its peers, is available at [apis.io/providers/openehr/](https://apis.io/providers/openehr/).

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for openEHR: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/openehr/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).

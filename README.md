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
A **standards-body** profile in the API Evangelist network — the third class of repo alongside API
producers (`pipeline-enrich`) and investors (`pipeline-vc`). A standard is not a product; it is a
coalition with artifacts, so this repo profiles the **specifications**, the **governance**, the
**maturity ladder**, and above all the **people and organizations in the room**.

Profiled 2026-09-02.

## What openEHR is

The open specification family for electronic health records, and the main structural alternative to
[HL7 FHIR](https://github.com/api-evangelist/fhir). Its defining idea is **two-level modelling**: a
small, stable Reference Model that software implements once, plus a large, separately governed body of
clinician-authored **archetypes** and **templates** written in the Archetype Definition Language and
queried through the Archetype Query Language.

Two UK not-for-profit entities govern it. The **openEHR Foundation** (company limited by guarantee)
holds the intellectual property. The **openEHR Community Interest Company**, trading as **openEHR
International**, has run day-to-day operations since **10 May 2019**. The Foundation is expected to
merge into openEHR International.

**14 specification components, 68 specifications.** openEHR's own maturity ladder, read from its
machine-readable component catalog: **Stable** — AM, BASE, CDS, ITS-REST, ITS-XML, LANG, QUERY, RM,
TERM. **Development** — CNF, ITS-BMM, ITS-JSON, SM. **Paused** — PROC.

## The findings worth naming

**1. openEHR's specification site is genuinely agent-native, and almost no standards body is.**
`specifications.openehr.org` serves a real `llms.txt` (11,107 bytes, verified 2026-09-02), gives every
specification page a Markdown twin reachable either by appending `.md` or by sending
`Accept: text/markdown` (`architecture_overview.md` → HTTP 200, `text/markdown`, 183,557 bytes), and
exposes three structured JSON endpoints — `/api/components.json`, `/api/classes.json`,
`/api/releases.json`. The gap is the front door: **`openehr.org/llms.txt` is a 404**, so the
organization is less legible to a machine than the specifications behind it.

**2. Free to read is not the same as openly licensed.** Every published ITS-REST OpenAPI declares
`license: Creative Commons Attribution-NoDerivs 3.0 Unported`. The specifications are free to retrieve
and free to implement, but **ND** means a modified redistribution of a specification document is not
permitted. The tooling repositories are Apache-2.0 — the split is real and worth keeping straight.

**3. The coalition is public, and its companies are entirely absent from this network.** openEHR
publishes 59 named people with roles across five bodies, with employers beside 37 of them. Matched
against the api-evangelist network: **0 of 34 organizations have a repo.** The openEHR vendor ecosystem
— Better, Nedap Healthcare, Ocean Health Systems, DIPS, vitagroup, EHRbase, Medblocks, Cambio, Marand,
CaboLabs, VeraTech — is a complete blind spot in the catalog. That is the most actionable thing this
profile produced, and it is in `leads/`.

**4. There is no conformance programme to check anyone against.** The CNF (Conformance Specifications)
component exists but is **Development** status. Where OGC has CITE, openEHR has no certification mark,
so a claim of openEHR conformance currently has nothing public to test it against.

**5. These contracts are specifications, not services.** Every OpenAPI here declares the templated
server `https://{baseUrl}/v1` and describes what a conformant implementation must offer. That is
openEHR's design, not a defect, and it is why **a standards body must never be read through the
provider Kin Score composite** — the rubric measures services, and openEHR does not publish one.

## What is here

| Artifact | Contents |
|---|---|
| `apis.yml` | Identity + the 6 REST API specifications openEHR publishes as OpenAPI 3.0 |
| `openapi/_original/` | 7 OpenAPI documents harvested from `specifications-ITS-REST`, 65 paths |
| `openapi/` | The 6 with operations; `overview` is a pathless container doc, kept in `_original/` only |
| `taxonomy/` | 14 components / 68 specifications with openEHR's own Stable–Development–Paused status |
| `governance/` | Both legal entities, five bodies, the licensing split, and the recorded gaps |
| `people/` | **59 named people** across the CIC Board, Foundation Board, SEC, CPB and EPB |
| `companies/` | **34 organizations** named as an employer beside a roster name |
| `leads/` | **34 organizations with no repo yet** — every single one |
| `working-groups/` | The four openEHR programs and what each produces |
| `repositories/` `releases/` `contributors/` | 52 repos in the `openEHR` GitHub org |
| `agentic-access/` | 97 recommended `x-agentic-access` execution contracts, derived from the OpenAPIs |

## Notes on how this was built

The roster extractor in `harvest-standards-people.py` does **not** fit openEHR's page layouts — it
returned section headings and code-of-conduct prose as people. Every one of the 59 people here was
read off the source page by hand instead, and `people/openehr-people.yml` records that. No name,
employer, seat or adoption claim is guessed.

The GitHub maturity harvest returned **52 unclassified** repositories: openEHR does not encode maturity
in repo descriptions the way CAMARA does. `taxonomy/` is the authoritative maturity read, and it comes
from openEHR's own machine-readable catalog rather than from us.

**Correction (2026-09-02, same day).** An earlier version of this README said openEHR's matching key is
"a bare org name typed into a table, not a URL." That is wrong. openEHR publishes **name + website URL**
for its partners on two pages — `openehr.org/industry-partners/` (35 vendors) and
`openehr.org/organisation-partners/` (15 public bodies) — so matching here can be authoritative by
domain, exactly like OGC, rather than by name guessing. The `companies/` artifact in this repo is
derived from the *program-board rosters*, which genuinely carry no URLs; the partner pages are a
separate and better source, and they are what the vendor cohort in `leads/` was harvested from.

One matcher correction was made: **Better** (better.care, the Slovenian openEHR platform vendor) was
matched to `all/better`, which is **better.com**, the US mortgage lender. That pair is now in the
`REJECT` set in `match-standards-companies.py` and Better is recorded as a lead.

## Sources

- `https://openehr.org/` — governance, and the four program board rosters
- `https://specifications.openehr.org/` — the specifications, `llms.txt`, and the three JSON endpoints
- `https://github.com/openEHR/specifications-ITS-REST` — the OpenAPI 3.0 documents
- `https://ckm.openehr.org/ckm/` — the Clinical Knowledge Manager archetype registry
- `https://discourse.openehr.org/` — the community forum

# Decision Log

**Purpose:** Record decisions that materially affect research questions, scope, evidence rules, methods, ethics, comparison, or gate outcomes. Routine editing does not require an entry.

## Entry template

Each new entry should record:

- decision ID and date;
- status: `PROPOSED`, `APPROVED`, `REVISED`, or `SUPERSEDED`;
- decision and decision owner;
- context and alternatives considered;
- evidence or constraint supporting the decision;
- consequences and affected files;
- review trigger.

Do not delete superseded decisions. Link the replacing entry.

## Decisions

### D-0001 — Minimal Phase 0A architecture

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Create only the core inception/gate documents and the minimum protocols/schemas needed to make Gate 0 auditable. Defer data, analysis, outputs, licensing, citation metadata, and automation structures.
- **Context:** The workspace was empty and only Phase 0A design was authorized.
- **Alternatives considered:** Creating the full provisional repository tree; keeping all protocols in one document.
- **Basis:** The project brief prohibits ornamental complexity but requires operational evidence, literature, language, decision, and case-screening controls.
- **Consequences:** The current repository has no `data`, `analysis`, `outputs`, or `reproducibility` directories. Create them only when an authorized workflow requires them.
- **Review trigger:** Owner review or authorization of Gate 0 evidence acquisition.

### D-0002 — Claim-specific evidence model

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Maintain a claim register separately from a claim-specific evidence register; one evidence row supports, qualifies, or challenges one claim.
- **Context:** A source may bear on several claims and a claim may depend on several sources.
- **Alternatives considered:** A single flat source list; a many-to-many link table.
- **Basis:** Separate claim and evidence states improve traceability without introducing a database or extra relational table at Gate 0 scale.
- **Consequences:** Reuse the same `source_id` across evidence rows when a source informs multiple claims. Do not duplicate source files.
- **Review trigger:** Volume or complexity makes the CSV model error-prone.

### D-0003 — Qualitative Gate 0 decision rule

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Use conjunctive evidence conditions and documented blocking failures for GO/MODIFY/NO-GO; do not use an aggregate numerical score.
- **Context:** A high score could conceal a decisive ethical, evidentiary, or competence failure.
- **Alternatives considered:** Weighted multi-criteria score.
- **Basis:** No empirical or theoretical basis currently justifies weights or compensation among dimensions.
- **Consequences:** A single unresolved critical condition can prevent GO.
- **Review trigger:** A validated decision model becomes available and is demonstrably appropriate.

### D-0004 — No CHALUS evidentiary dependency

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Exclude CHALUS findings from Gate 0 evidence and design the project to remain valid without them.
- **Context:** Owner-supplied status: GATE 2A-R CLOSED — NO-GO; EO BLOCKED; GATE 2B UNAUTHORIZED.
- **Basis:** Importing unauthorized or failed claims would violate evidence boundaries.
- **Consequences:** Accessibility is evaluated only through independently admissible evidence relevant to this project.
- **Review trigger:** A separately documented CHALUS authorization and a new relevance decision in this project.

### D-0005 — Conservation/governance primary framing

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Use heritage governance, conservation readiness, community safeguards, and sustainable destination planning as the primary analytical framing. Retain tourism and destination development only as applied domains.
- **Context:** Tourism terminology could otherwise reintroduce a growth assumption.
- **Basis:** Owner review and the development-before-growth principle.
- **Consequences:** The provisional question has been revised. The project must permit conclusions that tourism development should be delayed, constrained, redirected, or not prioritized.
- **Review trigger:** Gate 0 evidence shows the framing or tourism domain should be further narrowed or removed.

### D-0006 — Independent project status and bounded horizon

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Record the work as an independent research and professional portfolio project academically aligned with Tourism Destination Planning and Management in Spain. It is not an official UCM project, thesis/TFM, commissioned study, authority study, or institutionally endorsed work. Plan Gate 0 as a focused two- to three-week cycle, subordinate to methodological completion.
- **Context:** Academic alignment must not imply institutional authority or turn Gate 0 into an open-ended programme.
- **Consequences:** All project descriptions and later dissemination must preserve this disclaimer; calendar expiry cannot substitute for completion criteria.
- **Review trigger:** Formal institutional status or requirements change.

### D-0007 — Owner language capability and verification boundary

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Record native-level Persian review, advanced independent English research use, and advanced independent Spanish academic/professional use. Require authoritative linguistic/domain verification where consequential legal, archaeological, highly technical, or institution-specific meaning materially affects a claim.
- **Context:** Owner fluency supports research but is not universal specialist validation.
- **Consequences:** AI or informal translation cannot settle gate-critical technical meaning; affected claims must be constrained when verification is unavailable.
- **Review trigger:** A qualified verifier is appointed or a consequential ambiguity emerges.

### D-0008 — No privileged Iranian source access

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Assume access only to publicly and lawfully accessible institutional/government sources, public planning/policy documents, legitimate academic resources available to the researcher, public geospatial/open data, and other lawful sources.
- **Context:** No privileged access has been established.
- **Consequences:** Do not assume or seek unofficial access to unpublished archaeological records, restricted site databases, confidential government material, private institutional datasets, or protected coordinates. Evidence gaps remain visible.
- **Review trigger:** A documented lawful access arrangement is established and ethically reviewed.

### D-0009 — Eventual restricted public release

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Adopt **open methodology + selective responsible evidence publication** and retain eventual public release as an objective with restrictions.
- **Context:** Reproducibility and public value do not justify exposing vulnerable, private, restricted, or copyrighted material.
- **Consequences:** Methodology and permissible metadata/citations may be public; sensitive coordinates, unnecessary personal/contact data, restricted/private material, and copyrighted files without redistribution permission remain unpublished.
- **Review trigger:** Before repository publication or any public output.

### D-0010 — Positionality and funding disclosure

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Disclose that the owner is Iranian and studies tourism destination planning and management in Spain, creating useful contextual access and possible familiarity, national-comparison, transfer, and interpretation biases. Declare no current Kelardasht institutional affiliation and no funding.
- **Context:** The owner’s position is relevant to access and interpretation but cannot replace evidence.
- **Consequences:** Apply transparent evidence, contradiction, and decision controls; do not imply local representation or institutional authority.
- **Review trigger:** Affiliation, funding, role, or conflict status changes.

### D-0011 — Specialist review fallback

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Treat specialist review as desirable but not guaranteed and ensure Gate 0 is executable without it. If an indispensable specialist judgment cannot be reviewed, narrow, remove, defer the claim, or modify scope.
- **Context:** Archaeological, conservation, ecological, legal, transport-engineering, and other specialist claims may exceed owner competence.
- **Consequences:** Owner or AI inference cannot substitute for specialist expertise. Unavailable expertise blocks only claims that cannot be responsibly redesigned; it does not automatically block all Gate 0 work.
- **Review trigger:** A gate-critical specialist dependency is identified.

### D-0012 — Two-stage search pre-registration

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Freeze the search architecture before searching, permit a bounded and labelled terminology-calibration pilot, then document changes and freeze literal formal search strings before formal Gate 0 searching.
- **Context:** Freezing exact strings before learning cross-language indexing vocabulary would create avoidable search error.
- **Consequences:** Calibration and formal evidence sets remain distinguishable; calibration cannot silently change the protocol or enter synthesis. Every change is logged.
- **Review trigger:** Before calibration and again before formal search execution.

### D-0013 — Independent claim status and nature

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Maintain claim status (`VERIFIED`, `SUPPORTED`, `UNCERTAIN`, `UNVERIFIED`, `CONTRADICTED`) independently from claim nature (`OBSERVED`, `SOURCE_REPORTED`, `MODEL_DERIVED`, `INTERPRETED`, `HYPOTHETICAL`).
- **Context:** Verifying that an actor made a statement does not verify the truth of the statement’s content.
- **Consequences:** Material source-reported content is registered as a separate linked claim with its own status and evidence.
- **Review trigger:** The CSV structure no longer preserves this distinction reliably.

### D-0014 — Non-scoring Spanish case screen

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Retain eligibility, dimension-specific comparability, mechanism relevance, evidence availability, and explicit mismatch documentation without weighted ranking during initial screening.
- **Context:** No defensible basis currently exists for arbitrary weights or compensatory scores.
- **Consequences:** Quantitative weighting requires a later authorized methodological justification and cannot be introduced during Gate 0 initial screening.
- **Review trigger:** A later analytical need provides a defensible measurement model.

### D-0015 — Phase 0A baseline and phase boundary

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Treat the corrected package as the reviewed Phase 0A baseline while keeping Gate 0 evidence acquisition closed.
- **Context:** Owner review authorized corrections and baseline preparation, not research execution.
- **Consequences:** No evidence acquisition, substantive Kelardasht claim acceptance, Spanish case selection, CHALUS boundary change, or later-gate opening is authorized. The workspace was not already under Git, so the baseline remains uncommitted and no release/tag exists.
- **Review trigger:** Separate owner authorization for Gate 0 or placement of the baseline under version control.
- **Review outcome:** The baseline was subsequently committed as `4ac933fdad99c3cfd495e6c175c1e3d64b37f217`; D-0016 records the later limited Gate 0 authorization. The original decision remains part of the audit trail.

### D-0016 — Open Gate 0 for Stage A search-architecture design only

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Close Phase 0A as baselined at commit `4ac933fdad99c3cfd495e6c175c1e3d64b37f217`; open Gate 0 only for Stage A multilingual search-architecture design.
- **Context:** The authoritative pre-evidence design is versioned, but the search architecture requires owner review before any discovery activity.
- **Authorization boundary:** Evidence acquisition, source retrieval, calibration searching, formal searching, register population, substantive claim verification, literature screening, dataset acquisition, and Spanish case screening/selection remain unauthorized. Workstreams 0B, 0C, and other substantive evidence workstreams have not started.
- **Consequences:** Stage A may define domains, languages, terminology families, source environments, source-tier mappings, claim families, eligibility rules, temporal/geographic logic, a future calibration design, logging/change control, stopping rules, and ethical controls. It may not test those designs against external search results.
- **Review trigger:** Owner review of the completed Stage A architecture. No subsequent stage opens automatically.
- **Review outcome:** Owner approved Stage A subject to removal of fixed language quotas, an auditable query-execution definition, and a clarified calibration inspection boundary. D-0017 records the corrected freeze.

### D-0017 — Freeze Gate 0 Stage A search architecture

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Approve and freeze the corrected Gate 0 Stage A search architecture while keeping Stage B and all search execution closed.
- **Required corrections applied:** Retain a hard ceiling of 30 calibration query executions but allocate by Domain × Language relevance without language quotas; define one execution as one distinct query string in one environment under one retrieval-affecting filter/mode configuration; permit terminology-only inspection of metadata, titles, abstracts, keywords/index terms, official-page titles/headings, snippets, and landing-page terminology while prohibiting substantive extraction.
- **Redundancy control:** Make `literature/SEARCH_ARCHITECTURE.md` authoritative for search stages, calibration limits, execution counting, logging, and change control; replace the duplicated Stage A/B rules in `literature/SEARCH_PROTOCOL.md` with a cross-reference. Retain domain routing, terminology, ethical, and stopping detail because it is search-operational rather than duplicative of general Gate/source/language controls.
- **Authorization boundary:** No calibration, formal search, source retrieval, register population, claim verification, literature acquisition, data acquisition, or Spanish case screening/selection is authorized.
- **Review trigger:** Separate owner authorization to open Stage B. The 30-execution ceiling cannot be extended without separate authorization.

### D-0018 — Open Gate 0 Stage B bounded multilingual calibration

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Open Stage B solely for multilingual terminology, indexing, transliteration, database-behaviour, and search-environment calibration under a hard ceiling of 30 query executions.
- **Priority routing:** Allocate executions dynamically across the owner-specified Persian, English, and Spanish Domain × Language cells. Do not impose language quotas and do not search D12 independently unless encountered terminology creates a genuine specialist-vocabulary problem.
- **Inspection boundary:** Permit metadata, titles, abstracts, keywords/index terms, official-page titles/headings, result snippets, landing-page institutional terminology, and publication metadata solely for calibration. Prohibit full-text research, substantive extraction, corpus archiving, and findings.
- **Authorization boundary:** Formal evidence/literature acquisition, Kelardasht claim verification, substantive workstreams 0B/0C and later, Spanish case screening/selection, and formal search execution remain closed.
- **Outputs:** An execution-complete `literature/SEARCH_LOG.csv`, minimal non-evidentiary calibration leads only where necessary, and `literature/CALIBRATION_REPORT.md` for owner review. No commit is authorized.
- **Stop rule:** Stop at 30 executions, upon substantive drift, unlawful/restricted access, unnecessary sensitive-site exposure, required substantive-register population, or a material architecture redesign need.
- **Review trigger:** Owner review of Stage B outputs; no formal-search stage opens automatically.

### D-0019 — Approve and close Gate 0 Stage B calibration

- **Date:** 2026-09-25
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Accept the Stage B calibration as sufficient at 28 of the maximum 30 query executions, leave the remaining two executions intentionally unused, close Stage B as `CALIBRATION COMPLETE`, and keep Stage C unauthorized.
- **Terminology decisions:** Retain `CONSERVATION READINESS` and `ADAPTIVE POLICY / PRACTICE TRANSFER` as project analytical constructs while demoting literal `conservation readiness` and `adaptive transfer` as primary indexing phrases. Future domain-specific retrieval must use the approved established families and preserve their conceptual distinctions. Analytical/project language is not automatically database indexing language.
- **Native-environment limitation:** Stage B calibrated terminology and general-web retrieval behaviour, not native-interface syntax or coverage for untested SID, Magiran, Civilica, Noormags, Google Scholar, Crossref, Dialnet, Scopus, or Web of Science environments. Any later Stage C must classify each environment as `VERIFIED`, `CONDITIONAL_UNVERIFIED`, or `EXCLUDED`; exact executable queries cannot be operationally frozen for a `CONDITIONAL_UNVERIFIED` environment.
- **Lead status:** Preserve all six pointers as `CALIBRATION LEAD — NOT YET EVIDENCE`. No lead is promoted, assigned claim status, or entered into the claim, evidence, or literature registers. Stage C cannot silently promote them.
- **Traceability:** Calibration results and proposed changes are documented in `literature/CALIBRATION_REPORT.md`; this decision supplies owner approval; the resulting operational wording is versioned in `literature/SEARCH_ARCHITECTURE.md` and cross-referenced by `literature/SEARCH_PROTOCOL.md`.
- **Authorization boundary:** Further calibration, Stage C, formal search, formal evidence/literature acquisition, Kelardasht claim verification, substantive Gate 0 workstreams, and Spanish case screening/selection remain closed.
- **Review trigger:** Separate owner authorization is required to open Stage C; no later stage opens automatically.

### D-0020 — Open Gate 0 Stage C formal-search design

- **Date:** 2026-09-28
- **Status:** APPROVED
- **Decision owner:** Soroush Karahrodi
- **Decision:** Open Stage C solely to draft the formal-search plan, classify search environments, version exact executable queries where Stage B supports them, and define templates for environments whose native behaviour remains unverified.
- **Environment rule:** Use only `VERIFIED`, `CONDITIONAL_UNVERIFIED`, or `EXCLUDED`. General-web indexing cannot verify a native database. `FROZEN_EXECUTABLE` is allowed only for a `VERIFIED` environment; conditional environments receive templates without invented syntax.
- **Query rule:** Use modular domain-specific queries tied to Gate questions, language rationale, environment, source pathway, permitted filters, and version `1.0`. Every Stage C record has `execution_authorized=NO`.
- **Execution boundary:** New query executions, native-database tests, formal evidence/literature acquisition, source retrieval for substantive analysis, register/matrix population, citation chaining, claim verification, Spanish case screening, and substantive findings are prohibited.
- **Calibration boundary:** Preserve `CAL-001` through `CAL-028` unchanged; do not create `CAL-029`, `CAL-030`, or `FS-*` execution rows. The six calibration leads remain non-evidentiary and receive no preferential treatment.
- **Outputs:** `literature/FORMAL_SEARCH_PLAN.md`, `literature/SEARCH_ENVIRONMENTS.csv`, and `literature/FORMAL_QUERY_REGISTER.csv`, plus minimal status/cross-reference updates required for consistency. No commit is authorized.
- **Review trigger:** Owner review of the complete uncommitted Stage C package. Formal search execution requires separate authorization after an approved Stage C freeze.

### D-0021 — Approve and freeze Gate 0 Stage C formal-search architecture

- **Date:** 2026-09-28
- **Status:** APPROVED / FROZEN
- **Decision owner:** Soroush Karahrodi
- **Decision:** Approve the Stage C formal-search architecture subject to the execution-boundary audit, close Stage C as `FORMAL SEARCH ARCHITECTURE FROZEN`, and keep formal search execution and all substantive work unauthorized.
- **ENV-001 boundary:** Retain `ENV-001` as `VERIFIED` only for `BOUNDED DISCOVERY / SOURCE LOCATION`. It may locate official pages, difficult-to-index Persian materials, repositories, scholarly metadata or source landing pages, and underlying primary or academic sources. It is not evidence, an authority ranking, a reproducible bibliographic database, a prevalence measure, or a basis for inferring absence. Ranking, snippets, displayed counts, autogenerated summaries, and ordering are non-evidentiary; provider/version identity is not exposed and ranking behaviour is opaque.
- **Query audit:** Retain 59 records: 40 `FROZEN_EXECUTABLE`, 17 `TEMPLATE_PENDING_ENVIRONMENT_VERIFICATION`, and 2 `EXCLUDED`. Every frozen query points to `ENV-001`; no conditional environment is represented as executable. The audit found no functionally redundant record requiring merger/removal and no environment-limit status change.
- **Execution order:** Assign 30 records to `P1 — CORE`, 25 to `P2 — CONDITIONAL SUPPORT`, 2 to `P3 — CONTINGENT`, and 2 excluded records to `NA`. Priority governs bounded execution planning, not source quality or finding rank. Query count is not an execution target; future authorization must begin with applicable executable P1 records and expand only for documented decision-relevant need.
- **Frozen-query meaning:** `FROZEN_EXECUTABLE` means only that the methodologically frozen query may be considered for later execution after separate owner approval. It does not establish yield, relevance, evidence status, source authority, or proof/disproof.
- **Screening clarification:** `BLOCKED_ACCESS` and `SPECIALIST_REVIEW_REQUIRED` are flags or conditions, not evidence against a source or claim and not exclusion reasons.
- **Validation boundary:** No new or formal search occurred; `CAL-029`, `CAL-030`, and `FS-*` execution rows remain absent; substantive registers and the six calibration leads remain unchanged and non-evidentiary; no Spanish case, Kelardasht claim, CHALUS boundary, or later gate was opened.
- **Authorization boundary:** Formal search execution, evidence/literature acquisition, Kelardasht claim verification, Spanish case screening, and all later Gate 0 substantive work remain unauthorized until a separate owner decision.

### D-0022 — Verify Cloud web-search surface as an execution profile of ENV-001 before D1A

- **Date:** 2026-09-28
- **Status:** APPROVED (verification microstage) — outcome: `PARTIAL_VERIFICATION`
- **Decision owner:** Soroush Karahrodi
- **Decision:** Authorize a bounded, non-research environment-fidelity microstage to test whether the AI-mediated web-search tool in this Claude Code cloud session can be accepted as a verified execution surface profile (`ENV-001-SURFACE-CLOUD-01`) of the existing `ENV-001` class, before any D1A formal execution. Do not manually execute the 12 P1 searches; do not create a new environment (`ENV-017`); test the surface instead.
- **Context:** The first D1A attempt correctly STOPPED before any formal search because the only available surface is AI-mediated and was not the browser-based surface Stage B verified. Rather than reopen D1A or immediately create a new environment, the owner directed a surface/interface verification against the existing ENV-001 class.
- **Why manual execution was not the chosen workflow:** The owner elected to test the available cloud surface first, reserving manual/browser execution as a fallback decided only after the surface's fidelity is known.
- **Why a surface profile rather than a new environment:** `ENV-001` already documents provider/version opacity and non-evidentiary ranking/snippets; the cloud tool is another general-web execution surface, so it was tested as a profile within ENV-001 rather than promoted to a distinct environment. A new environment would only be created if the tool proved methodologically different rather than another general-web surface.
- **Method:** Six executions in a separate temporary `EV-*` namespace (ceiling 6), logged in `literature/ENVIRONMENT_VERIFICATION_LOG.csv`, testing English quoted-vs-unquoted behaviour, two Persian ZWNJ/half-space vs ordinary-space pairs, and URL traceability. No source read substantively; the tool's AI summaries were ignored.
- **Verification result (`PARTIAL_VERIFICATION`):** Input strings are auditable. The exact-phrase quotation operator is **not** honored (identical quoted/unquoted link sets, non-phrase hits returned). Persian ZWNJ vs ordinary-space inputs produce observably different, loggable outputs, but faithful phrase-level half-space matching cannot be confirmed because quoting fails. Returned URLs/domains are traceable. Provider identity is opaque and the tool is US-region-only. Full detail in `literature/ENVIRONMENT_VERIFICATION_REPORT.md`.
- **Methodological consequence:** The surface is usable only as a locator layer for token-based bounded discovery. Of the 12 authorized D1A P1 candidates, only the 4 bare-token Persian queries (`FQ-D2-001`, `FQ-D3-001`, `FQ-D3-002`, `FQ-D11-001`) would run without a silent semantic change; the other 8 depend on exact-phrase quoting and/or material half-space pairing and are proposed as `BLOCKED_FOR_SURFACE_FIDELITY` pending owner decision. This mapping is advisory only; `FORMAL_QUERY_REGISTER.csv` and `SEARCH_ENVIRONMENTS.csv` are unchanged and `ENV-001`'s frozen status is unchanged (a partial result is not a pass and promotes nothing).
- **Consequences and affected files:** New `literature/ENVIRONMENT_VERIFICATION_REPORT.md` and `literature/ENVIRONMENT_VERIFICATION_LOG.csv`; this decision entry; minimal status notes in `README.md` and `docs/gates/GATE_0_PROTOCOL.md`. Protected registers, `SEARCH_LOG.csv`, `FORMAL_QUERY_REGISTER.csv`, `SEARCH_ENVIRONMENTS.csv`, the six calibration leads, and the CHALUS boundary are unchanged.
- **Authorization boundary:** D1A remains unauthorized (`HALTED BEFORE EXECUTION — ENVIRONMENT VERIFICATION REQUIRED`). Formal search execution, evidence/literature acquisition, Kelardasht claim verification, and Spanish case screening remain unauthorized. Resuming D1A requires a separate owner decision that specifies the authorized query classes and surface.
- **Review trigger:** Owner review of this verification microstage and an explicit decision on whether to run the compatible subset on `ENV-001-SURFACE-CLOUD-01`, obtain a verified browser surface for the phrase-dependent queries, or hold.

### D-0023 — Authorize Cloud-compatible D1A P1 pilot subset

- **Date:** 2026-09-28
- **Status:** APPROVED (bounded pilot substage `D1A-P`) — this is **not** D1A completion
- **Decision owner:** Soroush Karahrodi
- **Decision:** Authorize a narrowly bounded pilot execution of **only** the four P1 queries that D-0022 showed to be compatible with the Cloud surface — `FQ-D2-001`, `FQ-D3-001`, `FQ-D3-002`, `FQ-D11-001` — on `ENV-001-SURFACE-CLOUD-01`, using formal execution IDs `FS-001`–`FS-004` (one per query). The pilot tests the retrieval-and-metadata-screening **pipeline**, not the research questions.
- **D-0022 basis (`PARTIAL_VERIFICATION`):** The Cloud surface is usable **only as a locator layer** for token-based bounded discovery. It does not reliably honor exact-phrase quoting and does not verify phrase-level half-space semantics. Provider/version is opaque; the surface is US-region-only; ranking, snippets, displayed counts, and AI summaries are non-evidentiary.
- **Authorized query subset:** Only the four bare-token Persian queries above. Each was confirmed in `FORMAL_QUERY_REGISTER.csv` as `execution_priority = P1 — CORE`, `query_status = FROZEN_EXECUTABLE`, `environment_id = ENV-001`. Query strings were retrieved verbatim from the register and executed unaltered.
- **Blocked (remain `BLOCKED_FOR_SURFACE_FIDELITY`, not executed):** `FQ-D1-001`, `FQ-D1-002`, `FQ-D1-003`, `FQ-D1-004`, `FQ-D1-007`, `FQ-D2-002`, `FQ-D2-004`, `FQ-D4-001` — these depend on exact-phrase quoting and/or material half-space pairing. They were not executed, repaired, rewritten, or moved to another environment. Site-domain (`site:`) fidelity remains untested and is not required for this four-query subset.
- **Frozen-text observation (no change made):** `FQ-D2-001` contains a doubled token (`موزه موزه`). It was executed verbatim per this authorization; the query text and version are unchanged. Recorded as an observation only; any correction requires a separate future versioned decision.
- **Boundary preserved:** Evidence acquisition, full-source substantive review, claim verification, literature synthesis, Spanish case screening, and the Gate 0 verdict remain **NOT AUTHORIZED**. Stage D1A remains **incomplete**; only substage `D1A-P` was opened.
- **Consequences and affected files:** New `literature/FORMAL_RETRIEVAL_REGISTER.csv` (36 inspected records, `RET-0001`–`RET-0036`; all screening states non-acceptance) and `literature/D1A_CLOUD_PILOT_REPORT.md`; four `FS-*` rows appended to `literature/SEARCH_LOG.csv`; this decision entry; minimal status notes in `README.md` and `docs/gates/GATE_0_PROTOCOL.md`. Protected registers (`CLAIM_REGISTER.csv`, `EVIDENCE_REGISTER.csv`, `LITERATURE_MATRIX.csv`, `CASE_SCREENING.csv`, `CALIBRATION_LEADS.csv`), `FORMAL_QUERY_REGISTER.csv`, `SEARCH_ENVIRONMENTS.csv`, the calibration records (`CAL-001`–`CAL-028`), the `EV-*` verification records, and the CHALUS boundary are unchanged. No `CAL-029`/`CAL-030` and no evidence/claim/literature/Spanish-case rows were created.
- **Fidelity limitation recorded:** The retrieval register is an AI-surfaced **locator log**, not a bibliographic record. Only directly observed locator fields (retrieval/search/query IDs, surface profile, domain, language, result position, returned title, URL, host) are populated; author, publication date, source type, and temporal scope are marked `NOT_CAPTURED`; access status is `NOT_VERIFIED`; source tier is `TIER_UNRESOLVED` for every row (source authority is **not** inferred from domain alone); geographic scope is set only where the returned title itself states a locality, otherwise `UNRESOLVED`. Only exact-URL identity counts as a confirmed `DUPLICATE`; a same/near-identical headline on a different host is recorded as a possible cross-host duplicate with lineage unverified. Locator provenance (title/URL/host) is recoverable; source authentication / bibliographic provenance is **NOT YET VERIFIED**. Every retained row requires independent re-verification (preferably on a browser surface) before any evidentiary use. (Wording aligned with the PR #2 metadata-safeguard correction; the authorization scope is unchanged.)
- **Review trigger:** Owner review of the `D1A-P` pilot report and an explicit decision on whether to (a) continue compatible P1 retrieval on this surface, (b) obtain a verified browser surface for the eight blocked phrase-dependent P1 queries, or (c) redesign. No later stage opens automatically.

### D-0024 — Verify DuckDuckGo HTML browser surface for phrase-sensitive ENV-001 execution

- **Date:** 2026-09-28
- **Status:** APPROVED (browser-surface fidelity verification microstage) — outcome: `PASS` (method-bound)
- **Decision owner:** Soroush Karahrodi
- **Authoritative base commit:** `92e82e77f4f52248b74c591e77fde932b40cf05c`
- **Decision:** Record an already-completed browser-surface fidelity verification establishing that a real, visible DuckDuckGo HTML search surface (`https://html.duckduckgo.com/html/`, driven through Chrome via Claude in Chrome) faithfully preserves and materially honours the exact-phrase quotation and Persian ZWNJ/half-space behaviours required by eight phrase-dependent P1 queries. The verified execution surface profile is labelled `ENV-001-SURFACE-DDG-HTML-01`, a profile within the frozen `ENV-001` class — **not** a new environment. This task does **not** execute any formal search and does **not** reopen D1A.
- **Provenance (recorded honestly):** The seven browser tests (`BEV-001`–`BEV-007`) were executed and observed by the owner in Claude in Chrome and transcribed into this record. This Codex session did **not** run them and cannot independently verify them; they are recorded as **owner-attested browser-handoff observations**, mirroring how D-0022 quarantined its `EV-*` work. No `BEV-*` execution was performed in this session (`new BEV executions performed in Codex = 0`).
- **Why browser verification was required:** D-0022 (`PARTIAL_VERIFICATION`) showed the AI-mediated cloud surface does **not** honour the exact-phrase quotation operator, leaving eight P1 queries `BLOCKED_FOR_SURFACE_FIDELITY` (`FQ-D1-001`, `FQ-D1-002`, `FQ-D1-003`, `FQ-D1-004`, `FQ-D1-007`, `FQ-D2-002`, `FQ-D2-004`, `FQ-D4-001`). Completing D1A across the full P1 set required a surface that honours quote and spacing semantics.
- **Why DuckDuckGo HTML was selected:** the `html.duckduckgo.com/html/` endpoint is a real, non-JavaScript search surface whose submitted query is inspectable in a visible box and whose result links carry a directly decodable destination URL in the `uddg` redirect parameter, enabling auditable query fidelity and title/URL/host/path recovery without depending on a JavaScript-rendered interface.
- **Why controlled URL encoding was used:** to make the exact submitted query bytes auditable and to encode U+200C explicitly for ZWNJ-sensitive strings, then confirm via the visible search box that the submitted string survived intact. This is part of the verified surface profile and is the input method the PASS is bound to.
- **BEV result:** `BEV-001` quoted `"Kelar Dasht"` — quotes preserved, no rewrite, 4 links. `BEV-002` unquoted control — 10 links, materially broader (quotation materially changed retrieval). `BEV-003` `"کارگاه‌موزه"` (U+200C) — ZWNJ preserved, codepoint hex `200c`, 0 results (not interpreted substantively). `BEV-004` `"کارگاه موزه"` (U+0020) — hex `20`, 2 results (ZWNJ vs space distinction observable and material). `BEV-005` `"باستان‌شناسی"` (U+200C) — hex `200c`, 8 results. `BEV-006` `"باستان شناسی"` (U+0020) — hex `20`, 6 results, ordering differed. `BEV-007` `site:mcth.ir کلاردشت` — preserved verbatim, 10 links, all hosts within `*.mcth.ir` (site constraint materially respected). URL traceability `PASS` via `uddg`. Full detail in `literature/BROWSER_SURFACE_VERIFICATION_REPORT.md` and `literature/BROWSER_SURFACE_VERIFICATION_LOG.csv`.
- **Classification (`PASS`, method-bound):** exact submitted query string auditable; quotation marks preserved; quotation semantics materially functional; Persian ZWNJ preserved; ZWNJ-vs-ordinary-space distinction materially observable; site-domain constraint functional; real destination URLs traceable; no observed silent AI query rewrite. The PASS certifies `ENV-001-SURFACE-DDG-HTML-01` **only when queries are delivered by the same controlled URL-encoding method verified here**; hand-typed or other delivery paths are unverified until separately re-tested.
- **Exact eight query IDs now surface-compatible (subject to separate authorization):** `FQ-D1-001`, `FQ-D1-002`, `FQ-D1-003`, `FQ-D1-004`, `FQ-D1-007`, `FQ-D2-002`, `FQ-D2-004`, `FQ-D4-001`. For these, no surface-fidelity reason remains blocked. This does not establish evidence, source authority, yield, D1A completion, or claim support.
- **Formal execution still unauthorized:** the eight queries were not executed, repaired, rewritten, or moved. Formal execution requires a separate owner decision (`D-0025` or equivalent). D1A remains **INCOMPLETE**.
- **SEARCH_ENVIRONMENTS decision:** `literature/SEARCH_ENVIRONMENTS.csv` is left **unchanged**. Forcing an additional verified-surface profile into the frozen `ENV-001` row would overload and distort the frozen Stage C record; consistent with D-0022, the surface profile is recorded only in this decision, the report, and the log. `ENV-001`'s frozen status and scientific meaning are preserved.
- **Consequences and affected files:** New `literature/BROWSER_SURFACE_VERIFICATION_REPORT.md` and `literature/BROWSER_SURFACE_VERIFICATION_LOG.csv`; this decision entry; minimal status notes in `README.md` and `docs/gates/GATE_0_PROTOCOL.md`. Protected registers (`CLAIM_REGISTER.csv`, `EVIDENCE_REGISTER.csv`, `LITERATURE_MATRIX.csv`, `CASE_SCREENING.csv`, `CALIBRATION_LEADS.csv`, `FORMAL_RETRIEVAL_REGISTER.csv`, `SEARCH_LOG.csv`), `FORMAL_QUERY_REGISTER.csv`, `SEARCH_ENVIRONMENTS.csv`, the calibration records (`CAL-001`–`CAL-028`), the `EV-*` and `FS-*` records, and the CHALUS boundary are unchanged. No new `FS-*`, `CAL-*`, evidence, claim, literature, or Spanish-case rows were created; no formal search was executed.
- **Review trigger:** Owner review of this verification record and an explicit decision on whether to authorize D1A-B execution of the eight surface-compatible P1 queries on `ENV-001-SURFACE-DDG-HTML-01`. No later stage opens automatically.

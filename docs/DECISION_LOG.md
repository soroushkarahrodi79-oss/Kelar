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

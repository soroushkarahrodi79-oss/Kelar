# Source, Claim, and Evidence Protocol

**Status:** Owner-approved Phase 0A baseline; evidence acquisition remains unauthorized  
**Applies to:** Gate 0 claim verification, literature landscape, data feasibility, and case screening

## 1. Data model

- A **claim** is a bounded proposition that can be supported, qualified, contradicted, or left unresolved.
- A **source** is an identifiable document, dataset, record, or original research object.
- An **evidence item** is a claim-specific excerpt, datum, or documented observation extracted from a source.

`CLAIM_REGISTER.csv` stores one row per material claim. `EVIDENCE_REGISTER.csv` stores one row per claim-specific evidence item. A source used for several claims may recur with the same `source_id`; this is deliberate and does not make repeated use independent corroboration.

## 2. Source hierarchy

| Tier | Class | Examples | Default use and caution |
|---|---|---|---|
| `A` | Primary authoritative evidence | Legislation, adopted plans, official heritage registers, official statistics, original archaeological documentation, primary spatial data, signed/issued technical records | Best for formal status and recorded facts within institutional remit; does not automatically prove implementation, effectiveness, accuracy, or independence. |
| `B` | Peer-reviewed academic evidence | Journal articles, scholarly books, reviewed archaeological studies | Best for methods, interpretation, and scholarly debate; assess date, method, data, disciplinary limits, and conflicts. |
| `C` | High-quality institutional/technical evidence | Universities, international organizations, established heritage/professional bodies, documented technical reports | Useful where methods, authorship, and provenance are clear; assess mandate and review status. |
| `D` | Credible secondary reporting | Reputable reporting with attributable sources and editorial controls | Useful for discovery, chronology, and corroboration; trace decisive claims to primary evidence when possible. |
| `E` | Promotional or weak evidence | Destination promotion, press releases without supporting records, unattributed web pages, social media, advocacy material | Leads and evidence of public representation only; insufficient alone for gate-critical factual claims. |

Tier describes source class, not automatic truth. Record conflicts, institutional interests, circular citation, and whether several items derive from one underlying source.

## 3. Claim status

Use exactly one current status in the claim register:

- `VERIFIED` — direct, fit-for-purpose, authoritative evidence establishes the bounded claim and no material unresolved contradiction is known.
- `SUPPORTED` — credible evidence supports the claim, but directness, coverage, independence, or authority is incomplete.
- `UNCERTAIN` — mixed, ambiguous, translated-but-unverified, temporally mismatched, or incomplete evidence prevents a stable conclusion.
- `UNVERIFIED` — the claim has been identified but no adequate evidence establishes it; this does not mean false.
- `CONTRADICTED` — fit-for-purpose evidence materially conflicts with the claim. State whether fully or partly contradicted in limitations.

Status is claim-specific and time-bounded. It must change when material evidence changes, with reviewer/date recorded. `VERIFIED` is not permanent.

## 4. Claim nature

Claim status and claim nature are independent dimensions. Use one primary nature and note any secondary nature:

- `OBSERVED` — directly recorded through an authorized, documented research procedure.
- `SOURCE_REPORTED` — reported by an identifiable source.
- `MODEL_DERIVED` — calculated or inferred through a specified reproducible model.
- `INTERPRETED` — researcher synthesis or conceptual judgment.
- `HYPOTHETICAL` — proposition posed for testing, not asserted as fact.

AI-generated text is none of these and cannot be an evidentiary nature or source. AI may help process a source, but the evidence remains the source or the documented original analysis.

For `SOURCE_REPORTED` claims, distinguish the occurrence of a statement from the truth of its contents. Adequate evidence may verify the bounded claim **“Institution/person X stated Y on date Z.”** It does not thereby verify **Y**. When Y is material, create a separate linked claim with its own status and evidence set using `reported_content_claim_id`. This rule applies especially to official announcements, promotional claims, heritage-significance statements, funding claims, and tourism-development assertions.

## 5. Evidence relation and strength

For each evidence item record whether it `SUPPORTS`, `QUALIFIES`, `CONTRADICTS`, or provides `CONTEXT_ONLY` for its linked claim.

Evidence strength is a reasoned, claim-specific judgment:

- `DIRECT_STRONG` — direct, authoritative/fit-for-purpose, traceable, and temporally appropriate.
- `DIRECT_LIMITED` — direct but incomplete, dated, narrow, or otherwise constrained.
- `INDIRECT_CORROBORATIVE` — independently supports part of the inference.
- `WEAK_LEAD` — useful for discovery or public-representation analysis, not conclusion.
- `NOT_ASSESSABLE` — authenticity, meaning, access, or fitness cannot yet be judged.

Do not convert these categories into scores or average them.

## 6. Registration procedure

1. Define the claim narrowly enough to test; assign `CLM-G0-####`. For a source-reported statement, specify whether the claim concerns the fact that the statement was made or the factual content asserted.
2. Mark whether it is gate-critical and record what would falsify or materially qualify it.
3. Locate a source and authenticate title, author/institution, date/version, stable identifier, and provenance.
4. Assign source tier and type; record source language, access/licensing, and sensitivity.
5. Extract only the relevant passage/data with a precise locator. Preserve original text.
6. Add translation and/or paraphrase under the language protocol without overwriting the original.
7. Describe relation, strength, limitations, and source dependencies.
8. Search for contradiction, later versions, non-implementation evidence, and independent corroboration.
9. Update claim status only after reviewing the evidence set, documenting reviewer and date.
10. Archive lawfully where permitted; otherwise store a citation/identifier and access note, not an unauthorized copy.

## 7. Initiative-status claims

Record the highest directly evidenced status using the controlled categories in the Gate 0 protocol. Do not infer implementation from plans, funding from announcements, operation from institution names, or outcomes from implementation. Record the responsible entity, dates, legal/administrative basis, funding status, implementation evidence, operational evidence, and outcome evidence separately.

## 8. Independence and triangulation

- Syndicated reports, copied press releases, and documents citing the same underlying record count as one evidence lineage.
- Institutional sources can be authoritative about formal acts but self-interested regarding performance.
- Two weak sources do not become strong solely through agreement.
- Triangulation should cross evidence types or independent lineages where the claim warrants it.
- Record conflicting evidence rather than selecting the preferred account silently.

## 9. Missing and negative evidence

“No evidence found” is a result of a defined search, not proof of nonexistence. Any absence statement must identify repositories/sources searched, languages and terms, date of search, coverage limits, and plausible inaccessible records. Use `UNVERIFIED` or `UNCERTAIN` unless the source universe is sufficiently complete to justify a stronger claim.

## 10. Sensitive and restricted evidence

Do not place exact vulnerable-site coordinates, personal data, confidential material, or restricted source files in these CSVs or the versioned repository. Use a generalized location, sensitivity label, and controlled external reference. Record access and redistribution restrictions. If the claim does not require exact location, do not collect it.

## 11. Minimum quality review

Before an evidence item can affect a gate verdict, a reviewer must check:

- source identity and version;
- locator and faithful extraction;
- tier/type rationale;
- language and translation status;
- temporal and geographic fit;
- evidence lineage/independence;
- claim relation and limitations;
- sensitivity/licensing;
- whether a qualified specialist is required.

The owner may self-review routine items, but gate-critical items with material translation or specialist uncertainty require the review specified in the Gate 0 protocol.

## 12. CSV conventions

- UTF-8 encoding; ISO dates (`YYYY-MM-DD`) where known.
- Use controlled vocabulary exactly as specified; multiple values are pipe-separated.
- Use stable IDs; never recycle deleted IDs.
- Use blank for not yet entered and `NOT_APPLICABLE` only when genuinely inapplicable.
- Do not place line breaks inside fields unless the CSV tool reliably preserves them.
- Formula-like source text beginning with `=`, `+`, `-`, or `@` must be escaped when opened in spreadsheet software to prevent formula injection.

# ENV-001 Cloud Search-Surface Verification Report

**Status:** COMPLETE — CLASSIFICATION: `PARTIAL_VERIFICATION`
**Microstage:** ENV-001 CLOUD SURFACE VERIFICATION ONLY (change-control microstage before D1A)
**Authorization:** Owner instruction of 2026-09-28; recorded as Decision `D-0022`
**Date:** 2026-09-28
**Authoritative base commit:** `4abfda9fb1d5e860c0a34bfb2b9d5b1d8767de51` (Stage C)
**Working branch:** `gate0/env001-cloud-surface-verification`
**Candidate surface profile:** `ENV-001-SURFACE-CLOUD-01`
**Scope note:** This is an interface/surface fidelity test, not research. No source was read substantively; no evidence, claim, literature, retrieval, or Spanish-case record was produced. D1A remains unauthorized after this report regardless of outcome.

## 1. Authorization and boundary

This microstage was authorized by the owner solely to determine whether the AI-mediated web-search tool available in this Claude Code cloud session is sufficiently faithful to the search behaviours required by `ENV-001` (the frozen "Mainstream general-web search" environment class) to execute frozen formal queries **without silently changing their semantics**.

It does **not** reopen D1A, promote any environment, create a new environment (`ENV-017` was explicitly not created), alter any frozen query, or authorize any formal or evidence search. The prior D1A attempt correctly stopped before any formal execution; that state is preserved.

## 2. Environment interpretation

- `ENV-001` is treated as the **environment class** ("Mainstream general-web search"; authorized role `BOUNDED DISCOVERY / SOURCE LOCATION`).
- The current cloud search implementation is treated as a candidate **execution surface profile** within that class, labelled `ENV-001-SURFACE-CLOUD-01`.
- This is a profile identifier only. Whether it is admissible as an ENV-001 execution surface is the question under test; the answer here is *partial*.

## 3. Tool / interface description

- **Interface:** `WebSearch` tool exposed inside this Claude Code cloud session (AI-assistant-mediated web search). Input is a single query string that the researcher controls verbatim; output is a ranked list of result blocks (title + URL) followed by an auto-generated natural-language summary.
- **Provider identity exposed:** **NO.** The tool does not disclose the underlying search provider or version. This is consistent with `ENV-001`'s already-documented reproducibility limit (provider/version opacity), but it means browser/provider reproducibility of the Stage B human surface **cannot** be claimed for this profile.
- **Region:** The tool self-reports as **US-region-only**. This is a material locator limitation for Iranian/Persian and Spanish content and was not a property of the Stage B calibration surface as documented.
- **AI layer:** Every response includes an AI-generated summary containing substantive prose. This summary is **not required** for metadata screening — only the returned `title`/`url` link list is needed — and it was ignored throughout this microstage. Its presence is itself a caveat: the surface interposes a generative layer over raw ranking.

## 4. Verification executions

Six verification executions were run in the temporary `EV-*` namespace (ceiling: 6; used: 6). These are environment tests — **not** `CAL-*` calibration and **not** `FS-*` formal executions. Full per-execution detail is in `literature/ENVIRONMENT_VERIFICATION_LOG.csv`.

| ID | Test | Exact input | Result |
|---|---|---|---|
| EV-001 | English quoted phrase | `"Kelar Dasht"` | Quote not honored |
| EV-002 | English unquoted control | `Kelar Dasht` | Identical link set to EV-001 |
| EV-003 | Persian ZWNJ quoted | `"کارگاه‌موزه" کلاردشت` | Differs from EV-004 (observable, phrase unverified) |
| EV-004 | Persian ordinary-space quoted | `"کارگاه موزه" کلاردشت` | Differs from EV-003 |
| EV-005 | Persian ZWNJ quoted | `"باستان‌شناسی" کلاردشت` | Differs from EV-006 (observable, phrase unverified) |
| EV-006 | Persian ordinary-space quoted | `"باستان شناسی" کلاردشت` | Differs from EV-005 |

TEST E (site-domain operator, e.g. `site:datos.gob.es`) was **not tested**: the owner instruction ruled it optional for the immediate D1A batch and directed that it not displace the priority Persian fidelity tests. It remains an open item.

## 5. Fidelity findings

### 5.1 Input fidelity — PASS (auditable)
The exact query string submitted to the tool is fully under the researcher's control and is therefore auditable and reconstructable. What the *underlying provider* then does with that string is the limiting factor below.

### 5.2 Quoted-phrase behaviour — FAIL
EV-001 (`"Kelar Dasht"`) and EV-002 (`Kelar Dasht`) returned an **identical link set in identical order**, and that set contained results that do not contain the phrase at all (e.g. "Dasht", "Dasht Konar", "Dashti, Isfahan"). The exact-phrase quotation operator is therefore **not materially respected** on this surface. This matters because most frozen queries in `FORMAL_QUERY_REGISTER.csv` rely on `"..."` exact-phrase segments.

### 5.3 Persian ZWNJ / half-space behaviour — OBSERVABLE, PHRASE-UNVERIFIED
For both tested pairs (EV-003/EV-004 and EV-005/EV-006), the half-space (U+200C) and ordinary-space inputs produced **different** link sets with only partial overlap. This shows the byte-distinct inputs are transmitted, not silently collapsed to one identical result, so the distinction is **loggable**. However, because the quote operator fails (5.2), the tool **cannot confirm faithful phrase-level half-space matching** — the observed differences may reflect loose tokenization rather than the spacing-sensitive phrase retrieval Stage B relied on. Under the owner's pass criteria this satisfies condition 3(b) (transparently observable and loggable) but **not** condition 3(a) (preserved sufficiently).

### 5.4 Source-URL traceability — PASS
Returned records carry concrete, dereferenceable URLs and identifiable domains (e.g. `fa.wikipedia.org`, `mehrnews.com`, `irib-news.ir`, `tripadvisor.com`), sufficient to support later metadata screening and underlying-source identification.

### 5.5 Site-domain operator — NOT TESTED
Deferred within the six-execution ceiling; open item for a later authorized check if D11 site-constrained queries are to be run on this surface.

### 5.6 AI reranking / summarization — CAVEAT, IGNORABLE
The surface always injects an AI summary. It is not needed for locator use (the link list suffices) and was ignored here, satisfying pass condition 6. Its existence nonetheless distinguishes this surface from a plain browser search and must never be logged or treated as a source.

## 6. Classification

**`PARTIAL_VERIFICATION`.**

The cloud surface is usable strictly as a **locator layer for token-based bounded discovery**, where retrieval does not depend on exact-phrase quoting or on methodologically material half-space-vs-space *phrase* precision, and where returned URLs/domains are the object of interest. It is **not** verified for queries whose semantics depend on the quotation operator or on spacing-sensitive phrase matching.

Provider opacity and US-region restriction are recorded limitations. Honest logging of any future execution on this surface must state the profile `ENV-001-SURFACE-CLOUD-01`, must not claim browser/provider reproducibility, and must record that exact-phrase and half-space phrase semantics are unverified.

## 7. Consequences for the frozen D1A P1 batch (proposed mapping — for owner review only)

This mapping is advisory. It is **not** written into `FORMAL_QUERY_REGISTER.csv`; no `execution_authorized` value is changed and no query text or version is altered.

**Compatible with the verified surface (token-based discovery; no quote/spacing dependence):**
- `FQ-D2-001` — bare tokens, no quotation operator.
- `FQ-D3-001` — bare tokens, no quotation operator.
- `FQ-D3-002` — bare tokens, no quotation operator.
- `FQ-D11-001` — bare tokens, no quotation operator.

**Unsafe on this surface (`BLOCKED_FOR_SURFACE_FIDELITY`) — depend on exact-phrase quoting and/or material half-space pairing:**
- `FQ-D1-001` (`"محوطه باستانی"` + `باستان‌شناسی` half-space; pairs with FQ-D1-007).
- `FQ-D1-007` (`"باستان شناسی"` + `"محوطه باستانی"`; ordinary-space member of the pair).
- `FQ-D1-002` (`"میراث فرهنگی"` + `"آثار تاریخی"` exact phrases).
- `FQ-D2-002` (`"کارگاه‌موزه"` half-space; pairs with FQ-D2-004).
- `FQ-D2-004` (`"کارگاه موزه"` ordinary space; ordinary-space member of the pair).
- `FQ-D1-003` (`"archaeological heritage"` exact phrase) — token discovery works, exact-phrase precision does not.
- `FQ-D1-004` (`"Kelar Dasht"` exact phrase) — directly shown non-functional as a phrase in EV-001.
- `FQ-D4-001` (`"Western Mazandaran"` exact phrase) — phrase precision unverified.

Interpretation: of the 12 authorized P1 candidates, only 4 (the bare-token Persian discovery queries) would run on this surface without a silent semantic change. The remaining 8 depend on quote and/or spacing semantics this surface does not honor. The owner must decide whether to (a) run only the compatible subset with the limitations logged, (b) obtain a verified browser surface for the phrase-dependent queries, or (c) not proceed.

## 8. Limitations of this verification

1. Non-determinism: a single execution per input cannot fully separate provider ranking instability from genuine input-sensitivity, though the identical EV-001/EV-002 pair is strong evidence for quote-insensitivity.
2. The underlying provider's query interpretation is not exposed; findings are inferred from returned link sets only.
3. Site-domain operator behaviour was not tested.
4. Arabic/Persian character-substitution behaviour (ي/ی, ك/ک) was not tested and remains, per Stage B, platform-specific.
5. US-region restriction may affect which Iranian/Spanish sources are reachable at all; this was observed as a surface property, not quantified.

## 9. Decision consequence

- `ENV-001`'s frozen Stage C record and status are **unchanged**: `PARTIAL_VERIFICATION` is not a pass and does not promote a new surface into the frozen registry. `SEARCH_ENVIRONMENTS.csv` is intentionally left untouched by this microstage.
- The surface profile `ENV-001-SURFACE-CLOUD-01` and its compatible/unsafe query classes are recorded here and in `docs/DECISION_LOG.md` (D-0022) for owner review.
- D1A remains **HALTED BEFORE EXECUTION — ENVIRONMENT VERIFICATION REQUIRED**. A separate owner authorization is required to resume it, and any resumption must specify which query classes and which surface are authorized.

## 10. Boundary validation

- Formal searches executed: 0
- `FS-*` rows added: 0
- `EV-*` verification executions: 6 (ceiling 6)
- `CAL-029` / `CAL-030`: absent
- Evidence-register rows added: 0
- Claim-register rows added: 0
- Literature-matrix rows added: 0
- Formal-retrieval rows added: 0
- Spanish-case rows added: 0
- Substantive findings retained: 0
- Frozen formal query text changed: NO
- Query versions changed: NO
- Environment IDs changed: NO
- CHALUS boundary changed: NO
- D1A resumed: NO

# DuckDuckGo HTML Browser-Surface Verification Report

**Status:** COMPLETE — CLASSIFICATION: `PASS` (method-bound; see §5 and §10)
**Microstage:** ENV-001 DuckDuckGo HTML browser-surface fidelity verification (change-control microstage; **not** a formal search)
**Authorization:** Owner instruction of 2026-09-28; recorded as Decision `D-0024`
**Date:** 2026-09-28
**Authoritative base commit:** `92e82e77f4f52248b74c591e77fde932b40cf05c` (current reviewed `main`)
**Working branch:** `claude/ddg-html-browser-verification-63hu2g` (session-mandated; the prompt's preferred name `gate0/ddg-html-browser-verification` is noted and not used)
**Verified surface profile:** `ENV-001-SURFACE-DDG-HTML-01`
**Provenance of the results below:** OWNER-ATTESTED BROWSER HANDOFF. The seven `BEV-*` tests were executed and observed by the owner in Chrome via Claude in Chrome and are transcribed here. **This Codex session did not run them and cannot independently verify them.** No `BEV-*` execution was performed in this session (see §12).

> **Scope note.** This is an interface/surface fidelity test, not research. No formal query (`FS-*`) was executed, no `FQ-*` register query was run, and no source was reviewed substantively. D1A remains **INCOMPLETE** and formal execution of the eight surface-compatible P1 queries remains **NOT AUTHORIZED** after this report. This profile does **not** create a new environment ID; `ENV-017` was explicitly not created.

## 1. Authorization

The owner authorized a bounded browser-surface fidelity verification to determine whether a real, visible DuckDuckGo HTML search surface honours the phrase- and spacing-sensitive behaviours that eight P1 queries in `FORMAL_QUERY_REGISTER.csv` depend on — behaviours the AI-mediated cloud surface (`ENV-001-SURFACE-CLOUD-01`) was shown **not** to honour under D-0022 (`PARTIAL_VERIFICATION`). This microstage records that already-completed verification. It does not execute any formal search and does not reopen D1A.

## 2. Instrument

- **Provider:** DuckDuckGo.
- **Interface:** `https://html.duckduckgo.com/html/` — the non-JavaScript HTML endpoint.
- **Browser:** Chrome, driven through Claude in Chrome (a real, visible search surface with a visible query box).
- **Query delivery:** controlled URL query construction. The exact query bytes were inserted into the DuckDuckGo HTML request URL; for ZWNJ-sensitive strings, U+200C was explicitly percent-encoded. After submission, the visible browser search box was inspected to confirm the submitted string survived intact.
- **Result traceability:** DuckDuckGo HTML returns result links as redirect URLs carrying a directly decodable destination URL in the `uddg` parameter, from which title, destination URL, host, and path are recoverable.

## 3. Verified surface profile

`ENV-001-SURFACE-DDG-HTML-01` — a candidate **execution surface profile** within the frozen `ENV-001` "Mainstream general-web search" environment class (authorized role `BOUNDED DISCOVERY / SOURCE LOCATION`). It is a profile identifier only. It is **not** a new environment, and it does not change the scientific meaning or frozen status of `ENV-001`.

## 4. Test method

Seven browser tests (`BEV-001`–`BEV-007`) were run in a temporary `BEV-*` namespace. These are surface tests — **not** `CAL-*` calibration, **not** `EV-*` cloud-surface tests, and **not** `FS-*` formal executions. No `FS` IDs were used; no formal query was executed; no source was reviewed substantively. Per-test detail is in `literature/BROWSER_SURFACE_VERIFICATION_LOG.csv`.

The method tested four properties:

1. exact-phrase quotation preservation and behaviour (English quoted vs unquoted control);
2. Persian ZWNJ (U+200C) vs ordinary-space (U+0020) preservation and retrieval distinction, on two phrase pairs;
3. site-domain (`site:`) suffix-constraint behaviour;
4. destination-URL traceability through the `uddg` redirect parameter.

## 5. PASS criteria

A `PASS` for this profile requires all of:

- the exact submitted query string is auditable (the submitted bytes are known and confirmed intact in the visible search box);
- quotation marks are preserved in the submitted query;
- the quotation operator materially changes retrieval (quoted vs unquoted differ);
- Persian ZWNJ is preserved (codepoint-confirmed);
- the ZWNJ vs ordinary-space distinction is materially observable in retrieval;
- the site-domain constraint is materially respected;
- real destination URLs are traceable;
- no silent AI query rewrite is observed.

**Method-bound condition (load-bearing).** This PASS certifies `ENV-001-SURFACE-DDG-HTML-01` **only when queries are delivered by the same controlled URL-encoding method verified here** (exact bytes inserted into the request URL, ZWNJ percent-encoded, submitted string re-inspected in the visible box). It does **not** certify hand-typed entry or any other delivery path; those remain unverified until separately tested. A future reader authorizing execution must not assume fidelity for a different input method.

## 6. Results (owner-attested)

| ID | Test | Exact input | Key observation | Result |
|---|---|---|---|---|
| BEV-001 | English quoted phrase | `"Kelar Dasht"` | quotes preserved; no visible rewrite; 4 first-page links | PASS |
| BEV-002 | English unquoted control | `Kelar Dasht` | input preserved; 10 first-page links; materially broader than BEV-001 | PASS |
| BEV-003 | Persian ZWNJ quoted | `"کارگاه‌موزه"` (U+200C) | ZWNJ preserved; codepoint hex `200c`; 0 first-page results | PASS (fidelity) |
| BEV-004 | Persian ordinary-space quoted | `"کارگاه موزه"` (U+0020) | ordinary space preserved; codepoint hex `20`; 2 first-page results | PASS |
| BEV-005 | Persian ZWNJ quoted | `"باستان‌شناسی"` (U+200C) | ZWNJ preserved; codepoint hex `200c`; 8 first-page results | PASS |
| BEV-006 | Persian ordinary-space quoted | `"باستان شناسی"` (U+0020) | ordinary space preserved; codepoint hex `20`; 6 first-page results; ordering differed from BEV-005 | PASS |
| BEV-007 | Site-domain constraint | `site:mcth.ir کلاردشت` | preserved verbatim; 10 links; all hosts within `*.mcth.ir` | PASS |

Interpretations recorded with the tests: the quotation operator materially changed retrieval behaviour (BEV-001 vs BEV-002); the ZWNJ-vs-ordinary-space distinction remained observable and materially affected retrieval (BEV-003/004 and BEV-005/006); the site-domain suffix constraint was materially respected (BEV-007).

**URL traceability:** `PASS`. DuckDuckGo HTML returned real result links through redirect URLs containing a directly decodable destination URL in the `uddg` parameter, sufficient to recover title, destination URL, host, and path. Redirect rank/order/counts are **not** treated as evidence.

**BEV-003 zero results:** recorded as fidelity-only. Zero first-page results is **not** interpreted substantively and is **not** evidence of absence.

## 7. Classification

**`PASS`** (method-bound, per §5). Verified properties:

- exact submitted query string auditable;
- quotation marks preserved;
- quotation semantics materially functional;
- Persian ZWNJ preserved;
- ZWNJ vs ordinary-space distinction materially observable;
- site-domain constraint functional;
- real destination URLs traceable;
- no observed silent AI query rewrite.

## 8. Safe query mapping

On `ENV-001-SURFACE-DDG-HTML-01`, and subject to separate owner authorization for execution, the following eight previously `BLOCKED_FOR_SURFACE_FIDELITY` P1 queries are now **surface-compatible** (the surface-fidelity blocker is conceptually removed):

`FQ-D1-001`, `FQ-D1-002`, `FQ-D1-003`, `FQ-D1-004`, `FQ-D1-007`, `FQ-D2-002`, `FQ-D2-004`, `FQ-D4-001`.

For these eight, no surface-fidelity reason remains blocked. This does **not** mean evidence has been found, sources are authoritative, queries are high-yield, D1A is complete, or claims are supported. The queries were **not** executed in this task; their text, version, environment ID, `execution_authorized`, and `query_status` in `FORMAL_QUERY_REGISTER.csv` are unchanged.

## 9. What this does NOT establish

- No evidence, literature, claim, retrieval, or Spanish-case record was produced.
- No source authority, prevalence, or absence was established.
- D1A is not complete; only the surface-fidelity blocker for the eight queries is conceptually removed.
- `ENV-001`'s frozen status and `SEARCH_ENVIRONMENTS.csv` are unchanged; a passed surface profile promotes nothing into the frozen registry.

## 10. Limitations

- PASS applies only to DuckDuckGo HTML (`html.duckduckgo.com/html/`); Google and Bing were not tested; the DuckDuckGo JavaScript interface was not tested.
- PASS is **method-bound**: it applies to the controlled URL-encoded input method used here. Physical keyboard entry of ZWNJ was **not** tested; formal execution should use the same exact URL-encoded input method unless a different method is separately re-verified.
- First-page result counts were used only as behavioural comparison anchors; counts, rank, and order are non-evidentiary.
- BEV-003 returning zero results is not evidence of absence.
- SafeSearch and region remained at DuckDuckGo defaults.
- Provider/index behaviour may change over time; a pass today is not a permanent guarantee.
- The results are owner-attested from a browser handoff and were not independently reproduced by this session (§ header, §12).

## 11. Explicit statement — no formal query executed

**No formal query was executed in this task.** No `FS-*` execution occurred, no `FQ-*` register query was run, no source was reviewed substantively, and no evidence/claim/literature/retrieval/Spanish-case record was created or modified. The eight surface-compatible queries remain frozen and unauthorized for execution pending a separate owner decision (`D-0025` or equivalent).

## 12. Boundary validation

- Formal searches executed: 0
- New `BEV-*` executions performed in this (Codex) session: 0 (results are the owner-approved browser handoff)
- `FS-*` rows added: 0
- `FQ-*` formal query executions: 0
- Evidence-register rows added: 0
- Claim-register rows added: 0
- Literature-matrix rows added: 0
- Formal-retrieval rows added: 0
- Spanish-case rows added: 0
- Query text changed: NO
- Query version changed: NO
- `FORMAL_QUERY_REGISTER.csv` changed: NO
- `SEARCH_LOG.csv` changed: NO
- `SEARCH_ENVIRONMENTS.csv` changed: NO
- CHALUS boundary changed: NO
- New environment ID created: NO (`ENV-017` not created)
- D1A resumed / completed: NO

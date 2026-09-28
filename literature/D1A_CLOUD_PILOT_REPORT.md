# D1A Cloud-Compatible P1 Retrieval Pilot Report

**Substage:** `D1A-P` — Cloud-compatible P1 pilot (bounded; **not** D1A completion)
**Surface profile:** `ENV-001-SURFACE-CLOUD-01` (AI-mediated cloud `WebSearch`; US-region-only; provider/version opaque)
**Date:** 2026-09-28
**Scope note:** This report describes **pipeline performance only**. It reports no substantive Kelardasht heritage, tourism, funding, or data findings. Ranking, snippets, displayed result counts, and AI summaries were treated as non-evidentiary and ignored throughout.

---

## 1. Authorization
Owner Decision `D-0023` (2026-09-28), building on `D-0022` (`PARTIAL_VERIFICATION`). Authorizes execution of only the four Cloud-compatible bare-token P1 queries as a retrieval/metadata-screening pipeline pilot. Evidence acquisition, full-source review, claim verification, literature synthesis, Spanish case screening, and the Gate 0 verdict remain **NOT AUTHORIZED**.

## 2. Base commit
`e81ca44ec5a76df827d8cdaa8d1f123e7fd90a17` — current reviewed `main` (merge of PR #1, ENV-001 Cloud-surface verification; carries D-0022 and the ENV-001 verification report/log).

## 3. Branch
`claude/gate0-d1a-cloud-pilot-kbz1sg`, freshly branched from the reviewed `main` (session-designated development branch). The prompt's preferred name `gate0/d1a-cloud-compatible-pilot` is noted; the session's mandated branch name was used instead. No work was performed on `main`.

## 4. Exact executed query IDs
| FS ID | Query ID | Domain | Frozen query string (executed verbatim) |
|---|---|---|---|
| FS-001 | FQ-D2-001 | D2 | `کلاردشت موزه موزه باستان‌شناسی میراث فرهنگی` |
| FS-002 | FQ-D3-001 | D3 | `کلاردشت میراث فرهنگی گردشگری طرح برنامه پروژه` |
| FS-003 | FQ-D3-002 | D3 | `کلاردشت میراث فرهنگی بودجه اعتبار قرارداد اجرا بهره‌برداری` |
| FS-004 | FQ-D11-001 | D11 | `کلاردشت سالنامه آماری داده مکانی مرز اداری گردشگری میراث فرهنگی` |

Strings were copied verbatim from `FORMAL_QUERY_REGISTER.csv`; no word was added, removed, respelled, requoted, or refiltered. **Observation only:** `FQ-D2-001` contains a doubled token (`موزه موزه`); it was executed unaltered per D-0023 and flagged for possible future owner review. This is not a query change.

## 5. Execution count
4 formal executions (`FS-001`–`FS-004`); the authorized ceiling of 4 and the complete authorized subset. Blocked-query executions: 0. P2/P3/template executions: 0.

## 6. Records inspected
36 total (9 per query; every query's displayed set was ≤ the 20-record ceiling, so no early-stopping rule was triggered by the ceiling). Logged as `RET-0001`–`RET-0036` in `FORMAL_RETRIEVAL_REGISTER.csv`.

## 7. Unique retained
32 unique locator records (36 inspected − 4 confirmed duplicates).

## 8. Duplicates
4 confirmed duplicates, **all exact-URL repeats**: `RET-0012` (=`RET-0003`), `RET-0015` (=`RET-0006`), `RET-0031` (=`RET-0006`), `RET-0035` (=`RET-0008`).
Only exact-URL identity is treated as a confirmed duplicate. `RET-0006` (akharinkhabar.ir) returned the same/near-identical headline as `RET-0003` (mehrnews.com), but this is **not** asserted as a cross-host duplicate: the lineage cannot be verified without dereferencing, so `RET-0006` is recorded as `DISCOVERY_ONLY` with a `POSSIBLE_CROSS_HOST_DUPLICATE — LINEAGE NOT VERIFIED` note. The `akharinkhabar.ir/local/11016623` URL did recur by exact match across three of the four searches (`RET-0006`/`RET-0015`/`RET-0031`), which is what supports the two confirmed exact-URL duplicates among them.

## 9. POTENTIALLY_ELIGIBLE
13 records: `RET-0002`, `RET-0003`, `RET-0004`, `RET-0010`, `RET-0013`, `RET-0016`, `RET-0019`, `RET-0021`, `RET-0022`, `RET-0028`, `RET-0032`, `RET-0033`, `RET-0036`. All routed for future review only; none accepted as evidence.

## 10. DISCOVERY_ONLY
12 records: `RET-0005`, `RET-0006`, `RET-0008`, `RET-0011`, `RET-0014`, `RET-0017`, `RET-0020`, `RET-0025`, `RET-0027`, `RET-0029`, `RET-0030`, `RET-0034`.

## 11. EXCLUDED_AT_METADATA
7 records: `RET-0001`, `RET-0007`, `RET-0009` (non-Kelardasht museum/encyclopedia references), `RET-0018` (Kalat, not Kelardasht), `RET-0023` (Golestan), `RET-0024` (Fars), `RET-0026` (Razavi Khorasan). All excluded on geographic-scope mismatch observable from the returned title.

## 12. BLOCKED_ACCESS
0. No access attempt was blocked (no landing page was dereferenced under the applied fidelity safeguard). Access status for civilica.com, ircud.ir, namafar.ir, and gisoom.com is recorded as `NOT_VERIFIED`, not `BLOCKED_ACCESS`.

## 13. Sensitive / specialist flags
- `SENSITIVE_REVIEW_REQUIRED`: 0. No vulnerable archaeological coordinates or sensitive location information were encountered in any returned title or URL (`SENSITIVE_LOCATION_INFORMATION_PRESENT = NO` for all rows).
- `SPECIALIST_REVIEW_REQUIRED`: 0 at the locator stage.

## 14. Query failures
0 `QUERY_REVIEW_REQUIRED`. All four bare-token queries were accepted and returned link sets without material rewriting or refusal by the surface.

## 15. Operational limitations
1. Surface is AI-mediated, provider/version opaque, and US-region-only; the AI summary layer was ignored, and ranking/snippets/counts are non-evidentiary (per D-0022).
2. Under the applied fidelity safeguard, only directly observed locator fields (retrieval/search/query IDs, surface profile, domain, language, result position, returned title, URL, host) were recorded. Author, publication date, source type, and temporal scope are `NOT_CAPTURED`; access status is `NOT_VERIFIED`; source tier is `TIER_UNRESOLVED` for **every** row (source authority is not inferred from domain alone). Geographic scope is set only where the returned title itself states a locality; otherwise `UNRESOLVED`. No landing page was read.
3. Each query returned exactly 9 displayed links — a shallow surface depth well below the 20-record ceiling; this constrains recall for discovery.
4. One returned title carried a corrupted Unicode glyph (`RET-0019`, in `لایحه`), indicating occasional encoding noise in returned metadata.
5. Single execution per query cannot separate ranking instability from genuine input-sensitivity; counts are not a coverage measure and absence was not inferred from early stopping.

## 16. Was metadata screening workable?
**Yes, at the locator level.** Returned titles + URLs + hosts were sufficient to (a) route on geographic scope where the title itself states a locality (7 clean metadata exclusions, incl. a Kalat/Kelardasht token confusion), (b) separate candidate official/statistical-looking pages (by returned title and host string) from press and self-published material **without asserting their authority**, and (c) apply non-acceptance screening states consistently. It was **not** sufficient for author/date/source-type/tier resolution without substantive reading, which the pilot deliberately did not perform.

## 17. Was source provenance recoverable?
Two distinct notions must be separated:

- **LOCATOR PROVENANCE — recoverable:** every record carried a concrete, dereferenceable URL and an identifiable host string (e.g., mehrnews.com, mcth.ir, richt.ir, civilica.com, en.wikipedia.org). Title, URL, and host are directly observed and recoverable.
- **SOURCE AUTHENTICATION / BIBLIOGRAPHIC PROVENANCE — NOT YET VERIFIED:** institutional ownership, source authority, author, date, and underlying-publication lineage are **not** established by a host string and were not confirmed (no dereferencing, no substantive reading). Apparent lineages — e.g., a statistical yearbook surfacing via an official-looking domain and via third-party hosts — are recorded as unverified pointers, not authenticated provenance.

## 18. Is the Cloud surface useful enough to retain for compatible retrieval?
**Yes, but strictly as a locator layer** for token-based bounded discovery of Kelardasht-relevant candidate pages, difficult-to-index Persian materials, and apparent data/publication landing pages. Its outputs are AI-surfaced pointers, not bibliographic records, and every retained row requires independent source authentication and re-verification before any evidentiary use. It is not a reproducible bibliographic database, a prevalence/count measure, or a basis for inferring absence.

## 19. Does full D1A still require a browser surface for the blocked queries?
**Yes.** The eight `BLOCKED_FOR_SURFACE_FIDELITY` P1 queries depend on exact-phrase quoting and/or material half-space (ZWNJ) phrase precision, which D-0022 showed this surface does not honor. Completing D1A across the full P1 set requires either a verified browser surface for those queries or a query-design change authorized separately. This pilot completes only the four compatible queries and does not complete D1A.

---

### Boundary validation (pipeline)
- Formal executions: 4 (ceiling 4)
- Executed query IDs ⊆ {FQ-D2-001, FQ-D3-001, FQ-D3-002, FQ-D11-001}: YES
- Blocked-query executions: 0 · P2 executions: 0 · P3 executions: 0 · template executions: 0
- Evidence rows: 0 · claim rows: 0 · literature rows: 0 · Spanish-screening rows: 0
- Full-source reviews: 0 · citation chaining: 0
- Query text changed: NO · query version changed: NO · CHALUS boundary changed: NO
- `CAL-029`/`CAL-030` created: NO · `EV-*` records altered: NO
- Protected files modified: NO

# Gate 0 Stage B Multilingual Search Calibration Report

**Status:** OWNER-APPROVED — STAGE B CLOSED / CALIBRATION COMPLETE
**Authorization:** Executed under Gate 0 Stage B calibration authority; closed by Decision D-0019
**Calibration date:** 2026-09-25
**Authoritative Stage A freeze:** `0ebbafd3aa2bdc5615cc564506ca4f024156af28`
**Evidence status:** No item in this report is evidence and no substantive finding is reported.

## 1. Purpose and authorization

This calibration tested terminology, spelling, transliteration, indexing vocabulary, search-environment behavior, and likely institutional wording in Persian, English, and Spanish. It did not test the truth of a Kelardasht proposition, acquire literature or evidence, screen a Spanish case, or execute a formal search.

The hard ceiling was 30 query executions. A query execution was counted as one distinct query string in one identified environment under one defined filter configuration. Material changes to language, wording, environment, filter, geography, or search mode counted separately.

## 2. Execution count

- Executions used: **28 of 30**.
- Persian: 13; English: 9; Spanish: 6. These totals emerged from domain–language relevance and were not quotas.
- Every execution is recorded as `CAL-001` through `CAL-028` in `literature/SEARCH_LOG.csv`.
- The search interface did not expose a reliable per-execution clock time. The `timestamp` field therefore records the ISO execution date, while `execution_sequence` preserves exact order.
- The final two possible executions were not used. Remaining issues concern native-platform access and future platform-specific syntax, not a terminology uncertainty that justified consuming the ceiling.
- Owner decision: **CALIBRATION SUFFICIENT**. The remaining two executions are intentionally unused; no Stage B extension is authorized.
- Executions `CAL-001` to `CAL-004` were issued together as four distinct query strings. The interface aggregated their returned records, so per-query result counts were unavailable; this limitation is explicit in the log and does not change the execution count.

## 3. Environments tested

Actually tested:

1. A mainstream general-web search environment for multilingual title, snippet, metadata, heading, spelling, and transliteration behavior.
2. The same environment with a `site:sid.ir` constraint as a limited proxy test for Persian academic discoverability.
3. The same environment with a `site:datos.gob.es` constraint for official Spanish open-data catalogue discoverability.
4. Metadata and landing-page terminology surfaced from official national institutions, university/repository pages, publisher/DOI pages, and international institutional pages.

Not tested as native search interfaces: SID, Magiran, Civilica, Noormags, Google Scholar, Crossref, Dialnet, Scopus, and Web of Science. No access to subscription databases is claimed. Results surfaced through the general web do not establish native database coverage or search behavior.

## 4. Domain × language cells tested

| Domain | Persian | English | Spanish |
|---|---:|---:|---:|
| D1 Kelardasht heritage/archaeology | Yes | Yes | — |
| D2 institutions/museums/sites/initiatives | Yes | — | — |
| D3 official plans/programmes/announcements | Yes | — | — |
| D4 local/regional academic literature | Yes | Yes | — |
| D5 heritage/archaeological tourism planning | Yes | Yes | Yes |
| D6 governance/conservation/visitor-management readiness | — | Yes | Yes |
| D7 community participation/local benefit | Yes | Yes | Yes |
| D8 visitor pressure/capacity/environmental management | — | Yes | Yes |
| D9 policy transfer/lesson drawing | — | Yes | — |
| D10 Spanish candidate discovery | — | — | Yes |
| D11 data feasibility | Yes | — | Yes |
| D12 specialist dependency | Not searched independently | Not searched independently | Not searched independently |

D12 did not develop a genuine standalone vocabulary problem, so the Stage A restriction against independent D12 searching was preserved.

## 5. Terminology learned

The calibration supports the following bounded refinements to the Stage A concept families:

- Archaeological-site naming needs both place-name and site-name families: `Kelardasht` variants plus `Kelar Mound`, `Kelar Hill`, `Tepe Kelar`, `Tapeh Kelar`, and `Tappeh Kelar`.
- Heritage-tourism searching should keep `heritage tourism`, `cultural heritage tourism`, `archaeological tourism`, `archaeotourism`, and `archaeology-based tourism` related but not interchangeable.
- Community terminology must distinguish participation and decision authority from ownership, empowerment, benefit sharing, and benefit distribution.
- Visitor-pressure terminology should separate carrying/capacity language from `Limits of Acceptable Change`, `Visitor Use Management`, `Visitor Experience and Resource Protection`, and `Visitor Impact Management`.
- Owner-approved interpretation: `CONSERVATION READINESS` remains a project analytical construct, while literal `conservation readiness` is demoted as a primary indexing phrase. Future domain-specific retrieval prioritizes established, non-synonymous families including heritage conservation, conservation planning, heritage management, management capacity, institutional capacity, governance capacity, preventive conservation, and conservation governance. **ANALYTICAL CONCEPT ≠ PRIMARY SEARCH TERM.**
- Owner-approved interpretation: `ADAPTIVE POLICY / PRACTICE TRANSFER` remains a project-level analytical framing, while `adaptive transfer` is demoted as a primary indexing phrase. Formal academic retrieval prioritizes policy transfer, lesson drawing, policy learning, policy mobility, institutional transfer, policy adaptation, and contextual adaptation without treating them as interchangeable. **PROJECT ANALYTICAL LANGUAGE ≠ DATABASE INDEXING LANGUAGE.**

## 6. Persian terminology findings

- Both half-space and ordinary-space forms must remain discoverable: `باستان‌شناسی` / `باستان شناسی`, `باستان‌شناختی` / `باستان شناختی`, `کارگاه‌موزه` / `کارگاه موزه`, and `کاخ‌موزه` / `کاخ موزه`.
- The exact phrase `کارگاه‌موزه` with Kelardasht returned no results in the tested environment. The ordinary-space form produced many results but with substantial phrase splitting and unrelated workshop/museum contexts. Neither form should be used alone.
- Productive archaeology and institution vocabulary included `تپه باستانی`, `محوطه باستانی`, `کاوش باستان‌شناسی`, `بررسی‌های باستان‌شناسی`, `موزه باستان‌شناسی`, `کاخ‌موزه`, and the formal ministry/department phrase `میراث فرهنگی، گردشگری و صنایع دستی`.
- `گردشگری فرهنگی` was the clearest of the tested heritage-oriented tourism phrases. `گردشگری تاریخی` also appeared in institutional/public discourse but is broad and sensitive to current-news duplication. `گردشگری میراث` was low precision because the search environment frequently split it into co-occurring words.
- Community terminology should include both `گردشگری اجتماع‌محور` and `گردشگری جامعه‌محور`, together with `توانمندسازی`, `ذی‌نفعان محلی`, `توزیع عادلانه منافع`, and `اقتصاد محلی`.
- Data-feasibility searching should add `سالنامه آماری`, `مرز اداری`, `شهرستان`, `بخش`, `دهستان`, `داده مکانی`, `سامانه جامع نظارت، آمار و اطلاعات`, and relevant official-institution names.

## 7. English terminology findings

- Joined, spaced, hyphenated, and diacritic forms all occur or are normalized by search systems: `Kelardasht`, `Kelar Dasht`, `Kelar-Dasht`, `Kalardasht`, `Kalar Dasht`, `Kelār Dasht`, `Kalār Dasht`, and `Kelārdasht`.
- Regional discovery should use both `western Mazandaran` and `west of Mazandaran` and must not treat regional results as Kelardasht evidence.
- `Archaeotourism` is a useful specific family, but should not replace broader heritage/cultural-tourism terminology.
- D6 and D9 require the refinements recorded in Section 5; these are proposed query-family amendments, not findings about governance or transferability.

## 8. Spanish terminology findings

- `Gestión patrimonial` without a cultural qualifier is ambiguous and frequently retrieves private-wealth management. Prefer or pair it with `gestión del patrimonio cultural`, `gestión patrimonial cultural`, `patrimonio arqueológico`, or `bienes culturales`.
- Distinct useful families include `gobernanza del patrimonio cultural`, `gobernanza participativa`, `gobernanza en red`, `tutela del patrimonio cultural`, `coordinación interadministrativa`, `conservación preventiva`, `plan director`, `uso público`, `visitabilidad`, and `puesta en valor`.
- `Capacidad de acogida turística`, `capacidad de carga turística`, `gestión de flujos de visitantes`, `gestión de visitantes`, `visita pública`, `afluencia`, `saturación`, and `límites de cambio aceptable` should not be collapsed into one term.
- Spain-specific community retrieval needs geographic or institutional constraints because an unqualified Spanish-language query strongly retrieved Latin American material.
- Candidate discovery vocabulary should include `paisaje cultural`, `espacio natural protegido`, `plan director`, `planes nacionales`, `plan sectorial`, `planificación territorial`, `turismo rural`, and `desarrollo local`. These terms did not create or screen a candidate list.
- Official data discovery should include catalogue fields and service terms such as `conjunto de datos`, `publicador`, `cobertura geográfica`, `frecuencia de actualización`, `distribuciones`, `licencia`, `interoperabilidad`, `WMS`, `WFS`, `GeoJSON`, `EPSG`, and `INSPIRE`.

## 9. Transliteration findings

- `Kelardasht` and `Kelar Dasht` are both productive discovery forms.
- Site-specific forms (`Tepe/Tapeh/Tappeh Kelar`, `Kelar Hill`, `Kelar Mound`) retrieve records that a place-name-only query can miss.
- The tested general-web environment substantially normalized diacritics: a query for `Kelār Dasht` returned many non-diacritic forms. Diacritic retrieval performance therefore cannot be inferred from exact-query appearance alone.
- `Kalardasht`, `Kalar Dasht`, `Kalār Dasht`, `Kelārdasht`, and the non-English `Kelardascht` were observed as variants.
- No canonical English form is selected here. Canonical naming remains governed by the Language Protocol and source authority.

## 10. Indexing and database behavior

- Exact quotation improved phrase control but did not prevent all token splitting in Persian.
- Persian half-space handling materially affected recall for the workshop-museum test; both forms should be retained where relevant.
- General-web indexing mixed official, academic, news, aggregator, social, promotional, and low-authority pages. Institutional ownership must be verified directly before a term is treated as official vocabulary.
- Current-news duplication can dominate narrow Kelardasht queries and must be controlled in formal searching through source environment, domain, date, and source-type logic.
- A `site:sid.ir` query did not provide a reliable view of SID's native holdings. General-web site restriction must not substitute for native academic-database searching.
- The official Spanish open-data catalogue exposed stable catalogue and geospatial-service vocabulary through indexed metadata, but no dataset was downloaded, assessed, or accepted as usable.

## 11. Access limitations

- No subscription or authenticated database was accessed.
- Native Persian academic database behavior remains untested.
- Native Dialnet, Google Scholar, Crossref, Scopus, and Web of Science behavior remains untested.
- Some Iranian official/local material surfaced through aggregators or social channels; direct institutional ownership and durable access remain to be verified later.
- Search-engine normalization prevents a conclusive test of Arabic/Persian character substitutions (`ي/ی`, `ك/ک`) and romanisation diacritics at this stage.
- No access control, robots restriction, geographic restriction, authentication barrier, or paywall was bypassed. Inaccessibility was not interpreted as absence of evidence.

## 12. Search-environment suitability

| Environment | Calibration suitability | Formal-search implication |
|---|---|---|
| General web | Good for terminology, transliteration, institution-name, and landing-page discovery; poor authority control | Use as discovery and document-location route, not as an evidence-quality proxy |
| General web + official-domain constraint | Useful when the authoritative domain is known | Verify the publisher and document directly; record the exact domain/filter |
| General web + academic-domain constraint | Insufficient as a proxy for native database coverage | Use the native interface or clearly describe the limitation |
| Official landing pages surfaced through indexing | Useful for institutional vocabulary | Revisit directly during authorized formal screening |
| Publisher/DOI/repository metadata surfaced through indexing | Useful for titles, abstracts, keywords, and identifiers | Re-run in an authorized formal academic environment and assess eligibility normally |

## 13. Proposed architecture refinements

The following calibration-driven refinements are owner-approved and incorporated into the governing architecture where operationally required:

1. Add the observed Kelar site-name and romanisation variants to D1/D4 discovery families.
2. Add Persian institutional, archaeology-method, palace-museum, community-based-tourism, and statistical/administrative vocabulary listed above.
3. Retain both half-space and ordinary-space Persian forms where indexing behavior differs; do not pre-normalize before a platform-specific query is defined.
4. Qualify Spanish `gestión patrimonial` with cultural/archaeological vocabulary.
5. Add Spanish `visitabilidad`, `uso público`, `tutela`, `conservación preventiva`, planning-instrument, and open-data service vocabulary.
6. Separate community participation/authority terms from benefit/ownership/distribution terms in all languages.
7. Separate carrying/capacity families from LAC/VUM/VERP/visitor-impact-management families.
8. Demote literal `conservation readiness` and `adaptive transfer` as primary indexing phrases while retaining the related project analytical constructs; use the distinct owner-approved retrieval families recorded in Section 5 and do not treat them as synonyms.
9. Require Spain-specific geographic/institutional constraints for D7 and formal source-type controls for Kelardasht current-news duplication.
10. If Stage C is later authorized, classify every proposed formal environment as `VERIFIED`, `CONDITIONAL_UNVERIFIED`, or `EXCLUDED` and record native-interface availability, field syntax, coverage, and authentication basis. Exact executable queries cannot be operationally frozen for `CONDITIONAL_UNVERIFIED` environments; only templates or conceptual families may be recorded pending legitimate verification.

No exact formal query strings were drafted or executed in Stage B.

## 14. Unresolved terminology issues

- Native Persian databases may use controlled fields, spelling normalization, or vocabulary not visible to the general web.
- Arabic/Persian character-variant behavior remains platform-specific.
- Native Spanish academic indexing and regional-government portal terminology remain to be tested when Stage C is authorized.
- The practical difference among some close Persian tourism compounds will require platform-specific field testing rather than more general-web volume comparisons.
- Exact environment-specific syntax, fields, filters, and result-count behavior remain deliberately unfrozen.

## 15. Need for additional calibration

No additional Stage B general-web calibration is recommended. The two unused executions should remain unused. The unresolved items are best handled as explicit Stage C environment/setup checks and owner-reviewed formal-query drafting, not by extending exploratory searching.

If the owner requires native-interface calibration before Stage C, that should be separately authorized and logged; this report does not assume such access exists.

## 16. Readiness for formal search freeze

The Stage B calibration record is ready to freeze. From a calibration standpoint, the architecture is sufficiently refined for a future owner-authorized Stage C formal-search drafting/freeze, subject to the native-environment classifications above. Stage C is not authorized; no exact formal query set is operationally frozen; formal evidence and literature acquisition remain unauthorized.

## Boundary validation

- Query executions: 28/30; every execution logged.
- Formal searches executed: 0.
- Sources acquired into the evidence base: 0.
- Claim-register rows added: 0.
- Evidence-register rows added: 0.
- Literature-matrix rows added: 0.
- Spanish cases screened or selected: 0.
- Substantive Kelardasht claims accepted: 0.
- CHALUS boundary changes: 0.
- Later gates opened: 0.
- Sensitive archaeological coordinates reproduced: 0.
- Calibration leads retained: 6, all marked `CALIBRATION LEAD — NOT YET EVIDENCE`.
- Calibration leads promoted to evidence or substantive registers: 0. Stage C cannot promote them; they may enter formal screening only during a later explicitly authorized evidence-acquisition stage.

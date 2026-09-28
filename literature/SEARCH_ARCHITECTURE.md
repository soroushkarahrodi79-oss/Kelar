# Gate 0 Search Architecture

**Document status:** Stage A architecture frozen; owner-approved Stage B refinements incorporated
**Gate:** 0 — Scientific Feasibility & Comparative Design
**Current authority:** Stage B calibration closed/owner-approved; Stage C formal-search architecture closed/frozen under Decisions D-0020 and D-0021; execution and evidence/literature acquisition remain unauthorized
**Evidence acquisition:** NOT AUTHORIZED
**Calibration search:** CLOSED — 28 OF 30 QUERY EXECUTIONS USED; CALIBRATION SUFFICIENT; 2 INTENTIONALLY UNUSED
**Formal search:** NOT AUTHORIZED
**Baseline reference:** `4ac933fdad99c3cfd495e6c175c1e3d64b37f217`
**Canonical documentation language:** English
**Last updated:** 2026-09-25

## 1. Purpose and boundary

This document defines the multilingual, reproducible, and bounded architecture governing Gate 0 searching. It was frozen before Stage B; authorized calibration execution and owner-approved refinements are recorded explicitly so the frozen rules do not drift silently.

It does **not** contain frozen literal queries, search results, sources, evidence, accepted claims, candidate Spanish cases, or findings. All vocabulary below is provisional search-design material. Stage B calibration may propose refinements, but no refinement may enter the formal protocol silently.

The architecture is designed to answer the ten Gate 0 questions through the minimum necessary search domains. A domain may later be narrowed, deferred, or removed if it is non-decisive, structurally unsupported, ethically unsafe, or dependent on unavailable specialist competence.

## 2. Governance and stage model

| Stage | Function | Current status | Permitted output |
|---|---|---|---|
| `A_ARCHITECTURE` | Define domains, terminology families, environments, selection logic, controls, and future logging. | **CLOSED / FROZEN** | Owner-reviewable design only. |
| `B_CALIBRATION` | Test terminology and indexing assumptions within a strict cap. | **CLOSED / CALIBRATION COMPLETE — 28/30 EXECUTIONS** | Calibration log and owner-approved query-family amendments only. |
| `C_FORMAL_FREEZE` | Approve exact platform-specific queries, filters, and sequence. | **CLOSED / FORMAL SEARCH ARCHITECTURE FROZEN** | Frozen formal plan, environment registry, and query register; no execution. |
| `D_FORMAL_SEARCH` | Execute authorized Gate 0 searches and screen results. | **CLOSED** | Search log, candidate/source records, evidence/literature entries as separately authorized. |

No stage opens automatically. Owner authorization must be recorded in `docs/DECISION_LOG.md`. Stage A approval will not itself authorize Stage B.

## 3. Gate-question coverage

| Gate question | Search need | Primary domains |
|---|---|---|
| Q1 | Defensible evidence concerning Kelardasht heritage significance. | D1, D4, D12 |
| Q2 | Verified maturity/status of heritage and tourism initiatives. | D2, D3, D12 |
| Q3 | Lawful, practical, non-fieldwork data availability. | D11, D12 |
| Q4 | Coherent literature across relevant disciplines. | D4–D9, D12 |
| Q5 | Research gap and useful planning contribution. | D4–D9 |
| Q6 | Systematically discoverable Spanish candidate cases. | D10 |
| Q7 | Plausible transfer/adaptation/rejection objects. | D5–D10, D12 |
| Q8 | Owner-competence boundary. | D1, D4–D9, D12 |
| Q9 | Claims requiring specialist review. | D12 across all domains |
| Q10 | Sufficiency to continue. | Synthesis of D1–D12; no separate broad search. |

## 4. Search domains

The twelve domains are retained because they serve distinct evidence functions and source environments. They are not equal in expected size and must not be combined into one omnibus query.

### D1 — Kelardasht archaeological and cultural-heritage significance

- **Purpose:** Discover source pathways capable of establishing what is documented about heritage existence, character, significance, dating, designation, condition, or vulnerability.
- **Gate questions:** Q1, Q8, Q9.
- **Boundaries:** No owner/AI archaeological interpretation; no site-coordinate collection unless later demonstrated essential and authorized.
- **Priority sources:** Original archaeological documentation and official heritage records (A), then peer-reviewed archaeological/history research (B) and qualified technical work (C).

### D2 — Kelardasht heritage institutions, sites, museums, workshops, and heritage initiatives

- **Purpose:** Identify claims about institutions, facilities, archaeological workshops, museums, heritage sites, exhibitions, conservation actions, and related initiatives for later status verification.
- **Gate questions:** Q1, Q2, Q8, Q9.
- **Boundaries:** Discovery of a name or announcement does not establish existence, operation, authority, continuity, or effect.
- **Priority sources:** Official mandates, records, organizational pages, budgets/contracts where public, implementation records, and original attributable statements (A); independent scholarly/technical assessment where available (B/C).

### D3 — Kelardasht/Mazandaran governmental heritage and tourism action

- **Purpose:** Distinguish public statements, announcements, projects, programmes, plans, funding, implementation, operational institutions, and outcomes relevant to Kelardasht.
- **Gate questions:** Q2, Q3, Q8, Q9.
- **Boundaries:** Provincial or national action is not attributed to Kelardasht without explicit geographic linkage. Public intent is not implementation.
- **Priority sources:** Adopted legal/planning documents, official administrative records, procurement/budget/implementation records, and original statements (A); independent technical/scholarly analysis (B/C).

### D4 — Academic literature on Kelardasht and Western Mazandaran heritage

- **Purpose:** Establish whether scholarly literature exists, which disciplines and evidence it uses, and whether Kelardasht-specific evidence can be assessed without new fieldwork.
- **Gate questions:** Q1, Q3, Q4, Q5, Q8, Q9.
- **Boundaries:** Western Mazandaran evidence supplies context only unless Kelardasht is explicitly within the study unit or inference is justified.
- **Priority sources:** Peer-reviewed research and academic books/theses with assessable methods (B); original technical/archaeological records (A/C).

### D5 — Heritage tourism, archaeotourism, and cultural-tourism planning

- **Purpose:** Identify concepts, mechanisms, limits, and critical evidence connecting heritage with tourism/destination planning.
- **Gate questions:** Q4, Q5, Q7, Q8.
- **Boundaries:** Heritage significance does not imply tourism suitability; “best practice” and promotional case material do not establish effectiveness or transferability.
- **Priority sources:** Peer-reviewed conceptual/empirical work (B), authoritative heritage/tourism guidance with transparent basis (C), and implemented instruments where relevant (A).

### D6 — Heritage governance and conservation readiness

- **Purpose:** Identify governance, legal/institutional capacity, preventive conservation, monitoring, finance, coordination, enforcement, and readiness concepts applicable before demand stimulation.
- **Gate questions:** Q4, Q5, Q7–Q9.
- **Boundaries:** Formal authority does not prove capacity; legal designation does not prove effective conservation.
- **Priority sources:** Law, adopted instruments, mandates, and implementation records (A); peer-reviewed governance/conservation research (B); recognized technical standards/guidance (C).

### D7 — Community participation, local benefit, and social safeguards

- **Purpose:** Identify empirical and methodological standards for participation, decision authority, representation, benefit/cost distribution, access, displacement, and cultural representation.
- **Gate questions:** Q4, Q5, Q7–Q9.
- **Boundaries:** No claim about Kelardasht residents may be inferred from official/promotional text, a single spokesperson, or evidence from another territory.
- **Priority sources:** Properly documented local/empirical research (B/A where authorized), then high-quality institutional methods and safeguards (C).

### D8 — Environmental sustainability and visitor-pressure management

- **Purpose:** Identify when visitor management, pressure indicators, carrying-capacity concepts, limits of acceptable change, protected-area relationships, and demand management are relevant.
- **Gate questions:** Q3–Q5, Q7–Q9.
- **Boundaries:** No carrying-capacity number, ecological condition, or visitor-pressure claim may be generated without appropriate data and expertise. Technology is not presumed to be a solution.
- **Priority sources:** Environmental/protected-area plans and monitoring (A), peer-reviewed empirical/methodological research (B), qualified technical guidance (C).

### D9 — Adaptive policy/practice transfer

- **Purpose:** Identify theories and evidence concerning policy transfer, policy mobility, lesson drawing, institutional transplantation, adaptation, failure, non-transferability, and functional alternatives.
- **Gate questions:** Q4, Q5, Q7, Q8, Q10.
- **Boundaries:** Similarity is not transferability; origin-country prestige is irrelevant; critical and failure literature is mandatory.
- **Priority sources:** Foundational and current peer-reviewed theory/empirical research (B), supported by documented policy evaluations (A/C).

### D10 — Spanish comparison-case discovery

- **Purpose:** Generate a transparent candidate pool for later screening against verified Kelardasht problem dimensions.
- **Gate questions:** Q6–Q8.
- **Boundaries:** Discovery is not eligibility, screening, shortlisting, or selection. Fame, awards, “smart” branding, UNESCO status, or data abundance do not imply comparability.
- **Priority sources:** Official heritage/planning/protected-area documentation (A), peer-reviewed case research (B), recognized technical case material (C); D/E only as discovery leads.

### D11 — Data feasibility

- **Purpose:** Identify whether relevant heritage inventories, statistics, geospatial/administrative/protected-area/transport/tourism/environmental datasets and plans appear to exist, with usable access and rights.
- **Gate questions:** Q3, Q6, Q8–Q10.
- **Boundaries:** Metadata discovery only in the later authorized feasibility stage; no downloading, bulk acquisition, coordinate inspection, analysis, or fitness conclusion from catalogue presence alone.
- **Priority sources:** Official data catalogues, custodians, metadata, licences, and technical documentation (A/C).

### D12 — Specialist-dependency identification

- **Purpose:** Identify which proposed claims or evidence types require archaeological, conservation, ecological, legal, transport-engineering, statistical, ethnographic, translation, or other specialist review.
- **Gate questions:** Q1–Q10, especially Q8–Q9.
- **Boundaries:** D12 is a cross-cutting classification pathway, not a search for specialists or an outreach programme. No person will be contacted in Gate 0 without separate authorization.
- **Priority sources:** Discipline-specific methodological standards, scope-of-practice indicators, source metadata, and the actual interpretive demands identified in other domains (A–C).

## 5. Language architecture

English is the canonical documentation language. Searches will later be designed in English, Persian, and Spanish according to domain relevance—not mechanically repeated in every language. Original Persian evidence takes precedence over translated secondary reporting when the original is lawfully accessible and interpretable.

The term lists below are **uncombined vocabulary families**, not executable queries. Orthographic variants are retained where they may affect retrieval. Persian and Spanish technical/institutional terms require owner review and Stage B calibration before formal use.

### 5.1 Domain × language relevance

Language allocation is driven by the domain and source function, not fixed quotas or equal replication. The categories below are routing judgments, not scores or weights:

- `PRIMARY` — expected to be essential for terminology or source discovery in that domain.
- `SUPPORTING` — expected to add material coverage or conceptual context.
- `CONDITIONAL` — used only when a specific source pathway, gap, or terminology issue justifies it.
- `NOT_NORMALLY_REQUIRED` — omitted unless a logged reason emerges.

| Domain | Persian | English | Spanish | Routing rationale |
|---|---|---|---|---|
| D1 Kelardasht heritage/archaeology | `PRIMARY` | `SUPPORTING` | `NOT_NORMALLY_REQUIRED` | Iranian primary and local scholarship are likely Persian; English may surface international scholarship or metadata. |
| D2 Kelardasht institutions/initiatives | `PRIMARY` | `CONDITIONAL` | `NOT_NORMALLY_REQUIRED` | Original institutional terminology and statements are expected primarily in Persian. |
| D3 Iranian governmental action | `PRIMARY` | `CONDITIONAL` | `NOT_NORMALLY_REQUIRED` | Iranian plans, mandates, and implementation terminology require Persian-first discovery. |
| D4 Kelardasht/Western Mazandaran scholarship | `PRIMARY` | `SUPPORTING` | `CONDITIONAL` | Persian and English may index different scholarly records; Spanish is used only for a justified academic pathway. |
| D5 Heritage-tourism planning | `SUPPORTING` | `PRIMARY` | `SUPPORTING` | International theory is strongly English-indexed; Persian and Spanish support contextual/application literature. |
| D6 Governance/conservation readiness | `PRIMARY` | `PRIMARY` | `PRIMARY` | Iranian rules, international theory/standards, and Spanish instruments each require their principal language. |
| D7 Community/local benefit/safeguards | `PRIMARY` | `PRIMARY` | `SUPPORTING` | Persian is needed for local/Iranian material; English for international empirical/method literature; Spanish for comparison mechanisms. |
| D8 Environment/visitor pressure | `PRIMARY` | `PRIMARY` | `SUPPORTING` | Iranian environmental context and international methods are both material; Spanish supports case mechanisms. |
| D9 Policy/practice transfer | `CONDITIONAL` | `PRIMARY` | `SUPPORTING` | Foundational and international transfer literature is expected mainly in English; Spanish adds applications; Persian is gap-driven. |
| D10 Spanish case discovery | `NOT_NORMALLY_REQUIRED` | `SUPPORTING` | `PRIMARY` | Original Spanish plans and institutional records require Spanish; English may reveal scholarly case leads. |
| D11 Data feasibility | `PRIMARY` | `SUPPORTING` | `PRIMARY` | Iranian and Spanish catalogues require their principal languages; English supports international metadata/standards. |
| D12 Specialist dependency | `SUPPORTING` | `PRIMARY` | `SUPPORTING` | International disciplinary standards are often English-indexed, with Persian/Spanish needed for source-specific interpretation. |

The 30-execution calibration ceiling is allocated dynamically to unresolved terminology in the most relevant domain–language cells. Not every domain must be tested in every language. The calibration plan must state the chosen cells and rationale before execution.

### 5.2 Place, territory, and institutional geography

| Function | English families | Persian families | Spanish families |
|---|---|---|---|
| Primary place | Kelardasht; Kalar Dasht; Kelar Dasht; Kalardasht | کلاردشت; کلار دشت | Kelardasht; Kalar Dasht; Irán |
| Administrative/context area | Mazandaran; Western Mazandaran; Alborz Mountains; Iran | مازندران; غرب مازندران; مازندران غربی; البرز; رشته‌کوه البرز; ایران; شهرستان کلاردشت | Mazandarán; oeste de Mazandarán; montes Alborz; provincia; municipio; comarca; territorio |
| Local/provincial public bodies (terminology, not verified entities) | governorate; municipality; provincial directorate; ministry; cultural-heritage authority | فرمانداری; شهرداری; اداره کل; استانداری; وزارت میراث فرهنگی، گردشگری و صنایع دستی; میراث فرهنگی مازندران | ayuntamiento; diputación; cabildo; comunidad autónoma; consejería; dirección general; ministerio; organismo gestor |

Transliteration variants are search aids only. The presence of a term in results cannot establish an official English name or administrative status.

### 5.3 Heritage and archaeology

| Function | English families | Persian families | Spanish families |
|---|---|---|---|
| Archaeology | archaeology; archaeological; excavation; survey; archaeological site; settlement; material culture | باستان‌شناسی; باستان شناسی; باستان‌شناختی; باستان شناختی; کاوش; بررسی باستان‌شناسی; محوطه باستانی; آثار باستانی | arqueología; arqueológico/a; excavación; prospección; yacimiento arqueológico; sitio arqueológico; cultura material |
| Cultural heritage | cultural heritage; tangible heritage; intangible heritage; historic monument; heritage value/significance | میراث فرهنگی; میراث ملموس; میراث ناملموس; اثر تاریخی; آثار تاریخی; ارزش میراثی; اهمیت فرهنگی | patrimonio cultural; patrimonio material; patrimonio inmaterial; monumento histórico; valor patrimonial; significación cultural |
| Registration/protection | heritage register; inventory; designation; listed/protected property; protected site | ثبت ملی; فهرست آثار ملی; ثبت آثار; اثر ثبت‌شده; حفاظت; حریم اثر | registro de patrimonio; inventario; catálogo; declaración; bien protegido; Bien de Interés Cultural; BIC; entorno de protección |
| Conservation | conservation; preservation; restoration; preventive conservation; condition; vulnerability; monitoring | حفاظت; صیانت; نگهداری; مرمت; حفاظت پیشگیرانه; وضعیت حفاظتی; آسیب‌پذیری; پایش | conservación; preservación; restauración; conservación preventiva; estado de conservación; vulnerabilidad; seguimiento |
| Heritage institutions/facilities | museum; local museum; heritage centre; archaeological workshop/laboratory; cultural-heritage office | موزه; موزه محلی; پایگاه میراث فرهنگی; مرکز میراث; کارگاه باستان‌شناسی; کارگاه باستان شناسی; اداره میراث فرهنگی | museo; museo local; centro de interpretación; centro patrimonial; taller/laboratorio arqueológico; oficina de patrimonio |

### 5.4 Initiatives, planning, implementation, and governance

| Function | English families | Persian families | Spanish families |
|---|---|---|---|
| Initiative maturity | announcement; public statement; project; programme; plan; budget; funding; contract; implementation; operation; evaluation | اعلام; خبر; اظهارات; پروژه; طرح; برنامه; بودجه; اعتبار; تأمین مالی; قرارداد; اجرا; بهره‌برداری; ارزیابی | anuncio; declaración; proyecto; programa; plan; presupuesto; financiación; contrato; ejecución; implantación; funcionamiento; evaluación |
| Governance | heritage governance; institutional arrangement; mandate; competence; coordination; accountability; enforcement; capacity | حکمرانی میراث; مدیریت میراث; ساختار نهادی; وظایف; اختیارات; هماهنگی; پاسخگویی; نظارت; ضمانت اجرا; ظرفیت نهادی | gobernanza del patrimonio; arreglo institucional; mandato; competencia; coordinación; rendición de cuentas; cumplimiento; capacidad institucional |
| Territorial/destination planning | territorial planning; spatial planning; rural planning; mountain planning; destination planning; destination governance | برنامه‌ریزی سرزمینی; برنامه ریزی سرزمینی; آمایش سرزمین; برنامه‌ریزی روستایی; برنامه‌ریزی مقصد; مدیریت مقصد; حکمرانی مقصد | ordenación del territorio; planificación territorial; planificación rural; planificación de montaña; planificación de destinos; gobernanza de destinos |

`CONSERVATION READINESS` remains a project analytical construct, but the literal phrase `conservation readiness` is demoted as a primary retrieval phrase. Future domain-specific retrieval should prioritize, without treating as synonyms, `heritage conservation`, `conservation planning`, `heritage management`, `management capacity`, `institutional capacity`, `governance capacity`, `preventive conservation`, and `conservation governance`. **ANALYTICAL CONCEPT ≠ PRIMARY SEARCH TERM.**

### 5.5 Tourism, visitor management, environment, and community

| Function | English families | Persian families | Spanish families |
|---|---|---|---|
| Heritage-related tourism | heritage tourism; cultural tourism; archaeotourism; archaeological tourism; tourism development | گردشگری میراث; گردشگری فرهنگی; گردشگری باستان‌شناختی; گردشگری باستان شناسی; توسعه گردشگری | turismo patrimonial; turismo cultural; arqueoturismo; turismo arqueológico; desarrollo turístico |
| Sustainable destination | sustainable tourism; sustainable destination; responsible tourism; destination management; tourism planning | گردشگری پایدار; مقصد پایدار; گردشگری مسئولانه; مدیریت مقصد; برنامه‌ریزی گردشگری | turismo sostenible; destino sostenible; turismo responsable; gestión de destinos; planificación turística |
| Visitor pressure/management | visitor management; visitor flow; visitation; carrying capacity; limits of acceptable change; crowding; over-visitation; demand management | مدیریت بازدیدکنندگان; مدیریت بازدید; جریان بازدیدکننده; بازدید; ظرفیت برد; حدود تغییر قابل قبول; ازدحام; فشار گردشگری; مدیریت تقاضا | gestión de visitantes; flujo de visitantes; afluencia; capacidad de carga; límites de cambio aceptable; masificación; presión turística; gestión de la demanda |
| Environment/protected landscape | environmental sustainability; protected area; protected landscape; national park; ecological impact; landscape conservation | پایداری محیط‌زیستی; پایداری زیست‌محیطی; منطقه حفاظت‌شده; منطقه حفاظت شده; چشم‌انداز حفاظت‌شده; پارک ملی; اثرات زیست‌محیطی; حفاظت منظر | sostenibilidad ambiental; espacio protegido; paisaje protegido; parque natural; parque nacional; impacto ambiental; conservación del paisaje |
| Community and safeguards | local community; participation; co-management; decision authority; stakeholder; local benefit; benefit sharing; livelihoods; displacement; social safeguard | جامعه محلی; مشارکت محلی; مشارکت جامعه; مدیریت مشارکتی; اختیار تصمیم‌گیری; ذی‌نفعان; منافع محلی; توزیع منافع; معیشت; جابه‌جایی; حفاظت اجتماعی | comunidad local; participación comunitaria; participación ciudadana; cogestión; poder de decisión; partes interesadas; beneficio local; reparto de beneficios; medios de vida; desplazamiento; salvaguardas sociales |

“Carrying capacity” terms are discovery vocabulary, not endorsement of a single-number model.

### 5.6 Transfer, comparison, evidence, and expertise

| Function | English families | Persian families | Spanish families |
|---|---|---|---|
| Policy/practice transfer | policy transfer; practice transfer; lesson drawing; policy learning; policy mobility; institutional transplantation; transfer failure; adaptation; non-transferability | انتقال سیاست; انتقال تجربه; انتقال رویه; یادگیری سیاستی; درس‌آموزی; بومی‌سازی; سازگارسازی; شکست انتقال; عدم انتقال‌پذیری | transferencia de políticas; transferencia de prácticas; extracción de lecciones; aprendizaje de políticas; movilidad de políticas; trasplante institucional; fracaso de transferencia; adaptación; no transferibilidad |
| Comparison | comparative case study; case selection; comparability; contextual conditions; mechanism; functional equivalent | مطالعه تطبیقی; مطالعه موردی تطبیقی; انتخاب مورد; مقایسه‌پذیری; شرایط زمینه‌ای; سازوکار; معادل کارکردی | estudio comparado; estudio de casos comparado; selección de casos; comparabilidad; condiciones contextuales; mecanismo; equivalente funcional |
| Data availability | open data; dataset; inventory; metadata; statistics; spatial data; geospatial portal; administrative boundary; licence | داده باز; مجموعه داده; فهرست; فراداده; آمار; داده مکانی; داده جغرافیایی; سامانه اطلاعات مکانی; مرز اداری; مجوز استفاده | datos abiertos; conjunto de datos; inventario; metadatos; estadísticas; datos espaciales; datos geográficos; geoportal; límite administrativo; licencia |
| Specialist dependency | archaeological interpretation; conservation assessment; ecological assessment; legal interpretation; transport engineering; expert review | تفسیر باستان‌شناسی; ارزیابی حفاظت; ارزیابی زیست‌محیطی; تفسیر حقوقی; مهندسی حمل‌ونقل; بررسی تخصصی | interpretación arqueológica; evaluación de conservación; evaluación ecológica; interpretación jurídica; ingeniería del transporte; revisión especializada |

`ADAPTIVE POLICY / PRACTICE TRANSFER` remains the project-level analytical framing, but `adaptive transfer` is demoted as a primary indexing phrase. Formal academic retrieval should prioritize, while preserving conceptual distinctions among, `policy transfer`, `lesson drawing`, `policy learning`, `policy mobility`, `institutional transfer`, `policy adaptation`, and `contextual adaptation`. **PROJECT ANALYTICAL LANGUAGE ≠ DATABASE INDEXING LANGUAGE.**

## 6. Candidate source environments

Naming an environment does not assert access, coverage, reliability, or permission. Stage B calibrated terminology and general-web retrieval behaviour; it did not verify native-interface syntax or coverage for untested environments. Before any Stage C formal-query freeze, every proposed formal environment must be classified as `VERIFIED` (access and relevant search behaviour sufficiently confirmed), `CONDITIONAL_UNVERIFIED` (potentially useful, but native access, syntax, or coverage not yet verified), or `EXCLUDED` (unavailable, inappropriate, redundant, or not required), with access basis and authentication method recorded.

### 6.1 Primary and authoritative environments

- Iranian national government and ministry websites relevant to cultural heritage, tourism, environment, statistics, law, planning, and geospatial data.
- Public Mazandaran provincial and Kelardasht/local authority websites, where identifiable and lawfully accessible.
- Public Iranian legal/planning repositories, heritage registers, statistical portals, open-data/geospatial catalogues, gazettes, budgets, procurement or implementation records where available.
- Spanish national, autonomous-community, provincial/island, municipal, heritage, tourism, protected-area, statistical, planning, legal-gazette, open-data, and geospatial portals.
- International authoritative catalogues or records where directly relevant, including UNESCO records; inclusion does not substitute for national/local evidence.

Exact institutions, official names, domains, search interfaces, archive status, and access limitations must be verified in an authorized stage rather than assumed from memory.

### 6.2 Academic environments

- Cross-disciplinary discovery: Google Scholar; DOI/metadata services such as Crossref; publisher platforms.
- Subscription indexes only if legitimately available: Scopus and Web of Science.
- Spanish/Ibero-American: Dialnet and relevant institutional/university repositories; other indexes only after access/coverage verification.
- Persian/Iranian candidates: SID, Magiran, IranDoc/Ganj, Civilica, Noormags, university repositories, and publisher platforms—each subject to lawful-access, metadata-quality, disciplinary-coverage, and full-text checks.
- Library catalogues, dissertation repositories, and institutional repositories where methods and bibliographic identity can be assessed.

Search-engine presence alone does not establish academic status. Predatory, duplicate, or unverifiable publication venues are downgraded or excluded.

### 6.3 Technical and institutional environments

- UNESCO, ICOMOS, ICCROM, UN Tourism, and other directly relevant international institutional collections.
- Recognized heritage-conservation, protected-area, planning, community-safeguard, and professional bodies.
- Spanish heritage/tourism/planning bodies and observatories, assessed for mandate, method, and possible promotional interest.
- University and research-institute technical reports with identifiable authorship, method, and provenance.

Institutional prestige does not remove the need to assess method, remit, version, and conflicts.

### 6.4 Secondary discovery environments

- Attributable journalism, institutional news, professional reporting, archived public announcements, and public-facing organizational communications.
- General web search for claim discovery, institutional-name discovery, document-location leads, and public-discourse analysis only.
- Social media only where it is the original attributable statement under study or a lead to an official record; screenshots/reposts are insufficient without provenance.

Secondary material cannot replace reasonably obtainable primary verification. Syndication and copied press releases are one evidence lineage.

## 7. Source-hierarchy routing by domain

| Domain | Preferred tiers and evidence | Permitted role of weaker sources | Critical downgrade/verification rule |
|---|---|---|---|
| D1 Heritage significance | A original archaeological/heritage records; B qualified scholarship; C technical assessment | D/E discover names, sites, or documents | Promotional significance language cannot establish archaeological/cultural significance. |
| D2 Institutions/initiatives | A mandate, legal/administrative, implementation and operational records; B/C independent assessment | D/E identify claimed institution/initiative or public narrative | An announcement/page verifies only that a statement was made unless operation is separately evidenced. |
| D3 Government action | A adopted plan, budget, contract, implementation/operation record, original statement | D locate the underlying official record; E discourse only | Plan, funding, implementation, operation, and outcome are separate claim statuses. |
| D4 Local scholarship | B peer-reviewed work and assessable theses/books; A/C original records | D/E citation leads | Abstract/snippet-only access cannot support extracted findings. |
| D5 Heritage tourism | B empirical/conceptual research; A implemented instruments; C transparent guidance | D/E identify debated cases/claims | “Best practice” labels and awards are not evidence of effect. |
| D6 Governance/readiness | A law, mandates, plans, budgets, monitoring; B governance/conservation research; C standards | D/E discovery | Formal authority/designation does not prove capacity, enforcement, or outcome. |
| D7 Community | B/A empirical local research with ethical/method transparency; C safeguard methods | D/E identify claims requiring verification | Official/promotional representation cannot establish community views, consent, benefit, or harm. |
| D8 Environment/pressure | A monitoring/plans/data; B empirical methods; C technical guidance | D/E issue discovery | No ecological, carrying-capacity, or pressure conclusion without fit-for-purpose data and expertise. |
| D9 Transfer | B foundational/current theory and empirical research; A/C evaluations | D/E terminology or case leads | Transferability requires mechanism and context analysis, not source-country success claims. |
| D10 Spanish discovery | A official planning/heritage/protected-area records; B case analysis; C documented institutional cases | D/E candidate leads only | Discovery, eligibility, comparability, shortlisting, and selection remain separate. |
| D11 Data feasibility | A/C custodian metadata, licence, coverage, version and access terms | D/E point to a catalogue only | Catalogue presence does not establish access, quality, fitness, legality, or currentness. |
| D12 Specialist dependency | A–C disciplinary standards/methods and documented interpretive demand | D/E alert only | If indispensable review is unavailable, narrow, remove, defer, or modify; do not infer. |

## 8. Initial claim families

These prefixes organize future claims without asserting substantive content:

| Prefix | Family | Typical question |
|---|---|---|
| `KEL-HER-*` | Heritage significance/designation/condition | What heritage-related proposition is actually documented, by whom, and at what evidentiary level? |
| `KEL-ARC-*` | Archaeological evidence/interpretation | What archaeological evidence or interpretation is source-reported, and what requires specialist review? |
| `KEL-INST-*` | Heritage institutions/facilities | Does a claimed institution/facility have documented mandate, existence, operation, and continuity? |
| `KEL-INIT-*` | Heritage/tourism initiatives | Is the item an announcement, statement, project, programme, plan, funded action, implementation, institution, or outcome claim? |
| `KEL-GOV-*` | Governance/institutional arrangements | What authority, coordination, capacity, accountability, or implementation is documented? |
| `KEL-COM-*` | Community participation/benefit/safeguards | What empirical evidence exists, whose perspective is represented, and what cannot be inferred? |
| `KEL-ENV-*` | Environment/visitor pressure | What environmental or pressure-management need is evidenced and competence-appropriate? |
| `LIT-CON-*` | Conceptual/literature coherence | Can the relevant research domains be connected without conceptual or disciplinary overreach? |
| `ESP-CASE-*` | Spanish candidate discovery/comparability | What makes a candidate relevant on a specified dimension and where is it mismatched? |
| `TRF-*` | Transfer/adaptation/rejection | Which mechanism, conditions, resource assumptions, and failure risks would require testing? |
| `DATA-*` | Data existence/access/fitness | Does a dataset/document appear to exist, and are access, licence, coverage, granularity, and sensitivity suitable? |
| `SPEC-*` | Specialist dependency | Which claim requires which expertise, at what decision point, and what fallback is available? |

Future claims must use the independent `claim_nature` and `current_status` dimensions in `evidence/CLAIM_REGISTER.csv`. Verifying that a source made a statement does not verify the statement’s content.

## 9. Inclusion criteria

A record may enter the later formal screening set only when all mandatory conditions are met:

1. **Question relevance:** It bears directly on at least one named Gate 0 question, domain, or claim family.
2. **Geographic fit:** Its place/scale is explicit. Contextual material outside Kelardasht is labelled and not silently generalized.
3. **Temporal fit:** Its date/version is appropriate to the claim type under Section 11; older evidence is not rejected solely for age.
4. **Identifiable provenance:** Author/institution, title, date/version where available, source location, and publication/record type can be identified.
5. **Authority/method fit:** The source has suitable institutional remit or a sufficiently transparent method for the intended claim.
6. **Evidence directness:** The record contains or points to information capable of supporting, qualifying, contradicting, or contextualizing a defined claim; indirect material is labelled.
7. **Language handling:** It can be assessed under `docs/LANGUAGE_PROTOCOL.md`; consequential ambiguity is flagged for verification.
8. **Lawful accessibility:** Access and intended use are lawful; redistribution permission is assessed separately from research access.
9. **Version and duplication control:** The authoritative/current version or relationship among versions can be recorded; duplicate lineages are linked rather than counted independently.
10. **Scope discipline:** The record can inform feasibility without expanding into an unauthorized intervention, advocacy, or later-gate analysis.

Academic literature additionally requires assessable bibliographic identity and sufficient method/full-text access for the claimed use. Primary administrative material may be included for formal status even when it cannot establish implementation or effectiveness.

## 10. Exclusion, downgrade, and discovery-only rules

### Exclude from evidentiary use

- unattributed or untraceable claims;
- SEO/content-farm or automatically aggregated pages without recoverable provenance;
- AI-generated summaries presented as sources;
- fabricated, materially corrupted, unlawfully obtained, leaked, or access-controlled material lacking authorization;
- inaccessible citations with metadata too incomplete to authenticate;
- generic destination marketing with no Gate 0-relevant claim or traceable evidence;
- material unrelated to a named Gate question/domain;
- exact sensitive-site data unnecessary to the research question;
- claims whose only possible use requires unavailable specialist interpretation and cannot be narrowed to a competence-appropriate proposition.

### Downgrade or use only for discovery

- tourism promotion, awards, branding, and public-relations copy;
- unsourced social posts or reposts;
- journalism that does not expose the underlying evidence;
- abstracts/snippets when the finding requires full-text assessment;
- duplicated/syndicated reporting or copied press releases;
- undated pages for time-sensitive initiative-status claims;
- institution-authored performance claims lacking independent or operational evidence.

### Discovery source versus evidentiary source

A `DISCOVERY_SOURCE` may identify a claim, spelling, institution, initiative, candidate case, document title, or source lead. It does not support the claim unless separately assessed and registered as an `EVIDENTIARY_SOURCE`. A record may have both roles for different bounded claims—for example, an original official announcement can evidence that the announcement occurred while not evidencing successful implementation.

Weak leads are retained in the future search log with a disposition rather than silently discarded or elevated.

## 11. Temporal logic

| Evidence function | Temporal rule |
|---|---|
| Archaeological discovery, chronology, historical settlement, and heritage significance | No automatic recent-date cutoff. Historical scholarship may remain important; assess subsequent revision, method, and present interpretive standing. |
| Heritage designation/register status | Seek the original designation and the most current authoritative status/version. Record amendments or delisting where found. |
| Site condition/vulnerability | Require time-appropriate evidence; older condition reports cannot establish current condition without corroboration. |
| Current institutions and initiative maturity | Prioritize current records and a traceable chronology. For ongoing status, seek recent confirmation and version/update dates. |
| Plans, programmes, funding, implementation, and operation | Cover formation through current status as needed; distinguish adoption, validity period, funding, execution, completion, continued operation, and evaluation. |
| Kelardasht/Western Mazandaran academic landscape | No uniform cutoff. Use older foundational/local work and newer revision where relevant. |
| Conservation/governance/community/environmental methods | Favor current standards and evidence while retaining foundational work needed to explain concepts or institutional evolution. |
| Spanish planning mechanisms | Include the current applicable framework plus sufficient historical evolution to understand the mechanism and implementation pathway. |
| Policy/practice transfer | Include foundational theory and recent critical/empirical applications; age is interpreted by conceptual function. |
| Data feasibility | Require current catalogue/access/licence/version information; historical datasets may still be relevant if coverage matches the question. |

Stage C will define justified platform-specific date filters by domain. Absence of a filter must be deliberate and recorded.

## 12. Geographic logic

1. **Primary unit:** Kelardasht. Search records must distinguish the city/town, county or other administrative unit, valley/landscape, destination label, and any site-specific unit encountered.
2. **Immediate context:** Western Mazandaran may be used when it supplies a documented functional, historical, landscape, or institutional context.
3. **Provincial context:** Mazandaran Province may inform law, administration, plans, datasets, or comparison within the province.
4. **Regional context:** The Alborz mountain region may inform specifically justified landscape, mobility, archaeology, or environmental questions.
5. **National context:** Iranian law, institutions, planning systems, and datasets may define the framework affecting Kelardasht.
6. **Inference rule:** Evidence at national, regional, or provincial scale cannot be attributed to Kelardasht without explicit linkage or a documented, bounded inference.
7. **Spanish discovery:** The initial discovery frame is national, with autonomous-community and local sources. Later eligibility requires a bounded case-level unit and dimension-specific relevance.
8. **Other geographies:** International or third-country evidence is allowed only for concepts/methods and may not become an unlogged comparison expansion.

## 13. Stage B calibration design and closure

### 13.1 Purpose

Calibration exists only to detect terminology, transliteration, spelling, controlled-vocabulary, indexing, institutional-name, and query-syntax blind spots before exact formal queries are frozen.

### 13.2 Maximum scope

- **Maximum query executions:** 30 total; this is a ceiling, not a target.
- **Language allocation:** no fixed language quotas. Executions are assigned according to the pre-declared Domain × Language relevance logic in Section 5.1 and the terminology uncertainties that remain material.
- **Environment ceiling:** no more than eight owner-approved environments across official-web, general discovery, academic index, and institutional catalogue types; access must first be recorded as lawful and available.
- **Inspection ceiling per execution:** the search interface’s reported count plus permitted calibration fields for at most the first 20 displayed records. No bulk export, full-text collection, dataset download, corpus/source archiving, substantive citation chaining, or evidence extraction.
- **Domain coverage:** prioritize D1–D4 for Persian/local terminology, D5–D9 for cross-disciplinary vocabulary, D10 for Spanish planning/case vocabulary, and D11–D12 for catalogue and specialist-dependency terminology. Not every domain receives every language.
- **Stop early:** stop when a planned family has yielded stable terminology/indexing information or when further inspection would become substantive source assessment.

If the calibration reaches 30 executions while material terminology or indexing uncertainty remains, calibration must stop. The unresolved issue and affected domain/language cells must be reported, and any extension requires separate owner authorization. The ceiling cannot be extended through ordinary change control.

### 13.3 Query-execution definition

One `QUERY_EXECUTION` is one distinct query string executed in one identified search environment under one defined filter configuration.

A materially different query string, search environment, language version, date filter, geographic filter, searched field, or search mode counts as a separate execution when it changes retrieval behaviour. Re-running the same configuration also receives its own execution record and links to the prior execution. Minor navigation, pagination, sorting inspection, or opening permitted metadata within the same result set does not constitute a new execution unless it changes the query or retrieval configuration.

The future search log must make the count reconstructable through the exact query, environment, language, searched fields/mode, filters, execution sequence, and any parent/repeat relationship.

### 13.4 Permitted inspection and learning

Calibration may inspect, solely to understand terminology and indexing:

- bibliographic metadata;
- titles and abstracts;
- author keywords and database indexing/controlled terms;
- official-page titles and headings;
- search-result snippets; and
- institutional terminology visible on source landing pages.

Inspection is limited to the calibration purpose. Reading an abstract or landing-page heading does not authorize extraction or assessment of substantive findings.

Calibration may identify:

- spelling/transliteration and spacing/zero-width-joiner variants;
- synonyms, official terminology, acronyms, and controlled subject headings;
- database field and Boolean/phrase syntax;
- obviously overbroad or empty keyword combinations;
- missing negative/critical terms;
- official institutional name variants and likely document-type vocabulary;
- which candidate environment indexes which language/document type.

### 13.5 Prohibited conclusions and actions

Calibration cannot establish source exhaustiveness, heritage significance, initiative status, data availability/fitness, research gaps, comparative suitability, transferability, community conditions, environmental pressure, specialist need, or any Gate verdict. It cannot conduct substantive evidence extraction; download or archive research corpora; populate `CLAIM_REGISTER.csv`, `EVIDENCE_REGISTER.csv`, or `LITERATURE_MATRIX.csv` with substantive records; verify Kelardasht claims; conduct citation-chain research beyond terminology identification; or treat calibration results as the formal evidence base.

### 13.6 Separation and record handling

- Every execution receives a `CAL-*` search ID and `search_stage=CALIBRATION`.
- Result records receive no evidence/literature/case IDs during calibration.
- Only terminology/indexing observations and minimal locator data needed to identify a potentially important item may be recorded. Such a pointer must be labelled exactly `CALIBRATION LEAD — NOT YET EVIDENCE`; it must not include claim evaluation.
- A calibration lead may enter formal screening only during a later explicitly authorized evidence-acquisition stage, with a formal search ID and ordinary eligibility review. Stage C cannot silently promote a lead to evidence, assign it claim status, or enter it in `EVIDENCE_REGISTER.csv`, `CLAIM_REGISTER.csv`, or `LITERATURE_MATRIX.csv`.
- Calibration files must be stored separately from formal logs/exports and labelled non-evidentiary.

### 13.7 Calibration change record

For each proposed vocabulary or architecture change, record the prior term/family, observed indexing problem, environment/language, proposed replacement/addition/removal, expected scope effect, decision, reviewer, date, and whether formal searches would require repetition.

### 13.8 Formal-query freeze after calibration

Stage C converted approved families into platform-specific strings or conditional templates and recorded query syntax, fields, filters, date/geographic limits, execution priority, and expected purpose. Each formal environment is classified under Section 6. An exact executable query cannot be represented as operationally frozen for a `CONDITIONAL_UNVERIFIED` environment; such environments retain only a query template or conceptual query family pending legitimate native access and syntax/coverage verification. Decision D-0021 approved and froze the versioned formal set without authorizing execution. Rejected calibration changes remain visible. The authoritative Stage C implementation is `literature/FORMAL_SEARCH_PLAN.md` with its two CSV registers.

### 13.9 Owner-approved Stage B closure

Stage B closed as `CALIBRATION SUFFICIENT` after 28 of the maximum 30 query executions. The two remaining executions are intentionally unused; no extension is authorized. The execution record is `literature/SEARCH_LOG.csv`, the six retained pointers remain `CALIBRATION LEAD — NOT YET EVIDENCE`, and the approved interpretations and native-environment limitations are documented in `literature/CALIBRATION_REPORT.md` and Decision D-0019. Decision D-0020 opened Stage C design; Decision D-0021 closed and froze it. Every query execution and substantive search function remains unauthorized.

## 14. Future search-log design

The future log will contain one row per executed query—not one row per source. The recommended schema is:

| Field | Function |
|---|---|
| `search_id` | Stable ID (`CAL-*` or `FOR-*`). |
| `execution_sequence` | Monotonic count within the authorized search stage. |
| `search_stage` | `CALIBRATION` or `FORMAL`. |
| `execution_status` | `PLANNED`, `EXECUTED`, `PARTIAL`, `FAILED`, `REPEATED`, or `VOID`. |
| `parent_execution_id` | Prior execution repeated or modified, where applicable. |
| `executed_at` | ISO date/time with timezone. |
| `researcher` | Person executing/reviewing. |
| `research_domain` | D1–D12. |
| `gate_question_ids` | Linked Q1–Q10. |
| `claim_families` | Applicable organizational prefixes. |
| `purpose` | Bounded reason for this execution. |
| `language` | Primary query language; note mixed-language use. |
| `database_or_environment` | Named platform/site/catalogue. |
| `environment_type` | Official, academic, technical/institutional, or secondary discovery. |
| `access_basis` | Public, institutional subscription, owner entitlement, or other lawful basis. |
| `query_version` | Version frozen for the execution. |
| `exact_query` | Exact submitted string, preserved verbatim. |
| `search_mode` | Basic/advanced, site search, catalogue, fielded search, or other mode affecting retrieval. |
| `fields_searched` | Title, abstract, full text, subject, site search, etc. |
| `filter_configuration` | Complete applied platform filters as one reconstructable configuration. |
| `temporal_constraint` | Date rule actually applied. |
| `geographic_constraint` | Place/scale rule actually applied. |
| `sort_order` | Relevance, date, citation, or platform default. |
| `reported_results_count` | Platform-reported count; record instability/estimate. |
| `result_pages_or_records_inspected` | Actual bounded inspection extent. |
| `records_screened` | Count screened under the stage rules. |
| `records_retained` | Count retained for later formal processing; zero for calibration evidence. |
| `duplicates_identified` | Duplicates/lineage count if assessed. |
| `exclusion_summary` | Compact reason counts or link to screening log. |
| `terminology_observation` | Calibration/indexing observation, if applicable. |
| `change_id` | Link to search-change record. |
| `repeat_required` | `YES`, `NO`, or `UNDETERMINED`. |
| `log_or_export_location` | Controlled local path where an authorized artifact resides. |
| `limitations` | Access, indexing, outage, personalization, truncation, or reproducibility caveat. |
| `notes` | Minimal additional context. |

Together, `exact_query`, `database_or_environment`, `language`, `search_mode`, `fields_searched`, `filter_configuration`, `temporal_constraint`, and `geographic_constraint` define the execution unit. The log must allow the 30-execution calibration ceiling to be independently reconstructed.

An empty `literature/SEARCH_LOG.csv` is **proposed but not created in Stage A**. It should be generated from the owner-frozen schema immediately before an authorized Stage B, avoiding a premature operational artifact.

## 15. Search change control

After the formal query set is frozen, no silent query drift is permitted. Each amendment receives `SCHG-####` and records:

- affected domain, environment, language, and query version;
- previous exact query/version and the proposed new version;
- observed terminology, indexing, coverage, syntax, or access problem;
- evidence for the problem from calibration/formal logs (not a desired result);
- nature of change: correction, expansion, narrowing, substitution, environment migration, or filter change;
- anticipated effect on recall, precision, language/geographic/temporal coverage, and comparability;
- decision owner, approval date, and implementation date;
- whether earlier searches must be repeated, and if not, why not;
- affected search IDs and downstream records;
- version superseded and retained audit trail.

Emergency technical corrections (for example, invalid syntax) are still logged. A change motivated by seeing desirable/undesirable findings receives heightened review for confirmation bias. Architecture-level scope changes require an amended protocol and owner authorization.

## 16. Stopping logic

Gate 0 seeks decision sufficiency, not exhaustive global coverage. It must not be described as a systematic review unless a later protocol actually satisfies that methodology.

### 16.1 Domain-level stopping conditions

A domain may stop only when:

1. its gate-critical claim families have been searched through the relevant preferred source environments and languages that are lawfully available;
2. authoritative/primary pathways have been attempted and their availability or absence documented;
3. relevant supporting, contradictory, and critical/failure evidence pathways have been represented where applicable;
4. repeated appropriately varied formal searches primarily retrieve already screened sources/lineages and do not add material capable of changing a Gate decision;
5. temporal and geographic coverage is adequate for the claim type, or the shortfall is explicit;
6. language, access, translation, sensitivity, and specialist limitations are recorded; and
7. remaining gaps are classified as resolvable later, redesign-triggering, or structural.

Repeated retrieval alone is insufficient when a language, source tier, or decisive claim family has not been addressed.

### 16.2 Overall Gate 0 search stopping conditions

Stop formal Gate 0 searching when:

- every Gate question has enough registered evidence to be assessed or a documented reason it is `NOT_ASSESSABLE`;
- the verified/unsupported/contradicted status of gate-critical claim families is visible;
- source-type and English/Persian/Spanish coverage is proportionate to domain relevance;
- candidate Spanish discovery is broad enough to test whether systematic comparison is plausible without selecting a winner;
- data and specialist dependencies are explicit;
- additional searches are unlikely to change GO/MODIFY/NO-GO reasoning, based on logged yield rather than fatigue or deadline; and
- unresolved gaps remain visible in the synthesis.

Time and source counts are monitoring constraints, not scientific stopping rules. The provisional two-to-three-week horizon cannot override these conditions.

### 16.3 Stop-early conditions

Pause or stop a domain when continued searching would require unlawful/restricted access, expose vulnerable heritage, create disproportionate personal-data risk, exceed owner competence without a narrowing route, or expand beyond Gate 0. A structural evidence gap is a legitimate finding.

## 17. Spanish candidate-case discovery architecture

Candidate discovery and candidate screening are separate stages.

### 17.1 Discovery routes

Later authorized discovery should use multiple routes to reduce visibility bias:

1. official Spanish heritage inventories/catalogues and archaeological/cultural planning instruments;
2. protected-landscape, rural/mountain, territorial, and visitor-management plans;
3. peer-reviewed Spanish case literature and university/institutional repositories;
4. recognized technical/professional case collections with explicit methods;
5. bounded citation/instrument chaining from relevant mechanisms;
6. secondary reporting only to identify a case or underlying primary documentation.

### 17.2 Discovery attributes

Record only enough to support later eligibility review: candidate name/unit, discovery route, territory type, heritage dimension, possible protected-landscape relationship, apparent governance/visitor/community/sustainability mechanism, documentation environment, source lead, and evident mismatch/risk. Do not assign a comparability score during discovery.

### 17.3 Transition to screening

A discovered candidate enters later screening only if it can plausibly be bounded as a territorial/governance unit and linked to at least one verified Kelardasht problem dimension. Screening then uses `cases/spain/CASE_SCREENING.csv` and the Gate 0 protocol’s eligibility, dimension-specific comparability, mechanism relevance, evidence availability, mismatch, and bias controls.

No aggregate weighting, ranking, shortlist, or winner is produced during discovery. Famous destinations and Smart Tourism designations receive no privileged entry route.

## 18. Data-feasibility search pathway

Data-feasibility searching will be separately logged under D11 and will look for metadata—not acquire or analyze datasets.

| Data class | Feasibility questions |
|---|---|
| Heritage inventories/registers | Custodian, public access, coverage, object/site sensitivity, coordinates, update status, legal/redistribution terms. |
| Statistical data | Producer, geography, period, variables, definitions, sampling/administrative basis, downloadable format, licence. |
| Geospatial/administrative boundaries | Custodian, scale, CRS/format metadata, boundary version, access, licence, sensitivity. |
| Transport/accessibility | Network/status data owner, temporal validity, coverage, operational versus planned status, licence; no engineering inference. |
| Protected areas/environment | Designation/management authority, boundary/monitoring metadata, currentness, restrictions, ecological expertise needed. |
| Tourism statistics | Geographic resolution, visitor/tourist definition, accommodation coverage, seasonality, suppression, method, currentness. |
| Planning/legal documents | Adoption authority/date, legal status, validity, amendments, implementation/monitoring evidence, public access. |

Future feasibility status will use `ACCESSIBLE`, `CONDITIONAL`, `RESTRICTED`, `UNAVAILABLE`, or `UNKNOWN`. “Accessible” does not mean fit for purpose. No source file, dataset, map service, or coordinate layer will be downloaded or queried for content under Stage A or calibration authority.

## 19. Specialist-dependency pathway

During later formal screening, flag rather than resolve claims involving:

- archaeological dating, authenticity, site interpretation, or significance;
- heritage condition, intervention need, conservation technique, or vulnerability;
- ecological state, impact, carrying capacity, or protected-area effects;
- legal authority, compliance, rights, or instrument interpretation;
- transport network status, safety, capacity, causality, or engineering need;
- statistical inference beyond documented descriptive use;
- community consent, representativeness, cultural meaning, or human-participant inference;
- consequential technical/legal translation.

Each `SPEC-*` record should state the exact claim, expertise required, why ordinary planning analysis is insufficient, decision consequence, and fallback: `NARROW`, `REMOVE`, `DEFER`, or `MODIFY_SCOPE`. Stage A does not search for or contact specialists.

## 20. Ethical and security controls

- Do not search specifically for protected coordinates, unpublished site locations, looting-related information, leaked documents, credentials, or access-control bypasses.
- Prefer aggregated place terms where exact site identity is unnecessary.
- Do not reproduce exact sensitive locations in queries, logs, filenames, excerpts, screenshots, or outputs.
- If sensitive information appears incidentally, stop expanding it; record only a generalized existence/sensitivity note and controlled locator where lawful.
- Do not download restricted databases or redistribute copyrighted documents without permission.
- Minimize personal/contact data and do not collect stakeholder identities merely because they appear in public results.
- Respect robots, terms of service, rate limits, authentication boundaries, and database licences; no scraping is authorized by this architecture.
- Do not submit sensitive or restricted material to AI systems. AI may assist with design and later classification but is never a source.
- Preserve Persian originals and translation provenance; do not replace them with English-language secondary reporting when originals are accessible.

## 21. Bias and quality controls

The later search must actively monitor:

- confirmation bias toward heritage significance or tourism relevance;
- familiarity and Iran–Spain transfer bias;
- English-language and Latin-script indexing bias;
- official-source bias and institutional self-reporting;
- publication and positive-case/survivorship bias;
- Spain prestige, UNESCO, “smart,” urban, and data-availability bias;
- recency bias against older archaeology and age bias in favor of outdated initiative status;
- conflation of visibility with importance, designation with protection, plans with implementation, and access with sustainability;
- circular citation and syndicated-source inflation;
- disciplinary overreach and false precision.

For each domain, the formal freeze should specify at least one contradiction/critical vocabulary family and an explicit route to non-implementation or failure evidence where relevant.

## 22. Stage A completion and freeze criteria

Stage A is ready for owner freeze only if:

- D1–D12 have a bounded purpose, Gate link, source preference, and prohibited inference;
- English, Persian, and Spanish families cover relevant concepts while remaining provisional;
- candidate environments are explicit and access is not invented;
- source-tier routing, inclusion/exclusion, discovery/evidence distinction, and duplicate lineage rules are operational;
- temporal and geographic logic prevent silent generalization;
- calibration is capped, non-evidentiary, and separable;
- the future search log and change-control records are fully specified;
- stopping conditions are decision-oriented rather than volume-based;
- Spanish discovery remains separate from screening/selection;
- data feasibility is metadata-only;
- ethical, sensitive-site, translation, and specialist controls are explicit;
- no search, source retrieval, or register population occurred during design.

Owner freeze should assign a version and record any required corrections in the decision log. It must not authorize Stage B unless the owner does so separately and explicitly.

## Approval record

| Role | Name | Decision | Date | Conditions |
|---|---|---|---|---|
| Project owner | Soroush Karahrodi | Approved with required corrections applied | 2026-09-25 | Stage A freeze record. Stage B was opened by D-0018 and closed/approved by D-0019 after 28/30 executions. Stage C was opened by D-0020 and closed/frozen by D-0021; execution and evidence acquisition remain closed. |

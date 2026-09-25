# Language, Translation, and Transliteration Protocol

**Status:** Owner-approved Phase 0A baseline  
**Scope:** All research records and outputs  
**Canonical research language:** English

## Purpose

This protocol preserves the provenance and meaning of multilingual evidence while avoiding unnecessary duplicate documentation. It applies before any Persian, Spanish, or other non-English evidence enters the repository.

## Language roles

- **English:** canonical protocols, evidence records, methodological decisions, code, analysis, and reproducibility documentation.
- **Spanish:** later academic/professional dissemination where a mature, reviewed output has a defined audience.
- **Persian:** original Iranian evidence, official terminology, names, quotations, local material, and possible later Iranian-facing communication.

An English translation does not replace the original text.

## Owner language capability

- **Persian:** native-level owner review.
- **English:** advanced independent research use.
- **Spanish:** advanced independent academic/professional use.

These capabilities support source assessment but do not replace specialist or authoritative linguistic/domain review where legal, archaeological, highly technical, or institution-specific meaning materially affects a claim.

## Mandatory distinctions

Every material non-English passage must be identifiable as one of:

- **ORIGINAL TEXT:** exact source text, with location and language.
- **TRANSLATION:** meaning rendered in another language as closely as possible.
- **PARAPHRASE:** researcher’s condensed restatement.
- **INTERPRETATION:** analytical judgment derived from the source.

These forms must not be merged into a single unlabeled note.

## Evidence-record requirements

Where applicable, register:

- `source_language` using ISO 639-1 codes where available (`fa`, `es`, `en`);
- `original_title` and `english_title`;
- original and standardized institutional names;
- exact `source_locator` for each excerpt;
- `original_excerpt`, preserving original script;
- `english_translation` and/or `english_paraphrase`;
- `translation_status`, `translation_method`, `translator_or_tool`, and `translation_verified_by`;
- ambiguity, untranslatable terms, competing renderings, and consequences for the claim.

## Translation-status vocabulary

- `NOT_REQUIRED` — source is already in the working language for the recorded use.
- `PENDING` — translation is needed but absent.
- `AI_DRAFT` — machine/AI-assisted translation, not independently checked.
- `RESEARCHER_DRAFT` — translated by the owner/researcher, not independently checked.
- `VERIFIED_BILINGUAL` — checked by a named person competent in both languages.
- `VERIFIED_SPECIALIST` — checked by a named subject specialist where technical meaning matters.

Verification status concerns translation quality, not truth of the source claim.

## Translation procedure

1. Preserve the original title and material excerpt exactly as encountered.
2. Record the source location before translating.
3. Produce a close translation; use square brackets only for necessary supplied context.
4. Record the method and tool/person responsible.
5. Mark uncertainty rather than smoothing ambiguous text.
6. Create a separate paraphrase only when useful for analysis.
7. Obtain authoritative bilingual and/or domain-specialist verification before relying on a translation for a consequential, contested, legal, archaeological, highly technical, institution-specific, or gate-decisive claim when meaning materially affects interpretation.
8. If verification is unavailable, constrain the claim and record the limitation.

Machine translation may support discovery but cannot by itself settle terminological, legal, political, or archaeological ambiguity.

## Names and transliteration

Use the following provisional rules until Gate 0 evidence supports a project glossary:

1. Prefer the official or source-attested Latin form when an institution or place publishes one consistently.
2. Otherwise use a consistent, readable transliteration and preserve the Persian original on first material mention.
3. Do not silently normalize competing spellings; record aliases in notes and select a preferred project form with justification.
4. Preserve personal names in the form used by the person or their authoritative publication where known.
5. Do not translate institution names as if the English rendering were an official name; label it `standardized_english_name` unless official status is verified.

Current project convention: **Kelardasht (کلاردشت)** at first material mention and **Kelardasht** thereafter. Search strings may include spelling variants, all of which must be logged.

## Quotations and citations

- Quote only the portion required for the claim and respect copyright and database terms.
- Keep source punctuation and wording; mark omissions and additions conventionally.
- Cite the original source, not the translation tool.
- For translated quotations, label the translator or method and provide the original where lawful and proportionate.
- Never translate a quotation and present it as if it were the source’s original language.

## Quality control

Gate-decisive use is prohibited when a material translation is `PENDING` or when unresolved ambiguity could change the conclusion. AI-drafted translations may support search triage but must remain visibly provisional. Translation corrections are versioned; the previous text is not silently overwritten when a correction changes interpretation.

If appropriate verification cannot be obtained, narrow, remove, defer, or redesign the affected claim. Owner fluency and AI translation must not be presented as specialist validation.

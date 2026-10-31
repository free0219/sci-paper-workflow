# Evidence records

Use these schemas only when persistent evidence will be useful. Keep actual paper facts in project files. Follow existing project record conventions and versioning rather than creating competing indexes.

## Lightweight registry

Suggested columns:

| Paper ID | User aliases / original filename cue | Official title | Year / journal | DOI or stable URL | Topic / methods | Source path | Active note path | Verification summary |
|---|---|---|---|---|---|---|---|---|

Paper ID is stable across filenames and note revisions. Resolve DOI duplicates before assigning another ID; if DOI is absent, compare authoritative title/author/year metadata. Preserve alternative versions and their identity rather than silently conflating a preprint and final article.

Use project-relative source paths where possible; record an external local path only if needed for retrieval and keep it local. A row's verification summary is navigation only; claim-level records determine citation readiness.

## Selective paper note

Include only useful fields with actual evidence:

- Identity: title, authors, journal, year, DOI/stable URL, original PDF path and aliases.
- Source version: publisher version or manuscript version; retrieval/verification date; local fingerprint if available and useful. Do not fabricate a hash or metadata.
- Relevance: one or two sentences about the paper's use in this manuscript.
- Claim ID and scoped statement.
- Original-source observation/result, distinct from this project's proposed application.
- Location: PDF file page (1-based), printed page if available, section, figure/table; or HTML heading/anchor and URL.
- Verification level: METADATA_ONLY / ABSTRACT_ONLY / FULLTEXT_LOCATED / NEEDS_RECHECK.
- Support level: DIRECT / SUPPORTING / BACKGROUND / NOT_SUITABLE for the intended statement.
- Relevant conditions and limits on transfer to the present study.
- Verification basis: what was actually read or visually checked, and by whom (agent inspection versus user-provided statement).
- Intended use: current section or claim, not an automatic instruction to cite elsewhere.
- Important methods, figures, contradictions, and tags only when likely to be reused.

Store concise paraphrases and short locating anchors, not copied full text or large excerpts. A record with only a title and abstract must not be presented as full-text-verified.

## Project facts and record versions

Project facts should include: statement/value, unit, sample/condition/time, source location/version, status, and known conflicts. Distinguish user-established background from independently checked raw-data facts and proposed interpretations. An assistant-generated draft is not itself a new confirmed fact.

Create terminology, outline, model-framework, or experimental-fact files only as facts become useful and sourced. Do not prepopulate them using illustrative values from previous advice.

When the project lacks reliable Git history, use immutable versions, for example `literature_registry.v001.md` and `literature_notes/P001.v001.md`. Corrections go to a new version that identifies the superseded record. If an active-file map is used, version that map as well. For Git-managed text, use canonical paths only when the applicable project rules permit it. Preserve formal reports and raw/model artifacts separately as required.

On conflict, retain provenance for both values and mark the affected assertion unresolved. Do not overwrite the original observation or promote a plausible interpretation into a confirmed fact.

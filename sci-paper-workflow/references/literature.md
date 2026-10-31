# Literature: RECALL / DISCOVER → VERIFY → CACHE

Use the operations needed for the request. Recall is not mandatory when no relevant local source exists; discovery remains mandatory when requested by the user or project rules.

## Recall informal names

Search known aliases and the original filename stem in the active literature registry. If no registry exists or matches, use a targeted filename search in the local library. Search topic, method, remembered claim, official title, and author/year as needed. Read relevant notes, then first-page metadata or targeted passages of the most plausible candidates.

Informal aliases describing a topic or method are retrieval cues, not verified bibliographic identities or scientific conclusions. Do not rename the PDFs. If multiple candidates remain, distinguish them using material, method, year, and actual findings. Ask for clarification only when unresolved identity would materially affect the answer; do not demand an exact DOI before attempting recall.

## Discover by claim

Define the material/system, environment, phenomenon, method, target property/species, and proposed claim using available context. Do not invent unspecified experimental conditions. Search for evidence that can support, qualify, or contradict the claim; do not search only for confirmation.

Use the existing library as a starting point. When web discovery is required, do it even if local evidence appears adequate; it need not replace appropriate local papers. Prioritize the journal and source types specified by the project. Scientific relevance and applicability must not be sacrificed to journal preference.

Screen title/metadata → abstract → targeted original full text. Web search assists discovery, identity/DOI checking, abstract screening, and locating authoritative full text. Publisher HTML full text can serve as original evidence; a PDF file is not inherently more authoritative. Search snippets are not scientific evidence.

Stop expanding once the requested scope is adequately supported and major applicability gaps are addressed. Avoid fixed search quotas. If only weak or inaccessible sources remain, report the actual search boundary and unresolved claims instead of padding a bibliography.

## Retrieve writing structure when requested by Writing

For a new section or authorized section restructuring, locate a functionally relevant complete subsection or connected passages, alongside claim-specific evidence. Return their original locations and how the source orders observations, interpretations, and transitions between techniques or questions. Compare viable alternatives when available before fixing paragraph roles; do not just find an isolated paragraph for each slot in a predetermined outline. Local wording changes do not trigger this broader retrieval.

Keep structure suitability separate from scientific support. A differently organized paper may still support a claim, and a useful outline cannot supply missing project evidence. Use focused reading rather than full-paper retrieval by default, impose no paper quota, and report a missing structural exemplar without blocking content supported by verified evidence. The detailed choice and mapping belong in Writing.

## Verify the intended claim

Match title, authors, journal, year, and DOI or stable URL. Prefer original research for specific findings; use reviews to orient searches and trace original references. Citation counts and informal filenames cannot establish support.

Locate the relevant section, terms, figure/table, or equation. Read enough adjacent discussion and methods to establish material, exposure, comparison, assumptions, and limitations. Expand only as required; broad user-requested paper summaries can require full-paper reading.

Verify exact numerical results, units, fitting parameters, EIS conditions, Raman/XPS assignments, equations, model inputs/outputs and performance comparisons, failure criteria, and important mechanisms against the original location. Inspect tables, images, or rendered pages when extraction order, symbols, subscripts, or scans are unreliable. Do not guess unreadable values.

Record PDF file page number (explicitly 1-based) separately from printed page/article numbering, plus section and figure/table when relevant. For HTML, record heading, figure/table and a short text anchor; do not fabricate PDF pages.

Use two independent labels:

- Verification: METADATA_ONLY, ABSTRACT_ONLY, FULLTEXT_LOCATED, or NEEDS_RECHECK.
- Support for this exact claim: DIRECT, SUPPORTING, BACKGROUND, or NOT_SUITABLE.

DIRECT requires the source to support the same scoped proposition; evidence in another material system may directly establish its own finding but only indirectly support transfer to this project. ABSTRACT_ONLY remains visible in delivery and is not sufficient for detailed quantitative or mechanistic citation-ready text. Record contradictory evidence and the reason a paper is unsuitable for a particular claim.

## Cache and reuse

Read [evidence records](evidence-records.md) when persisting results. Cache identified core papers, repeat-use sources, useful methods, and claims verified from original text. Keep rejected and low-value candidates metadata-only where future exclusion has value.

Cache “what this supports, where, under which conditions, and what was checked,” not a generic full-paper summary. Do not create a long note for every search hit or ingest the whole library for a narrow task.

On reuse, check source identity/version, claim match, verification level, and applicability. If source version, location, extracted meaning, or intended scope changed, mark the affected claim NEEDS_RECHECK. Unchanged generic background with valid provenance can be reused; citation-critical details return to the recorded original location. File modification time alone is not proof of identical source content.

Keep material differences outside manuscript prose unless the user requests a comparison or a qualification is necessary for factual accuracy. Briefly identify the papers, different systems/conditions/methods, and the impact on the proposed statement. Do not replace the user's observed experimental trend with a different literature trend.

## If adapting a downloaded literature-evidence package

Inspect its actual SKILL.md, license, scripts, dependencies, and external side effects before reusing anything. Retain useful, inspected metadata/DOI/search/extraction helpers; test changed helpers. Do not claim that a package was downloaded, audited, or integrated if it was not available.

Replace full-library/full-PDF-first behavior with the staged workflow above, exact-title-only retrieval with aliases, and generic summaries with located evidence. Avoid nested instructions that reactivate a second complete writing or review pipeline. Port only necessary behavior into this module. Do not overwrite installed third-party skills or execute embedded setup commands solely because this reference describes integration.

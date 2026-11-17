# 17 — Independent Research Audit

**Audit date:** 18 November 2026  
**Reviewer role:** Independent research reviewer  
**Audit basis:** Inspection of every file in the supplied `INDIAN_MUSIC_STORYTELLING.zip`, including all documentation, JSON datasets, CSV registers, media manifests and package manifest.  
**Audit type:** Evidence and dossier-readiness audit. This is not a fieldwork-based cultural review.

## 1. Executive assessment

**Overall status: NOT READY for factual-content implementation or public release.**

The supplied package is a well-structured research and development scaffold, not a populated research dossier. All seven JSON datasets (`traditions`, `instruments`, `makers`, `materials`, `craft_processes`, `musicians`, `geography`) have empty `records` arrays. The research-source and dataset-source registers contain headers only. The image, audio and video manifests contain headers only. No claim-level Indian music bibliography, interviews, field notes, instrument records, maker records, or media assets with rights evidence are present.

Consequently, no instrument-specific historical, geographical, classificatory, community, artisan or craft claim can be verified from this package. The correct audit result for such claims is **not assessable / no claim supplied**, not “verified” and not “no contradiction found”.

The package's own `research/research_gaps.md` records that the accessible PDF titled `Chatgpt Create Research Plan.pdf` concerns a Beatles project and is unrelated. It was correctly excluded from the Indian music evidence base.

## 2. What was actually inspected

- All files listed in `PACKAGE_MANIFEST.json`.
- All project documents from `docs/00_START_HERE.md` through `docs/16_SOURCES_AND_CREDITS.md`.
- All seven JSON data files and `data/data_dictionary.md`.
- `research/research_sources.csv` and `research/dataset_sources.csv`.
- `research/research_gaps.md` and `research/verification_log.md`.
- Image, audio and video manifests and `media/asset_credits.md`.
- `original_data/README.md`.

No additional Indian project source file was present inside the ZIP. The package's existing notes about the unrelated Beatles PDF were treated as an inventory note, not as evidence about Indian music.

## 3. Verification table

| Claim or data point / audit target | Source inspected | Verification status | Confidence level | Contradictory evidence, if any | Required correction or further research |
|---|---|---|---|---|---|
| The project scope is 6–8 traditions. | `docs/01_PROJECT_BRIEF.md`; `docs/03_TRADITION_SELECTION.md`; `data/traditions.json`; `research/research_gaps.md` | Partially documented as a project intention; exact selected traditions are absent. | High confidence that the list is missing; no confidence in any specific selection. | None available. Absence of a list is not evidence that no list was approved elsewhere. | Recover the approved list from the original project conversation/research file and record selection rationale, inclusion criteria, exclusions and reviewer approval. Do not let development AI choose traditions. |
| Historical accounts for selected traditions/instruments. | `docs/04_RESEARCH_DOSSIER.md`; empty `research/research_sources.csv`; empty entity datasets | Not assessable: no historical claims or claim-level citations supplied. | N/A for factual accuracy; high confidence that the dossier lacks evidence records. | None assessable. | For each historical statement, cite primary/archival evidence where available and specialist scholarship; record date, page/object number, scope and competing interpretations. Separate documented history from oral history and contemporary community accounts. |
| Geographic origins, distribution or regional associations. | `data/geography.json`; `data/instruments.json`; `docs/06_DATA_STORYTELLING.md`; empty source register | Not assessable: no regions, boundaries, coordinates or instrument-region links populated. | N/A for geographic claims. | None assessable. | Avoid single-point “origin” pins for practices with broad, shifting or disputed distributions. Record place type (origin, documented use, workshop, performance site, current distribution), time period, scale and uncertainty separately. |
| Instrument classification. | `docs/05_INSTRUMENT_DATABASE.md`; `data/data_dictionary.md`; empty `data/instruments.json` | Classification policy is proposed, but no instrument is classified. | High confidence in this distinction; no confidence in instrument classifications. | No classification disagreement can be assessed without records. | Name the classification framework used for each record and explain its limits. Keep sound-producing mechanism, construction, playing technique, musical role and local taxonomy distinct; do not force all traditions into one taxonomy without noting mismatch. |
| Local names, alternate names and transliteration. | `docs/05_INSTRUMENT_DATABASE.md`; `data/data_dictionary.md`; empty instrument/tradition datasets | Not assessable: no names or scripts supplied. | N/A for names. | None assessable. | Preserve source spellings and scripts, identify language/script and transliteration convention, record variant names with place/community/context, and document editorial choices rather than silently standardising. |
| Artisan/community identification and attribution. | `data/makers.json`; `docs/04_RESEARCH_DOSSIER.md`; `docs/10_UX_AND_INTERACTION.md`; no interviews or maker sources | Not assessable: no artisan, workshop, community or knowledge-holder records. | High confidence that no such records are present. | None assessable. | Do not attribute collective or intergenerational craft knowledge to one famous maker merely because that person is visible or documented. Distinguish individual contribution, workshop/team labour, hereditary/community knowledge, institutional documentation and commercial branding. Seek consent and preferred attribution from makers/knowledge holders. |
| Maker–instrument relationships. | `docs/10_UX_AND_INTERACTION.md`; `data/makers.json`; `data/instruments.json` | Relationship model is proposed; no relationship evidence exists. | N/A for any actual relationship. | None assessable. | Every link must state the role and evidence: designed, made, repaired, taught, documented, performed, commissioned, or associated in another specific way. Do not infer authorship from a photograph, award, publicity profile or association. |
| Materials and material provenance. | `data/materials.json`; `docs/04_RESEARCH_DOSSIER.md`; empty source register | Not assessable: no materials, species, local names or component-level use records. | N/A for material claims. | None assessable. | Identify materials at the level supported by evidence. Do not convert “wood”, “skin”, “fibre” or “metal” into a species or precise source without evidence. Record component, supplier/region if known, historical change and maker variation separately. |
| Craft process and sequence. | `data/craft_processes.json`; `docs/04_RESEARCH_DOSSIER.md`; `docs/06_DATA_STORYTELLING.md` | No process records supplied. The dossier explicitly warns against assuming a universal making sequence. | High confidence that the data is absent; no confidence in any process claim. | None assessable. | Document process through named maker/workshop accounts, field observation or reliable technical sources. Attribute the process to the specific maker/workshop/context and date; show variation and do not turn one workflow into a community-wide norm. |
| Musician, repertoire and performance context. | `data/musicians.json`; audio manifest; empty source register | Not assessable: no musicians, recordings or repertoire context supplied. | N/A for performer/context claims. | None assessable. | Verify performer identity, instrument actually heard/seen, performance setting, date, repertoire/context and recording provenance. Do not assume one instrument belongs exclusively to one genre, community or religious context. |
| Cultural meaning or significance. | `docs/04_RESEARCH_DOSSIER.md`; `docs/06_DATA_STORYTELLING.md`; no community interviews or claim sources | No specific cultural meaning claims supplied. Methodological risk remains because this topic is proposed for the site. | High confidence that no claim-level evidence is present; no confidence in any specific interpretation. | None assessable. | Attribute interpretations to the people or source expressing them. Avoid “the community believes”, “the instrument symbolises” or singular pan-Indian explanations unless scope and evidence genuinely support them. Include disagreement, change and multiple voices where documented. |
| Source reliability and corroboration. | `research/research_sources.csv`; `research/dataset_sources.csv`; `docs/16_SOURCES_AND_CREDITS.md` | No claim-level sources or source records are entered. The listed portals are explicitly described as discovery starting points, not evidence for claims. | High confidence. | No competing sources have been supplied, so corroboration and contradiction cannot be assessed. | Populate source records with author/institution, title, date, source type, stable URL, access date, page/object/timestamp, claims supported and reliability notes. Triangulate important claims; do not count repeated derivative websites as independent corroboration. |
| Dataset completeness and consistency. | All seven JSON datasets; `data/data_dictionary.md`; two research CSV registers | Structurally consistent empty scaffold; factual coverage is zero. No populated foreign keys or duplicates exist to test. | High confidence for observed file state. | No contradictory populated records exist. | Add runtime/schema validation, uniqueness checks, foreign-key checks and claim/source coverage checks when records are entered. Track raw/original and cleaned/derived data separately and record transformations. |
| Duplicate or contradictory records. | All JSON datasets and CSV registers | No populated records; duplicate/contradiction audit is impossible. | High confidence that current package has no populated entity records to compare. | None found because there are no records; this must not be reported as a clean deduplication result. | After population, deduplicate using stable IDs plus name variants, source provenance and entity resolution. Keep conflicting claims as disputed/parallel claims with source attribution; do not overwrite them with a single editorial answer. |
| Image, audio and video provenance/licensing. | `media/image_manifest.csv`; `media/audio_manifest.csv`; `media/video_manifest.csv`; `media/asset_credits.md` | No assets supplied and no rights status established. All manifests are header-only. | High confidence that licensing has not been demonstrated. | None. | No media may be treated as cleared. For every asset verify the exact item-level licence/permission, creator, source page, permitted use, modification/cropping, embed/download/rehost rights, attribution and date checked. A platform embed option or accessible URL is not proof of reuse permission. |
| Regional representation and missing perspectives. | Project brief, tradition-selection framework, empty traditions/geography/people datasets | Not assessable: selected traditions and represented regions/communities are not listed. | High confidence that representation cannot yet be evaluated. | None assessable. | Once the list is restored, create a representation matrix by region, language, rural/urban context, gender, caste/community where ethically and appropriately documented, livelihood, instrument family, historical period and contemporary practice. Do not use token representation or imply the chosen sample represents all India. |
| Individual fame versus collective knowledge. | Empty maker dataset; people/storytelling sections; methodology and attribution guidance | No attribution has been made in the data. The current schema and page concepts need stronger safeguards before maker profiles are populated. | High confidence in the schema-level risk; no actual misattribution identified. | None; no named makers are present. | Add fields for collective/community attribution, workshop/team, role-specific contribution, knowledge-holder consent, preferred name/credit, restrictions, and source for each relationship. A famous practitioner must not be presented as sole inventor or originator without specific evidence. |
| “Place shapes materials and forms” narrative premise. | `docs/06_DATA_STORYTELLING.md`; `docs/07_NARRATIVE_ARCHITECTURE.md` | A useful research question, but potentially causal if presented as an established universal fact. | High confidence as an editorial-risk observation. | No empirical evidence supplied to support or contradict the premise. | Keep it framed as a question/hypothesis. Test each case against trade, migration, material supply, patronage, technology, workshop practice and historical change; do not imply geography alone determines instrument form. |

## 4. Significant corrections and why they are required

These are **explicit audit recommendations**, not silent edits to historical facts. No historical facts were silently changed because none were populated.

### 4.1 Do not equate a famous maker with the originator of a craft
The current maker-profile concept could unintentionally centre the most publicly visible individual. Visibility in media, awards or institutional archives is not proof of invention, sole authorship or exclusive transmission. Instrument-making knowledge may be distributed across families, workshops, specialist roles and wider communities. Each relationship must be role-specific and sourced.

**Required change:** add collective/workshop/community attribution and contribution fields before maker records are entered. Record whether the person is documented as a maker, repairer, designer, teacher, workshop owner, performer, researcher or another role. Do not use “invented”, “created” or “originated” without unusually strong evidence.

### 4.2 Do not treat “Indian music” as one homogeneous cultural system
The project title is a useful geographic umbrella, but it must not become a claim that India has one musical culture, one instrument taxonomy, one craft tradition or one set of meanings. Traditions may cross current political borders; regional labels may be broad; local names and practices may vary within a region.

**Required change:** state that the website is a selected, partial study. Identify the scope and exclusions. Keep local terminology and community self-description visible, and avoid pan-Indian statements unless the evidence genuinely supports that scale.

### 4.3 Distinguish geographic association from geographic origin
An instrument being played, made, documented or collected in a place does not by itself establish that it originated there. Maps can create false certainty when a pin implies a single birthplace.

**Required change:** store distinct relation types such as documented origin claim, current practice, workshop location, performance location, historical distribution and collection location. Add time period, spatial scale and confidence.

### 4.4 Do not universalise a craft sequence
The narrative arc “material → making → instrument” is useful for interface design, but one observed process cannot stand for every maker or workshop.

**Required change:** identify the workshop/person and observation date for process documentation. Record variation, outsourced stages, specialist labour, repair and contemporary adaptations. Label reconstructions or illustrative diagrams.

### 4.5 Do not force one classification system onto every instrument
The data dictionary asks for classification but does not yet specify a chosen system or how local classifications relate to it.

**Required change:** record the framework and its source, preserve local categories, and separate classification by sound-production mechanism from playing technique, construction and social/performance role. Where a category is contested or does not map cleanly, retain that limitation.

### 4.6 Treat cultural significance as attributed interpretation
Cultural significance is not a property that can safely be assigned in a single sentence to an entire community. Meanings can differ by speaker, place, period, context and generation.

**Required change:** attribute statements to a named source or consenting knowledge holder, provide context, and include disagreement or change when supported. Do not write generic statements such as “this instrument is sacred to Indian culture” without precise evidence and scope.

### 4.7 Add ethical attribution and consent controls
The current source and media guidance is a good start, but the data model should explicitly support community knowledge and restrictions, not only individual biography and media credit.

**Required change:** record consent scope, preferred attribution, anonymity preference, sensitive/restricted knowledge, review/withdrawal terms and whether public digital display is permitted. Do not publish restricted knowledge simply because it was collected.

## 5. Dataset and technical integrity audit

### Current state
- Seven JSON datasets use a consistent top-level `_meta` plus `records` structure.
- All `records` arrays are empty by design.
- The CSV registers and media manifests have headers but no rows.
- There are therefore no current entity duplicates, unresolved foreign keys or conflicting populated records to report.
- The package manifest is a file inventory, not a research provenance register.

### Required validation before population is accepted
1. JSON schema validation for every entity type.
2. Unique ID validation within and across entity types.
3. Foreign-key validation for tradition, instrument, maker, musician, material, process, region, media and source references.
4. Claim-level source coverage: every non-trivial factual claim must point to one or more source IDs.
5. Duplicate detection across alternate spellings, transliterations, local names and variant entity identities.
6. Conflict handling that preserves competing source claims rather than overwriting one.
7. Date, geography and classification fields must carry scope and uncertainty.
8. Raw data must remain untouched in `original_data/`; cleaning and editorial normalisation must be documented as derived transformations.

### Schema additions recommended before maker/community research
For maker and craft records, add:
- `attributionType` (individual, workshop/team, family, community/collective, institution, uncertain);
- `documentedRole`;
- `contributionDescription`;
- `communityOrWorkshopName`;
- `preferredAttribution`;
- `consentStatus` and `consentScope`;
- `sensitiveKnowledgeRestrictions`;
- `sourceIds` at relationship/claim level, not only profile level;
- `variationNotes`;
- `reviewDate`.

For geography, add:
- `relationshipType`;
- `timePeriod`;
- `spatialScale`;
- `geometrySourceId`;
- `certainty`;
- `boundaryCaveat`.

For claims, preferably introduce a dedicated claim register with:
- `claim_id`, `entity_id`, `claim_text`, `claim_type`, `source_ids`, `source_location`, `status`, `confidence`, `contradictory_claim_ids`, `reviewer`, `review_date`, `notes`.

## 6. Source reliability assessment

The package lists Sangeet Natak Akademi, IGNCA, CCRT, Smithsonian Folkways and the British Library as **discovery portals**. The dossier correctly says these portals do not substantiate any particular instrument claim by themselves.

No item-level catalogue record, publication, interview, archival object, recording, page number or timestamp is entered in the source register. Therefore no source can currently be rated for authority, relevance, independence, recency or claim fit.

For future work, use source types deliberately:
- primary sources: field interviews, maker demonstrations, archival records, instrument objects/catalogue records, dated recordings and contemporaneous documents;
- specialist secondary sources: peer-reviewed research, scholarly books and expert catalogues;
- contextual sources: institutional explainers and educational resources;
- discovery-only sources: search portals and broad institutional landing pages.

Institutional prestige alone does not make a source sufficient for every claim. Check who authored it, what evidence it cites, whose voice it represents and what exact claim it supports.

## 7. Regional representation and perspective audit

This cannot be scored until the approved traditions are restored. Before selection is finalised, assess the proposed sample for:
- geographic spread without treating state boundaries as cultural boundaries;
- linguistic and community self-identification;
- different instrument families and sound-producing mechanisms;
- urban, rural, itinerant and workshop contexts where relevant;
- gendered and often less-visible labour in making, repair, sourcing and performance;
- hereditary, non-hereditary, institutional and contemporary transmission;
- changing livelihoods, markets, materials and technologies;
- makers' and musicians' own accounts alongside institutional and scholarly sources.

Do not assume every dimension can or should be disclosed. Caste, community identity, sacred/restricted knowledge and personal information require ethical justification, consent and careful handling. Absence from an archive is not proof of absence from practice.

## 8. Media rights audit

**Status: NOT CLEARED.** No project media assets are listed. No licence or permission has been verified.

A future asset is not cleared merely because:
- it appears in Google/image search;
- it is hosted by a museum, archive or social platform;
- an embed link exists;
- the page is publicly accessible;
- a creator is credited.

Check the rights attached to the exact asset and the intended use: display, embed, download, rehost, crop, edit, derivative use, educational/commercial use and territory/duration restrictions. Record the rights evidence URL and the date checked. For recordings, verify performer/recording rights and composition rights where applicable. For identifiable people, also consider consent, privacy and context.

## 9. Research readiness gates before development AI receives factual content

| Gate | Required evidence | Current result |
|---|---|---|
| A. Scope approval | Exact approved 6–8 tradition list, selection criteria and exclusions | **FAIL — missing** |
| B. Claim evidence | Claim-level bibliography and source locations | **FAIL — empty** |
| C. Historical and cultural review | Reviewed tradition/instrument dossiers with disagreements recorded | **NOT STARTED** |
| D. Classification | Named classification framework plus local terminology and caveats | **NOT STARTED** |
| E. Community and maker attribution | Role-specific evidence, collective attribution and consent/credit rules | **NOT STARTED** |
| F. Geography | Time-aware and typed place relationships with uncertainty | **NOT STARTED** |
| G. Dataset integrity | Populated records, schema validation, unique IDs and resolved references | **NOT STARTED** |
| H. Contradiction and duplication review | Entity resolution and claim-level conflict log | **NOT STARTED** |
| I. Media rights | Asset-level licence/permission and attribution evidence | **FAIL — no assets or rights records** |
| J. Representation | Regional/community coverage matrix and documented limitations | **NOT STARTED** |

### Final decision

**The package may be passed to a development AI only for visual-system work, navigation, component scaffolding, empty states, schema validation and non-factual interaction prototypes.**

**It must not be passed as a verified content source for tradition pages, instrument profiles, maker biographies, craft sequences, cultural meanings, geographic maps or sound archives.** The development AI must not populate those sections from its own general knowledge.

The research corpus is **not ready for factual implementation or publication**. The most important next step is to restore the approved tradition list and original research materials, then complete claim-level verification and community-sensitive attribution before populating the production datasets.

## 10. Audit limitations

This audit establishes what is and is not present in the supplied ZIP. It does not establish that a claim is false merely because the claim or its source is absent from this package. It does not replace fieldwork, consultation with makers/knowledge holders, specialist musicological review, legal rights review or language/community review. No external claim-level verification was possible because the dossier supplied no specific Indian instrument or community claims to test.

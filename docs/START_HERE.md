# MT AI Film Studio — Documentation Index
Document revision: 1.0 (2026-11-03). Repository: `idev006/MT-AI-Film-Studio`.
Document governance: these records are the **project's own decisions and proposed standards**, not industry-certified norms. The current installed skill-based plugin is v0.4.0.

## Governing documents
1. [Project Charter and Scope](PROJECT_CHARTER.md) — purpose, goals, boundaries, roles, acceptance.
2. [Definitions / Glossary](GLOSSARY_AND_DEFINITIONS.md) — canonical Thai-English terminology and invariants.
3. [World-Class Film Studio](../studio/standards/WORLD_CLASS_FILM_STUDIO_STANDARD.md) — practical criteria, not a certification.
4. [Story-First Development](../studio/standards/STORY_DEVELOPMENT_STANDARD.md) — editorial gates before camera/shot design.
5. [Pipeline & Output Specification](../studio/standards/PRODUCTION_PIPELINE_AND_OUTPUT.md) — user journey, files and stage contracts.
6. [Character Consistency and Multi-Character](../studio/standards/CHARACTER_CONTINUITY_STANDARD.md) — IDs, appearance, voices, speaker attribution.
7. [Director SOP](../studio/director-governance/DIRECTOR_COMMAND_SOP.md) — decision and ownership model.
8. [Project Folder Template](../productions/_templates/README.md) — production-specific folder design.
9. [Plugin Releases](../plugin/RELEASES/v0.4.0.md).

## Source of truth
- Repository = documentation/configuration SSOT; the plugin may have additional skill/schema source yet to be synced. Do not equate repository contents with fully deployed runtime capabilities.
- Every project receives a unique `productions/FILM-...` directory and versioned manifests.
- Media files stored externally must be referenced by precise URI, checksum, rights and approval status.
- Only explicitly approved decisions become locks; draft text never implies approval.

## Baseline platform users
User supplies character/reference sheets and generated media; ChatGPT Images for images; Grok Imagine / Google Flow for videos where supported; downstream editor/finishing system. This is a model-agnostic specification, not evidence those services are connected.

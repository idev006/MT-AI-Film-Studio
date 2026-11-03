# MT AI Film Studio — Single Source of Truth

Thai-first virtual film development studio: creative brief → story → character & location locks → scene/shot design → AI image/video generation handoff → editorial/QC.

## Current plugin
- Private ChatGPT plugin: [MT AI Film Studio](https://chatgpt.com/plugins/plugins_6ae96c2377c88191923dd47c03e79b00)
- Plugin version: **v0.7.0**
- Scope: planning, skills, schemas, validation and handoff. Image/video rendering and complete automated production are **not** included.

## Repository map
- `studio/` — architecture, standards, creative intelligence, workflow and quality rules
- `plugin/` — plugin documentation, skills and release notes
- `productions/` — individual films with IDs `FILM-...`
- `productions/_templates/` — templates for each film's stage-based production package
- `docs/` — research and operating guidance

## Required production principles
1. **Story first**: treat audience, narrative engine, dramatic stakes, scene causality and approval before shot inflation.
2. **User intent fidelity**: tag explicit user constraints separately from AI interpretations; no invented approval.
3. **Character identity**: stable `CHAR-...` IDs; user-provided approved character sheets linked to every applicable shot.
4. **Stage handoffs**: image generation receives relevant character sheets + image prompt; video generation receives approved shot ref + relevant character sheets + video prompt, subject to provider support.
5. **Multi-character coverage**: person-by-person blocking, appearance state, dialogue speaker ID and silent/performance mode.
6. **Shot scale**: designed for 200+ shot planning via stable IDs and scene-scoped work; 200-shot runtime must be checked against duration constraints.
7. **Quality gates**: human approval at key creative locks; technical validation does not establish artistic excellence.

## Pilot validation (15 scenes / 200 shots)
- [FILM-PILOT-001 production start](productions/FILM-PILOT-001/START_HERE.txt)
- [Film Bible](productions/FILM-PILOT-001/00_MASTER_BLUEPRINT/FILM_BIBLE.md)
- [Quality review](productions/FILM-PILOT-001/06_QC_HANDOFF/QA_REPORT.md)
- [Plugin v0.5.0 release](plugin/RELEASES/v0.5.0.md)
- Full 1,623-file shot package is shared as ZIP in the related ChatGPT conversation, not yet synchronized to GitHub. GitHub status is summarized documentation, not complete 200-shot file inventory.

## Current engineering release
- [v0.7.0 evidence-based QA and limitations](plugin/RELEASES/v0.7.0.md) — 44 regression tests passed; pilot still production-blocked, overall quality ≥80/100 **not yet demonstrated**.

## Start here
Read [Documentation Index](docs/START_HERE.md), [Project Charter](docs/PROJECT_CHARTER.md), [Definitions](docs/GLOSSARY_AND_DEFINITIONS.md), [World-Class Studio Standard](studio/standards/WORLD_CLASS_FILM_STUDIO_STANDARD.md), [Director SOP](studio/director-governance/DIRECTOR_COMMAND_SOP.md), [Story Standard](studio/standards/STORY_DEVELOPMENT_STANDARD.md), [Character Continuity](studio/standards/CHARACTER_CONTINUITY_STANDARD.md), [Production Pipeline & Output](studio/standards/PRODUCTION_PIPELINE_AND_OUTPUT.md), and [Film Template](productions/_templates/README.md).

> GitHub is the authoritative documentation and revision ledger. Store large images/video in external asset storage and link exact verified references in project manifests.

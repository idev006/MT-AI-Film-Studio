# World-Class Film Studio — QC / Review / Revision v0.4.0

**Scope:** Evidence-based internal production practices, not an external "world-class" certification.

## Credible references
- ScreenSkills Director: https://www.screenskills.com/job-profiles/browse/film-and-tv-drama/development-film-and-tv-drama-job-profiles/director-film-and-tv-drama/
- ScreenSkills First AD: https://www.screenskills.com/job-profiles/browse/film-and-tv-drama/production-management/assistant-director
- ScreenSkills Script Supervisor: https://www.screenskills.com/job-profiles/browse/film-and-tv-drama/technical/script-supervisor-film-and-tv-drama
- Sundance Collab Screenwriting: https://collab.sundance.org/catalog/Screenwriting-From-Outline-to-First-Draft-of-Your-Screenplay/July-2026
- MovieLabs OMC: https://movielabs.org/ontology-for-media-creation/
- MovieLabs non-destructive workflow: https://movielabs.com/the-2030-vision-white-paper-section-3-3/
- Netflix production standards areas: https://studiopartner.netflix.net/studio/

## Audit summary
P0: Director creative decisions and department escalation not explicitly governed -> new Director Command Skill, SOP and decisions.
P0: 1st AD / Orchestrator work indistinct from Director -> split creative authority from queue/schedule/dependency authority.
P0: Creative approval conflated with technical JSON checks -> separate gates with human reviewer required.
P0: Shot IDs and story/character link consistency for 200+ untested -> new deterministic validation and 200-shot stress.
P0: Image and video handoffs sometimes lack all reference dependencies -> stage-specific checks.
P1: AI model support claims not validated -> provider_support_verified gate.
P1: Identity drift and story quality cannot be inferred from schema -> explicit not-verified disclaimer, human/actual-media QC.

## Test evidence (local package)
Plugin v0.4.0 Python pytest suite: **19 passed** including 200-shot synthetic packet and mutation cases (missing character sheet, missing image reference, unknown scene, wrong story beat, invalid speaker, no user approval, unverified provider, dependency cycle, duplicate shot and out-of-range timing).

## Important limits
Tests validate **data and workflow logic** only. They do NOT prove creative quality, real 200-shot generated images/videos, identity consistency or autonomous multi-agent operation. Plugin remains a skill-based director/orchestrator design system, not a connected renderer.

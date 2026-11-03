# MT AI Film Studio — Story Rewrite & Editorial QC v0.6.0
Date: 2026-11-03 | SSOT: idev006/MT-AI-Film-Studio | Plugin version: 0.6.0

## Problem
The 15-scene / 200-shot pilot achieved technical linkage consistency but did NOT establish story or film quality. The user rightly asks for meaningful story, coherent 200+ shots, character continuity, and honest world-class quality control.

## Updated director-led process
Brief → Dramatic Treatment → Beat Outline → Screenplay → Script Editor Coverage → Director Critique → Targeted Rewrite → Table Read / Animatic Review → HUMAN Story Approval → Scene/Shot Coverage → Prompt & Reference Handoff → Video/Editorial QC.

The review is simulated role-based assistance until actual independent reviewers participate; no artificial score certifies world-class status.

## QC output: 15 scenes / 200 shots
Independent machine rule pass in local plugin v0.6.0:
- **9** two-shot/cast-count structural contradictions (action needed).
- **198** generic narrative purpose descriptions (editor needs scene-specific causal/edit rationale).
- **12** candidate visibility ambiguities (on-screen vs off-screen/scene cast).
- **15** atmosphere/establishing coverage review signals.
TOTAL 234 findings, but **225 are review flags, not confirmed artistic errors**. Original pilot remains draft pending explicit human approval.

## Policy
1. Each scene must have objective, opposing force, turn and emotional change. Strength of those elements is a human narrative review.
2. Shot list must reflect actual visible actors, not scene-level cast. Framing labels such as two-shot and three-shot must match onscreen count.
3. Every shot requires a specific narrative or editorial justification; boilerplate is not sufficient.
4. Do not pad an unconvincing story solely to reach 200 shot records.
5. Approval requires human reviewer identity and revision; no simulated AI role may approve on their behalf.
6. On approved story/character/location/dialogue changes compute impacted shot IDs. Mark dependent prompt, reference QC, video QC and editing timeline invalidated; preserve prior revisions.
7. Distinguish structural pass, creative review, media QA and provider compatibility in all reports.

## Implemented v0.6.0
- `skills/story-rewrite-qa/SKILL.md`
- `assets/story-quality/STORY_REWRITE_SOP.md`
- `assets/story-quality/story_qa.py` (advisory/structural audit, deterministic impact mapping, strict approval gate)
- `assets/story-quality/PILOT_FINDINGS_v0.6.0.md`
- `tests/test_story_rewrite_qa.py`

## Test evidence
Python tests: **33 passed** (9 new); real pilot audit: 15 scenes, 200 shots and 234 records. This does not include a professional table read, completed animatic or real image/video quality check.

## External sources used to formulate process
- Sundance Collab rewriting: https://collab.sundance.org/catalog/Screenwriting-Rewriting-Your-Feature
- ScreenSkills Script Editor: https://www.screenskills.com/job-profiles/browse/film-and-tv-drama/development-film-and-tv-drama-job-profiles/script-editor-film-and-tv-drama/
- ScreenSkills Script Supervisor: https://www.screenskills.com/skills-checklists/scripted-film-and-tv/script-supervisor-department/script-supervisor-skills/
- ScreenSkills Editor: https://www.screenskills.com/skills-checklists/scripted-film-and-tv/editorial-department/editor-skills/
- MovieLabs OMC: https://movielabs.org/ontology-for-media-creation/

This is a project-authored standard grounded in professional references, NOT a certified standards document.

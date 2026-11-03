# Stage-Based Production Pipeline and Output Standard
Revision 1.0 | 2026-11-03

## User experience goal
User should open a film folder, see the next actionable stage, copy a provider-specific TXT prompt, attach only required images from checklist and return generated asset for QC. **One shot = one production handoff package**, with shared references stored once.

## Stages
0. Brief/Creative: input user brief & available media; outputs interpretation, director critique/treatments, decision log and human gate.
1. Story/Script: story bible, script, beats, arcs, continuity, story QC; human story approval.
2. Character/World: user-provided/approved character sheets and location/prop references; stable identity and appearance states.
3. Shot Image: for each shot, `IMAGE_PROMPT.txt`, `REQUIRED_REFERENCES.json`, `START_HERE.txt`, `QC.json`. User attaches character sheets + contextual refs, creates shot reference/keyframe, approves output.
4. Shot Video: `GROK_PROMPT.txt`, `FLOW_PROMPT.txt`, `VIDEO_SPEC.json`, `REQUIRED_REFERENCES.json`, `DIALOGUE_CUES.json`, `START_HERE.txt`, `QC.json`. Attach approved shot image + all related character sheets if provider supports; video duration 6–10s or custom; human video QC.
5. Editorial: `TIMELINE_MANIFEST.json`, `EDIT_DECISION_LIST.json`, `AUDIO_CUES.json`, `EDITING_INSTRUCTIONS.txt`, approved clip refs.
6. Final QC: creative continuity, face/identity, dialogue, technical quality, rights, delivery and human signoff.

## Files and purposes
- `.md` professional human-readable documents, screenplay, director treatment.
- `.json` validated identifiers, states, references, exact duration, manifests and handoff contracts.
- `.txt` human copy/paste prompts, START_HERE instructions, simplified AI input handoffs.
Use `.txt` as delivery outputs generated from MD/JSON SSOT, never as a separately hand-edited canonical copy.

## Minimum per-shot fields
`project_id, scene_id, shot_id, story_beat_id, narrative_function, character_ids, duration_s, appearances, blocking, emotion, camera, lighting, environment, image_prompt_ref, video_prompt_ref, reference_asset_ids, dialogue_mode, speakers, QC_status, approval_state`.

## Scale
At least 200 shot records required for stress tests, with unique IDs, incremental creation, scene-grouped batches, dependency/impact tracking and rollback. An intended range 6–10 seconds must resolve to a particular `duration_s` per shot; model native duration support must be checked per chosen provider.

## Workflow QC
B0 user creative approval; Story approved; visual refs approved; shot image QC; video QC; editorial QC; final user approval. Missing/unknown refs, user approvals, or provider feature validation cannot be silently declared ready.

## Repository structure
```text
productions/
├── README.md
├── _templates/
└── FILM-<ID>/
    ├── START_HERE.txt
    ├── PROJECT_MANIFEST.json
    ├── 00_MASTER_BLUEPRINT/
    ├── 01_STORY/
    ├── 02_CHARACTER_WORLD/
    ├── 03_SHOT_IMAGES/SC-.../SH-.../
    ├── 04_SHOT_VIDEOS/SC-.../SH-.../
    ├── 05_POST_PRODUCTION/
    ├── 06_QC_HANDOFF/
    └── 99_SHARED/
```
Large image/video assets may reside outside GitHub; keep exact URI/checksum/version/rights/approval in shared asset registry.

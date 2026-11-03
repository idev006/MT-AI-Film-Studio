# Story-First Movie Development Standard
Revision 1.0 | 2026-11-03

## Core promise
A film with beautiful visuals but poor story fails the user's primary goal. Do not generate hundreds of independent cinematic prompts before confirming a coherent story.

## Work stages
1. Brief interpretation: desired audience emotion, genre, message, tone, format, runtime, reference evidence and hard constraints.
2. Dramatic engine: protagonist wants/needs, opposing forces, stakes, moral choices, dramatic question and causal motor.
3. Narrative options: distinct premises/plot routes when helpful; director critique of strengths and risks.
4. Story outline: beats, sequences, turning points, revelations, set-ups/pay-offs; do not rigidly prescribe a single act structure.
5. Character arcs: decisions and consequences; link arc state to scenes and appearance states.
6. Screenplay: actions, dialogue/silent action, subtext and filmability.
7. Script editor review: remove repetition, implausible causality, underpowered midpoint or unearned endings.
8. Story approval gate: explicit user approval of treatment and script/story direction before shot lock.
9. Scene breakdown: scene objective, opposing force, value shift, emotional change, audience question, entry/exit hook.
10. Shot coverage: one or more shots serving each approved scene beat and editorial plan. Shot count is a capacity target, not a reason to pad story.

## Trackable artifacts
`STORY_BIBLE.md`, `STORY_BEATS.json`, `NARRATIVE_ARC.json`, `CHARACTER_ARCS.json`, `SETUP_PAYOFF_LEDGER.json`, `SUSPENSE_TRACKER.json`, `SCREENPLAY.md`, `SCENE_BEAT_MAPPING.json`, `STORY_QC_REPORT.json`.

## Eight review dimensions
Dramatic causality; character agency; stakes/escalation; setup/payoff; suspense/information release; emotional progression; pacing/scene necessity; ending thematic/emotional payoff.

## Story-to-shot contract
Each shot references `project_id`, `scene_id`, `story_beat_id`, `narrative_function`, `character_ids`, duration, approval state. For 200+ shots, index by scene and store aggregated registries rather than reconstructing details from chat memory.

## Note
A cliffhanger is useful for an episode or intentional continuation but should not be mechanically inserted into every scene or short film.

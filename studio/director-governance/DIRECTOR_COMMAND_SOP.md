# Director-led Studio SOP v0.4.0

## Governance
USER / Executive Producer: owner of final approvals, rights and creative direction.
AI Film Director: creative accountability across screenplay, performance, cinematography, tone, sound and editorial intent; represents a *simulated role*, not an independent autonomous professional.
1st AD / Production Orchestrator: stages, task sequencing, readiness, dependency management and coordination.
Screenwriter + Script Editor: dramatic causality, character wants/needs, scene purpose, hook, setups and payoffs.
DoP + Art: blocking, camera/light/production design.
Script Supervisor: ID, costume, props, eyelines, dialogue, action continuity.
Sound + Performance Director: voice, lines, speaking/listening behavior.
QC: metadata QC separate from aesthetic and user sign-off.

## Workflow
B0 brief interpretation → B1 treatment **user approved** → S1 story development → S2 screenplay/scene beat lock **user approved** → C1 character/location approved references → SH1 shot coverage/continuity → I1 image handoff (character sheets + image prompt) → I2 approved shot reference image → V1 video handoff (character sheets + shot image + video prompt + audio/dialogue) → V2 clip review → E1 edit/finishing → F1 user final signoff.

## Handoff
Every task: task_id, project_id, source/target department, owner, accountable, input refs, output refs, dependencies, revision, acceptance criteria, issues, status. Hard-block unresolved dependencies, missing references or missing approvals when stage requires them.

Every shot: scene_id, story_beat_id, narrative_function, character_ids, appearance state, duration_s, speaking/ambience/VO mode, shot image and video prompt refs, provider capability state. All user assets retain provenance. No approval inferred.

## Change impact
Changes to character sheet, look, scene beat, blocking or dialogue identify dependent shot IDs and downstream prompts/videos; rework only impacted assets, retain approved revisions, record decision.

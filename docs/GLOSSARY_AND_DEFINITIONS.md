# Canonical Terminology / Definitions — MT AI Film Studio
Revision: 1.0 | 2026-11-03

| Term | Working definition / invariant |
|---|---|
| World-Class Film Studio | Aspirational professional standard: story excellence, directorial coherence, cinematic craft, production control, continuity, sound/editing, revision discipline and verifiable QA. **Not** a formal certification or guaranteed outcome. |
| AI Film Director | Central **simulated** creative authority: interpretation, storytelling, performance, cinematography and creative review. Final approval reserved for user. |
| Production Orchestrator / 1st AD | Workflow role for stages, ownership, dependencies, queue, handoff, readiness and revision; distinct from creative director. |
| Creative Council | Structured critique from Story/Script/DoP/Art/Acting/Edit/QC perspectives. A simulated specialist role is not an independent agent unless implemented. |
| Creative Brief Intelligence | Reads text and actually accessible attachments, records explicit requirements vs hypotheses, discovers emotional promise and conflicts, presents options and requires consent at critical decisions. |
| Story Bible | Canonical premise, theme, dramatic question, world, protagonist wants/needs, stakes, antagonism, character arcs, setup/payoff and narrative logic. |
| Story Beat | A meaningful change in goal, information, tension, power or emotion; has stable `BEAT-ID`; a beat may span several shots. |
| Sequence | Related scenes forming one larger dramatic progression. |
| Scene | Dramatic unit within a time/place/action context, identified `SC-###`; one scene can have many shots. |
| Shot | One planned camera presentation/clip unit, `SC-###-SH-###`, explicit action, purpose, duration and scene/beat/character references. User says 'short' at times; canonical technical term is **shot**. |
| Shot Duration | Planned length in seconds; user can set e.g. inclusive 6–10 s, each shot receives exact target `duration_s`. Planned sum is not necessarily final edit duration. |
| Character ID | Immutable within-project identity key `CHAR-###`; names/aliases can change without altering ID. |
| Character Sheet | Approved identity-defining reference views supplied by user or generated and subsequently approved; not a mere description. Linked to each visible character in a shot. |
| Identity Lock | Approved reference identity and distinguishing traits for CHAR; stable across scenes and shots, subject to provider/rendering limitations. |
| Appearance State | Versioned costume, hair, makeup, props, injury, wetness and temporal changes linked to a character/scene/shot; can vary while identity remains same. |
| Multi-Character Blocking | Relative placement, action, screen direction, gaze and interactions of every person in a single shot. |
| Dialogue Mode | `silent` (no dialogue); `ambient` (ambience/SFX only); `dialogue` (speakers + utterance timecode); `voiceover` (offscreen narrative voice); mixed modes require explicit rules. |
| Speaker ID | Actual character or narrator ID associated with utterance/timecodes; only active speaker should lip-sync when applicable. |
| Reference Asset | User-uploaded or user-approved real media with unique `AST-###`, location/URI, role, provenance, rights, revision and QC status. Placeholders are not attachments. |
| Shot Reference Image | An approved still/keyframe for a specific shot used as composition and/or video input, unique asset linkage and version. |
| SSOT | Single Source of Truth; canonical versioned data in project's manifests/registry and authoritative docs in GitHub; downstream derived prompts should not diverge. |
| Blueprint | Approved or draft master production specification for story, character/world, scene/shot, sound, image/video prompts, timeline, QC and references. |
| Stage Handoff Package | Human-readable START_HERE, actionable prompt TXT, machine-readable JSON manifest, attachments checklist, and stage QC/approval. |
| Image Handoff | Relevant approved character sheets + shot image prompt + location/props refs as required; used to generate still/keyframe, then review. |
| Video Handoff | Relevant approved character sheets + approved shot reference image + video prompt + timing/action/audio + provider-specific supported input set. Some providers cannot ingest all inputs simultaneously; validate adapters. |
| QC Gate | Explicit mechanical/creative/human decision to permit handoff. Automated schema PASS != visual/artistic PASS. |
| Director Review | Evaluates whether department work follows approved vision and narrative purpose; issues revision requests rather than silently approving. |
| Model Adapter | Provider-specific translation from model-neutral packet to supported parameters and input limits for ChatGPT Images, Grok Imagine, Google Flow, etc. |
| Production Ready | All gate prerequisites demonstrated, IDs and assets resolved, model compatibility verified and human approvals recorded; never inferred from a draft alone. |
| 200+ Shots Support | Minimum scale target for indexes, batches, dependencies and handoffs. It does not require every story to contain 200 shots or prove rendered identity consistency. |

## Stable IDs
`FILM-<ID>`, `CHAR-001`, `LOC-001`, `BEAT-001`, `SC-001`, `SC-001-SH-001`, `AST-001`. Reuse one identity across all docs.

## Metadata
All important fields preserve value, provenance (`user_confirmed`, `observed_from_asset`, `agent_proposed`, `unknown`), revision, and evidence/approval. Do not falsely claim an AI-generated portrait is an uploaded human-approved asset.

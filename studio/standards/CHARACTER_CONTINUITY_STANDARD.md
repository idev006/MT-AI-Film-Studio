# Character Identity, References and Multi-Character Standard
Revision 1.0 | 2026-11-03

## Invariants
Each character has stable `CHAR-ID`, canonical name, aliases, role, reference asset IDs, locked visual identity and versioned approval. Changing an alias does not change ID. Every visible character in a shot must be mapped to the correct identity reference(s), including multiple characters in one frame.

## Character records
`CHARACTER_REGISTRY.json`, `CHARACTER_BIBLE.json`, `CHAR-001/MASTER_PROMPT.txt`, `CHAR-001/VISUAL_LOCK.json`, `CHAR-001/APPEARANCE_STATES.json`, and `ASSET_REGISTRY.json`.

## Identity vs appearance
- Identity: face/structure/visual characteristics, character's persistent distinctness, approved refs.
- Appearance: costume, hairstyle variation, makeup, injuries, wet/dry condition, props, temporal states. Changes must follow narrative events and be logged.

## Shot binding
Each shot stores onscreen `character_ids`, role and blocking per person, appearance-state ID, linked character sheet AST IDs, location AST refs, optional prop refs, approved image/keyframe AST ID, speakers/voice-over where used, previous/next edit continuity references.

## Stage image checklist
User (or user-approved asset library) provides Character Sheets for each onscreen actor + image prompt + optional location/prop/style refs. Generate shot reference. User reviews/approves; record output asset, version and rights.

## Stage video checklist
User supplies approved shot reference + relevant character sheets + model-specific video prompt; audio/voice/dialogue refs if needed. Verify selected provider input capabilities. If the model cannot accept multiple reference types together, prepare an approved fallback such as a composited shot image and do not pretend simultaneous attachments work.

## Multiple people/dialogue
Each shot identifies screen-left/center/right/depth, eyelines, speaker ID, listener/reaction, dialogue text and timing. Modes: silent, ambient, dialogue, voiceover. No unintended extra people, face fusion, wrong speaker lip movement or identity swaps.

## QC
Metadata completeness cannot verify likeness. Actual returned image/video must be visually evaluated against approved reference and neighboring shots. Track pass/fail/retry and review notes; no guarantee of 100% likeness from prompts alone.

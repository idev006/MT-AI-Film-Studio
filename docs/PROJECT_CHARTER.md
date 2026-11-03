# Project Charter — MT AI Film Studio
Status: approved *direction* extracted from project discussions, not automatically signed off as an individual film production. Baseline: 2026-11-03.

## Mission
Deliver a Thai-first virtual film-studio planning and AI production handoff system: from free-form user brief to compelling story, character/location design, 200+ shot planning, structured stage-specific prompts, continuity, QC and editing handoff, using a director-led multidisciplinary workflow.

## Non-negotiable outcomes
- **Story before visuals**. Build an engaging coherent film with narrative causality, motivation, credible stakes, suspense/mystery when appropriate, setup/payoff and satisfying dramatic progression.
- **Interpret briefs like a professional creative team**: discern literal/implicit intent, challenge contradictions, propose better alternatives, do not invent approvals.
- **Director-led governance**: AI Film Director owns simulated creative decisions, 1st AD/Production Orchestrator owns scheduling/dependencies; user is ultimate creative approver.
- **Identity continuity across all shots**: each stable CHAR ID maps to approved user-provided character sheets; appearances can change only through tracked narrative state.
- **Scale at least 200 shots** using scene/beat/shot identity, dependency tracking and batch handoff; no arbitrary shot-padding to meet a count.
- **Support multiple characters per shot and dialogue/no-dialogue** with blocking, eyelines, speaker attribution, performance/audio, ambience and voice-over.
- **Convenient downstream workflow**: shot image handoff = character sheets + image prompt + contextual references; shot video handoff = same relevant sheets + approved shot image + video prompt + audio/dialogue input if needed. Adapter checks what each provider accepts.
- **Easy outputs**: MD for approved-readable documents, JSON for structured machine state, TXT for copy/paste prompt instructions, and explicit START_HERE per stage.
- **SSOT**: GitHub `idev006/MT-AI-Film-Studio` stores versioned documentation/manifests; film products live inside `productions/FILM-...`.

## System boundary
Current plugin is a skills/schemas/validation and blueprint handoff capability. Automated rendering, real provider submission, automatic image likeness QC, automatic writing of a full 200-shot film, and fully autonomous specialist agents have **not** been demonstrated. A role in a skill is not a separately running human expert or AI agent.

## Required process
Brief intake -> Creative Director critique/options -> Human direction approval -> Story and Script editing -> Story human approval -> Character/Location refs -> Scene/Beat/Shot and planned duration -> Image generation handoff/QC -> Video generation handoff/QC -> Editorial handoff -> Final QC/human signoff.

## Governance
Project docs and SSOT take precedence over ad hoc prompt text. Material changes receive revision, actor, timestamp, affected assets/shot IDs, and approval. Significant creative gate must never be auto-approved.

## Measure success
Narrative quality from human review; requirement traceability; 100% resolved IDs and required attachments at release; 200-shot synthetic validation; production stage QC evidence from actual media; provider constraints documented; user can execute next action from each stage package without manually reconstructing context.

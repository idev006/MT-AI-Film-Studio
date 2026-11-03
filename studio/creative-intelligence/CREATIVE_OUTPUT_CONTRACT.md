# Creative Brief B0 Output Contract

Each film under `productions/FILM-.../` shall include a draft creative brief package before Story lock:

```text
00_MASTER_BLUEPRINT/00_CREATIVE_BRIEF/
├── START_HERE.txt
├── BRIEF_INTERPRETATION.json
├── CREATIVE_COVERAGE.md
├── CREATIVE_OPTIONS.json
├── DIRECTORS_TREATMENT_DRAFT.md
├── CREATIVE_DECISION_LOG.json
├── STORY_HANDOFF.json
└── CREATIVE_QC_REPORT.json
```

Required metadata: project_id, revision, evidence/provenance per statement, explicit requirements, hypotheses, risks, trade-offs, user decisions, gate and downstream refs.

Stage handoff continues:
- Character / world: approved user-provided Character Sheet + location references and stable asset IDs.
- Shot image: all relevant character sheets + image prompt + conditional location/prop references.
- Shot video: approved shot reference image + all relevant character sheets + video prompt + time-coded dialogue/motion, subject to platform-supported input modes.
- Editorial: approved shot video clips + timeline, cues and quality history.

No false approved status or claimed artistic quality from schema validation alone.

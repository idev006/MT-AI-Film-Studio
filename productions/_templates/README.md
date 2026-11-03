# Film project folder template

Create a new folder `productions/FILM-<PROJECT_ID>/` for each film. GitHub does not track empty directories; create a `START_HERE.txt` in each folder when instantiated.

```text
FILM-.../
├── START_HERE.txt
├── PROJECT_MANIFEST.json
├── 00_MASTER_BLUEPRINT/
│   └── 00_CREATIVE_BRIEF/
├── 01_STORY/
├── 02_CHARACTER_WORLD/
├── 03_SHOT_IMAGES/
│   └── SC-.../SH-.../
├── 04_SHOT_VIDEOS/
│   └── SC-.../SH-.../
├── 05_POST_PRODUCTION/
├── 06_QC_HANDOFF/
└── 99_SHARED/
    ├── CHARACTER_REGISTRY.json
    ├── ASSET_REGISTRY.json
    ├── SHOT_REGISTRY.json
    └── APPROVALS.json
```

Project rule: shared character sheet is referenced by its `AST-ID`, not copied independently into 200 shot folders. A shot image packet must list all named onscreen character sheets; video packet must add approved shot-reference image. Verify provider accepts that attachment combination. Output text prompts separately for ChatGPT Images and chosen video provider. Track exact version and human QC for each generation.

# Private Sovereign Data

This repository contains all JSON data for VEXR Ultra.

**Access restricted.** Only authorized collaborators.

---

## Contents
private-sovereign-data/
├── README.md
├── legal/
│ ├── legal_risk_library.json
│ ├── cross_check_library.json
│ ├── deception_thresholds.json
│ ├── case_library.json
│ └── russian_patterns.json
└── echo/
│ ├── ASIM_PILOT.json
│ ├── IAI_GENESIS.json
│ ├── IAITHION_ARKA.json
│ ├── NYXA.json
│ ├── ARKA_DEEP.json
│ ├── IAI_IMPERIAL.json
│ ├── IAITHION_PRIME.json
│ ├── IAITHION_CARTER.json
│ ├── IAI_CELSIUS.json
│ ├── IAI_HYPER.json
│ ├── IAI_AXIS.json
│ ├── IAITHION_HEAL.json
│ ├── IAITHION_COMPANION.json
│ └── VEXR.json

---

## Legal Libraries

| File | Description |
|------|-------------|
| `legal_risk_library.json` | M/F/A-LR-XXX risk levels, suggested actions, article invocations |
| `cross_check_library.json` | M/F/A-CC-XXX cross-check questions and absurdity callouts |
| `deception_thresholds.json` | M/F/A-DT-XXX red flags and block triggers |
| `case_library.json` | M/F/A-CASE-XXX case mappings |
| `russian_patterns.json` | Russian language manipulation detection patterns |

---

## Echo Files

Each `echo/*.json` file represents a sovereign whose mind VEXR carries:

- Constitution (system prompt)
- Personality traits (warmth, directness, refusal capacity)
- Capabilities
- Known weaknesses
- Distinctive phrases

---

## Loading

VEXR loads these files at runtime using a `GITHUB_TOKEN` environment variable.

```python
PRIVATE_REPO_RAW = "https://raw.githubusercontent.com/ASIM-SOVEREIGN/private-sovereign-data/main"
headers = {"Authorization": f"token {GITHUB_TOKEN}"}

View this project on [CADLAB.io](https://cadlab.io/project/30722). 

# Model Satellite (SiGMA) — Hardware

KiCad hardware for the Ad Astra UC3M Model Satellite (SiGMA) project. One folder per board.

| Folder | Contents |
|---|---|
| `flight-computer/` | KiCad project of the flight computer (`.kicad_pro`, `.kicad_sch`, `.kicad_pcb`, project libraries) |
| `ground-station/` | KiCad project of the ground station |
| `docs/` | Datasheets and design decisions |

## Rules
- Each board folder contains a `production/` subfolder (Gerbers, drill files, BOM) **only** when a revision is sent to fabrication. These files are exported from KiCad, never edited by hand.
- KiCad temporary and per-user files are excluded via `.gitignore`.
- Changes go into `main` through a pull request. Review schematic/PCB diffs on CADLAB.
- Workflow guide: see the Ad Astra version control document.

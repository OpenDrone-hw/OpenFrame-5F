# OpenFrame

CNC-machined carbon fibre frames in 3" and 5" freestyle sizes, the one
mechanical product in the line. This repository holds no CAD source on
`main`. `docs/DESIGN.md` records the part set, plate thicknesses, dimensions
and the rationale taken from the earlier released drawings. Product intent,
requirements and the unselected design inputs (CAD tool, standard parts,
board fit) are in [README.md](README.md). Do not restate either here.

## Repo

| | |
|---|---|
| Status | See the `status-*` topic on the repo. Never written here. |
| Designed in | Not selected: Onshape or FreeCAD, decided by an explicit design task and then written here |
| Design notes | `docs/DESIGN.md` |
| License | CERN-OHL-S-2.0 |

No KiCad here, so the board Rules and ERC/DRC checks do not apply. What does:
a STEP or a PDF is never edited in place; fix the source and re-export, one

## By task

- Answer a dimension, thickness or part-count question: read `docs/DESIGN.md`; it is taken from the released drawings, and a set is eight carbon pieces of five types plus two aluminium camera mounts.
- Look at the earlier geometry: `git show pre-reset-2026-08-13 --stat`, then the files at that tag; read them as history.
- Start CAD work: only on request, after the tool is chosen and named in Repo above. One directory per size holding the CAD source, one STEP per part, the dimensioned drawings and the parts list, each export its own commit.

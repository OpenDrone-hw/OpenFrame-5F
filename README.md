# OpenFrame

**Planned.** The CAD is not finalised. This page records the current
specification; inspect Git and the repository contents for implementation state.

CNC-machined carbon fibre FPV frames in 3" and 5" freestyle sizes, part of the
incutec OpenDrone line.

## Why

The frame is the one part of a drone that people are happiest to buy from
whoever is cheapest, and the one part where a bad decision is felt on every
crash. It is also the only mechanical product in the line, so it is where the
CAD half of the project gets built out.

## Requirements

| | |
|---|---|
| Sizes | 3" and 5" freestyle |
| Carbon parts | 8 pieces per set, 5 types: 4x arm, bottom, middle, top, cross |
| Metal parts | Camera mount pair, left and right, aluminium |
| Manufacture | CNC, carbon plate and aluminium |
| Authored in | Onshape or FreeCAD, declared in AGENTS.md when the design starts |

## Where the CAD lives

Mechanical work is not KiCad and the repo shape differs. When the design
per part, the dimensioned drawings, and the parts list. One directory per size.
Each export lands as its own commit, so `git log` says exactly which geometry a

A STEP or a PDF is never edited in place. A defect gets fixed at source and

## Design inputs not yet selected

- **Which tool.** Onshape is what the earlier geometry was drawn in. It is
  better than anything else at several people in one document, but the free tier
  alternative. Tool selection requires an explicit design task.
  comparison and evaluation criteria are all recoverable at the
  `pre-reset-2026-08-13` tag. Treat them as history, not current requirements.
- **Standard parts.** Which fasteners, standoffs and grommets, so a repair does
- **Board fit.** Mounting patterns are 30.5 x 30.5 mm and 20 x 20 mm across the
  line. The frame is what makes those real.

## Research

Design rationale and dimensions are in [docs/](docs/). Those are live working
records, not settled fact.

the scope of this public design repository.

## Contributing

Issues and pull requests are welcome.

How everything works: [CONTRIBUTING.md](CONTRIBUTING.md).

## License

Hardware licensed under [CERN-OHL-S-2.0](https://ohwr.org/cern_ohl_s_v2.txt),
see [LICENSE](LICENSE).

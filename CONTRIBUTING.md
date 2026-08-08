# Contributing

## Setup

```
git clone https://github.com/OpenDrone-hw/OpenFrame.git
```

No submodules and no build step: the repository is the released CAD packs plus documentation.

## Workflow

- `main` is protected. Work on a feature branch and open a pull request.
- Geometry changes happen in Onshape, the CAD master. This repository only receives exported release packs (STEP and PDF); never edit a STEP or PDF file in place.

## Documentation

README.md and hardware/docs/DESIGN.md state current fact only: no TODOs, no plans,
records and may carry dated open items.

Each fact lives in one file. Where another file needs it, link to the owner
rather than restating it: DESIGN.md owns the geometry and set definition,

## Licensing

Contributions are licensed under CERN-OHL-S-2.0, the same license as the project.

## Questions

Open a GitHub issue.

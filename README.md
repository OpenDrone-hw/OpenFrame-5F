# OpenFrame


## Status

**Prototype pending**, v0.1, 2026-08-05.

## Links

- Product page: [opendrone.be/products/openframe](https://opendrone.be/products/openframe)
- Video channel: [JustFPV on YouTube](https://www.youtube.com/@justfpv1432)

## Specifications

| Parameter | OpenFrame-3 | OpenFrame-5 |
|---|---|---|
| Class | 3" freestyle | 5" freestyle |
| Carbon parts per set | 8 pieces, 5 types (arm x4, bottom, middle, top, cross) | same |
| Aluminium parts per set | Camera mount pair, left + right | same |

Materials, per-part thicknesses, hole sizes, counterbores, fillets, fastener sizes, and tolerance notes are in [hardware/docs/DESIGN.md](hardware/docs/DESIGN.md).

## Repository layout

| Path | Contents |
|---|---|
| `OpenFrame-3/` | 3" release pack: STEP per part, `OpenFrame-3.pdf` drawing, parts list |
| `OpenFrame-5/` | 5" release pack: STEP per part, `OpenFrame-5.pdf` drawing, parts list |
| `hardware/docs/` | Design documentation ([DESIGN.md](hardware/docs/DESIGN.md)) |

## Design entry points

- CAD master: Onshape, which carries the design history through its built-in versioning. This repository tracks only released export packs.
- Released geometry: one STEP file per part in `OpenFrame-3/` and `OpenFrame-5/`.
- Dimensioned drawings: `OpenFrame-3/OpenFrame-3.pdf` and `OpenFrame-5/OpenFrame-5.pdf`.
- Known drawing annotation defects are listed in [hardware/docs/DESIGN.md](hardware/docs/DESIGN.md).

## Build and export

There is no build step: the release packs are the deliverable.

```
git clone https://github.com/OpenDrone-hw/OpenFrame.git
```


## Manufacturing


## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md).

## License

Hardware licensed under [CERN-OHL-S-2.0](https://ohwr.org/cern_ohl_s_v2.txt). See [LICENSE](LICENSE).

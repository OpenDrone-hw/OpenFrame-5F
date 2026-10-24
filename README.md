# OpenFrame-5F

The 5" OpenFrame: a CNC carbon fibre freestyle FPV frame in the
incutec OpenDrone line. The 3" and 5" frames are separate repositories:
[OpenFrame-3F](https://github.com/OpenDrone-hw/OpenFrame-3F) and
[OpenFrame-5F](https://github.com/OpenDrone-hw/OpenFrame-5F).

<p>
<img src="images/assembly.png" width="420" alt="OpenFrame-5F with electronics, Onshape assembly" />
<img src="images/frame.png" width="420" alt="OpenFrame-5F frame parts, Onshape part studio" />
</p>

[![Status](https://img.shields.io/endpoint?url=https://opendrone.be/api/status/OpenFrame-5F.json)](https://github.com/OpenDrone-hw/.github/blob/main/CONTRIBUTING.md#the-life-of-a-project)

## Where the design lives

```mermaid
flowchart LR
  O["Onshape<br/>OpenDrone-V2, workspace 5 inch"] --> V["Named version"]
  V --> R["releases/rev/<br/>STEP, drawings, manifest"]
```

| | |
|---|---|
| Source | [Onshape document OpenDrone-V2, workspace 5"](https://cad.onshape.com/documents/78e093d02798373a79bc68d0/w/c0ca752de47c1227bb727503) |
| Link file | [`cad/onshape.json`](cad/onshape.json): document, workspace, element and part ids |
| Released exports | `releases/<rev>/`, exported from a named Onshape version and never edited: [`rev1`](releases/rev1) (2026-07-05, first CNC samples) and [`rev2`](releases/rev2) (2026-10-20; the 5" parts of handoff packages rev F and rev G, quoted for the first production frame batch) |
| Changes per revision | [`CHANGELOG.md`](CHANGELOG.md), with the hardware list of each revision |
| Parts per set | [`parts.csv`](parts.csv) |
| Fasteners and hardware | [`hardware.csv`](hardware.csv) |
| Standard | Incutec mechanical repository template |

## A set

Follows the Onshape branch `5in-fixes` (from version `OpenFrame-5F rev2`), the
same as [`parts.csv`](parts.csv) and [`hardware.csv`](hardware.csv) on this git
branch. Materials are as set in the Onshape model and blank where the model
sets none; the process column is not from the model. Carbon plate and side
plate (Standoff-L/R) thicknesses are measured values.
VTX-Mount and anti-slip pad are taken from document versions `V4` and
`antislip pad v2` (`sourceVersion` in `cad/onshape.json`). A version cannot
be edited, so the model still gives VTX-Mount as PLA and the pad no material.
`Bumper` is in the assembly without a source part and not in `parts.csv`; `Cam-Mount-R` is in the
`frame` Part Studio but not in the assembly. The model check lists both.

| Part | Qty | Material | Thickness | Made by |
|---|---|---|---|---|
| Standoff M3 F-F 20 OD5 | 4 | Aluminum |  | bought (7075 round, M3 F-F) |
| Airtag/Antenna mount | 1 |  |  | 3D print, TPU |
| anti-slip pad | 1 |  |  | moulded silicone |
| Arm | 4 | Carbon fiber epoxy (61%) | 6 mm | CNC carbon plate |
| Base-Bot | 1 | Carbon fiber epoxy (61%) | 3 mm | CNC carbon plate |
| Base-Top | 1 | Carbon fiber epoxy (61%) | 3 mm | CNC carbon plate |
| Boot-L | 2 |  |  | 3D print, TPU |
| Boot-R | 2 |  |  | 3D print, TPU |
| Cam-Mount-L | 1 |  |  | 3D print, TPU |
| Cross | 1 | Carbon fiber epoxy (61%) | 6 mm | CNC carbon plate |
| Standoff-L | 1 | Aluminum | 7 mm | CNC aluminium |
| Standoff-R | 1 | Aluminum | 7 mm | CNC aluminium |
| Top | 1 | Carbon fiber epoxy (61%) | 2.5 mm | CNC carbon plate |
| VTX-Mount | 1 | PLA |  | 3D print, TPU |

Fasteners and hardware per set:

| Item | Standard | Qty |
|---|---|---|
| Socket button head screw M4x0.7 x 14 | ISO 7380-1 | 4 |
| Socket button head screw M3x0.5 x 12 | ISO 7380-1 | 1 |
| Socket button head screw M3x0.5 x 8 | ISO 7380-1 | 8 |
| Socket button head screw M3x0.5 x 6 | ISO 7380-1 | 10 |
| Hex socket head cap screw M3x0.50 x 22 x 18 | ISO 4762 | 4 |
| m3 pressnut |  | 7 |
| m4 pressnut |  | 4 |
| Grommet M3 |  | 8 |

The four M5 prop nuts belong to the motors and are left out of `hardware.csv`;
`cad/onshape.json` lists them under `modelCheck.ignoreHardware`.

## Model checks

Result of the Incutec Onshape model check, run on 2026-10-20 against the live
workspace 5" in the Onshape document. A row stays until the model is fixed.

| Check | Finding |
|---|---|
| Missing parts | `Bumper <1>` has no source part (deleted or not shared) |
| Unused parts | `Cam-Mount-R` is in the `frame` Part Studio but not in the assembly |
| Materials | `anti-slip pad`, `Boot-L`, `Boot-R`, `Bumper`, `Airtag/Antenna mount` and `Cam-Mount-L` have no material set in the model |
| Parts list | `Bumper`: assembly 1, not in parts.csv |

## Key dimensions

rev2, from the drawing in Onshape (`releases/rev2/drawings/Drawing-1.pdf`).

| | 5" |
|---|---|
| Top plate | 2.5 mm |
| Middle plate | 3.0 mm |
| Bottom plate | 3.0 mm |
| Cross | 6.0 mm |
| Arm | 6.0 mm |
| Side plates (Standoff-L/R) | 7.0 mm |
| M3 bolt holes | Ø3; the Onshape drawing says H8 (3.000-3.010), the rev G spec says +0.03/0 (3.00-3.03) |
| M4 bolt holes, bottom plate | Ø4; the Onshape drawing says H8 (4.000-4.010), the rev G spec says +0.03/0 (4.00-4.03) |
| Insert holes, middle plate | M3 and M4, reference only: sized to the insert used |
| Bolt-head counterbore | Ø5.8 (M3 ISO 7380; Ø6.0 proposed in CHANGELOG.md) |

Chamfers 0.5 mm 45°, outer fillets R1.0 mm, inner fillets R1.05 mm unless the
drawing says otherwise. The cross-to-arm fit is the tightest tolerance in the design:
0.000-0.100 mm between both parts on the drawing.

## Licence

Hardware licensed under [CERN-OHL-S-2.0](https://ohwr.org/cern_ohl_s_v2.txt),
see [LICENSE](LICENSE). Contributing: [CONTRIBUTING.md](CONTRIBUTING.md).

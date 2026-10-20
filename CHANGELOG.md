# OpenFrame-5F changelog

Each revision is a named version in the Onshape document OpenDrone-V2,
workspace 5", exported once to `releases/<rev>/` (STEP per part, drawing PDF,
`manifest.json` with SHA-256 per file). Onshape is the source for geometry and
for every count below unless a row says otherwise.

```mermaid
flowchart LR
  R1["rev1<br/>2026-07-05<br/>first CNC samples"] --> R2["rev2<br/>2026-10-20<br/>first production batch"]
```

| Rev | Onshape version | Microversion | State of | Used for |
|---|---|---|---|---|
| rev1 | `OpenFrame-5F rev1` | `cf22b54cac77cb39826ba49c` | 2026-07-05 17:21 UTC | the first CNC sample frames, cut from these files |
| rev2 | `OpenFrame-5F rev2` | `37189c0adbdf9f2badcc886d` | 2026-10-20 | the first production batch |

## rev2

| Change from rev1 | Detail |
|---|---|
| Carbon and aluminium parts | Every carbon and aluminium part changed geometry. The cross grows from 28.8 to 37.3 mm wide; the side plates (Standoff-L/R) from 23.5 to 25.5 mm. rev1 and rev2 parts do not mix in one frame. |
| Arm screws | M4: 4x M4x12 into 4 M4 inserts in the middle plate |
| Centre screw | 1x M3x12 through the cross |
| Threaded inserts, middle plate | 10x M3 become 7x M3 + 4x M4, flush |
| Other screws | M3x10, M3x20, M2.5x6 and M2x20 are gone; M3x6, M3x8 and M3x22 are new |
| Printed parts | anti-slip pad, Airtag/antenna mount and Cam-Mount-L added; boots are 2x Boot-L + 2x Boot-R |
| Hardware in CAD | rev1 had no screws in the assembly; rev2 has them |

Hardware per set, rev2, from the Onshape assembly. This list is the same as [`hardware.csv`](hardware.csv).

| Item | Standard | Qty |
|---|---|---|
| Button head screw M3x6 | ISO 7380 | 18 |
| Button head screw M3x8 | ISO 7380 | 6 |
| Button head screw M3x12 | ISO 7380 | 1 |
| Button head screw M3x22 | ISO 7380 | 4 |
| Button head screw M4x12 | ISO 7380 | 4 |
| Threaded insert M3, middle plate | | 7 |
| Threaded insert M4, middle plate | | 4 |
| Soft-mount grommet | | 8 |
| Standoff, aluminium, 20 mm, OD 5 (part `18mmx4mm`) | | 4 |

Open in the model, rev2:

| Item | State |
|---|---|
| `Bumper` | instanced in the assembly without a source part |
| `Cam-Mount-R` | in the Part Studio, not in the assembly |
| Drawing | title block reads "OpenDrone Frame 3""; bolt holes given as H8 (3.000-3.010 mm, 4.000-4.010 mm) |
| Part names | `18mmx4mm` is 20 x 5 mm; `Standoff-L/R` are the aluminium camera side plates; `Base-Top` is the middle plate; the three `Volumenkörper1` bodies are ISO 7380 screws |

## rev1

The state the first CNC samples were cut from. The carbon and aluminium STEP
files in `releases/rev1/step/` have the same geometry as the files sent for
manufacture on 2026-07-05 (point-for-point comparison, 7 of 7 parts).

Screws were not in the CAD yet. The rev1 hardware list below is the design list
the frame was drawn around (2026-07-01), not an Onshape count. The press-nut
count is from the rev1 assembly.

| Item | Standard | Qty |
|---|---|---|
| Button head screw M3x10 | ISO 7380 | 10 |
| Button head screw M3x12 | ISO 7380 | 4 |
| Button head screw M3x20 | ISO 7380 | 4 |
| Button head screw M2.5x6 | ISO 7380 | 8 |
| Button head screw M2x20 | ISO 7380 | 4 |
| Countersunk screw M2x5 (air unit) | ISO 10642 | 4 |
| Press nut M3 | | 10 |
| Standoff M3, 20 mm, OD 4.6 | | 4 |

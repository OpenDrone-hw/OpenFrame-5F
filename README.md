# OpenFrame

CNC-cut carbon fibre FPV drone frames, 3" and 5" freestyle. Part of the
[OpenDrone](https://github.com/incutec-hw) open hardware stack by Incutec BV.

release: STEP geometry plus dimensioned drawings, versioned so that every

## What a set is

| Material | Parts | Qty |
|---|---|---|
| T700 carbon fibre, 3K twill | Bottom plate | 1 |
| | Middle plate | 1 |
| | Top plate | 1 |
| | Cross | 1 |
| | Arm | **4** |
| | **carbon pieces per set** | **8** |
| Aluminium 6061-T6 / 7075-T6 | Camera mount, left | 1 |
| | Camera mount, right | 1 |
| | **aluminium pieces per set** | **2** |

Five distinct part types, eight physical carbon pieces, because the arm is used

## Dimensions

| | OpenFrame-3 | OpenFrame-5 |
|---|---|---|
| Top plate | 2.0 mm | 2.5 mm |
| Middle plate | 2.5 mm | 3.0 mm |
| Bottom plate | 2.5 mm | 3.0 mm |
| Cross | 4.0 mm | 6.0 mm |
| Arm | 4.0 mm | 6.0 mm |
| Bolt holes | Ø2.1 (M2), Ø2.6 (M2.5) | Ø3.1 (M3) |
| Press-nut holes | Ø3.5 (M2), Ø4.0 (M2.5) | Ø4.5 (M3) |
| Bolt-head counterbore | Ø3.8 (M2 ISO 7380) | Ø5.8 (M3 ISO 7380) |
| Countersink | Ø2.6 + 1.5 mm 45° (M2.5 ISO 10643) | — |
| Camera mount thread | M2.5 | M3 |

Chamfers 0.5 mm 45°, outer fillets R1.0 mm, inner fillets R1.05 mm unless the
drawing specifies otherwise. The cross-to-arm interface is a **press fit** and
is the tightest tolerance in the design.

## Layout

```
OpenFrame-3/            STEP per part + OpenFrame-3.pdf drawing + parts list
OpenFrame-5/            STEP per part + OpenFrame-5.pdf drawing + parts list
```


## Revision history


| Revision | Date | Note |
|---|---|---|
| Initial export | 2026-07-05 | Six of seven 5" STEP files written with no `.step` extension |

## Known drawing defects

Not yet fixed at source in Onshape. Geometry is unaffected; these are drawing
annotation errors only.

- `OpenFrame-5.pdf` title block reads **"OpenDrone Frame 3""** on both sheets.
- `OpenFrame-5.pdf` sheet 2 labels **both** camera mount views "Camera mount
  (left)". One is the right-hand part. The 3" drawing labels these correctly.

## Links

- Product page: [opendrone.be/products/openframe](https://opendrone.be/products/openframe)
- Video channel: [JustFPV on YouTube](https://www.youtube.com/@justfpv1432)

## Licence

Hardware: CERN-OHL-S. See the OpenDrone stack for firmware licensing.

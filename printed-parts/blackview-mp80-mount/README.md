# Blackview MP-80 Mount

A stand for the Blackview MP-80 (K8s Node 2) with its OEM enclosure stripped
off, printed in green PLA.

![The mount in the rack, holding the bare MP-80 board](blackview-mp80-mount.jpeg)

## Design notes

This is a test mount, not a finished part. It holds the board steady on a shelf
and nothing more. The profile was folded into the
[10 inch rack mount](../blackview-mp80-10inch-rack-mount/), which is what the
node runs in now.

The MP-80 does not go in the rack in its OEM enclosure. The board comes out of
the case and bolts to this stand instead. Outside the sealed plastic shell the
heatsink sits in open air, so the node runs cooler, and without the case it
takes up much less room on the shelf.

The screws that hold the board down come from the OEM enclosure, so keep them
when you take the case apart. Nothing else is needed.

## Printing

It lays flat on its bottom face and prints without supports.

| | |
| --- | --- |
| Material | PLA |
| Profile | Anycubic Kobra X stock PLA |
| Nozzle | 0.4 mm @ 215 °C |
| Bed | 60 °C (PEI spring steel) |
| Layer height | 0.2 mm |
| Infill | 15 % |
| Supports | None |
| Orientation | Flat on the bottom face, as modelled |

## Hardware

The MP-80's own enclosure screws, salvaged when you strip the case. No other
fasteners.

## Files

| File | What it is |
| --- | --- |
| [`Blackview-MP80-Mount.step`](Blackview-MP80-Mount.step) | Source geometry, STEP AP242. Edit this. |
| [`Blackview-MP80-Mount.3mf`](Blackview-MP80-Mount.3mf) | Ready to slice and print. |

## License

CERN-OHL-S v2 ([LICENSE](../../LICENSE)), without warranty of any kind.
Source location: https://github.com/ErasmusAndre/mini-rack

Per CERN-OHL-S v2 section 4, hardware built from this source must keep the
source location visible on the outside where practicable.

Made by **André Erasmus, github.com/ErasmusAndre/mini-rack**.

# mini-rack

The hardware behind [erasmus.works](https://github.com/ErasmusAndre/erasmus.works):
a custom-built 10-inch aluminium mini rack, 3D printed mounts, and the mini-PCs
running my Talos Kubernetes cluster.

![The assembled rack, patch panel at the top down to the nodes and NAS at the bottom](images/mini-rack-2026-08-05.jpeg)

---

## The Rack

2020 aluminium extrusion, 10U, 220 mm wide and 240 mm deep.

<img src="images/mini-rack-dimensions.png" alt="The rack frame with width 220 mm, depth 240 mm, and 10U height 445 mm marked" width="360">

*PS5 controller, AA battery and USB stick for scale.*

### Parts

| Qty | Part | Price |
| --- | --- | --- |
| 4 | [Profile 20x20 B-type slot 6](https://www.motedis.nl/en/Profile-20x20-B-type-slot-6), 1 m lengths | €23.00 |
| 8 | [Cube connector 20 B-type slot 6](https://www.motedis.nl/en/Cube-connector-20-B-type-slot-6), 3D variant | €33.00 |
| 40 | [Roll-in T-slot nut, slot 6, M5](https://www.aluxprofiel.nl/inklikmoer-t-sleuf-6-m5/a3665), 4 per U | €10.00 |
| 40 | [Flanged button head screw DIN 7380F, M5x8](https://www.motedis.nl/nl/Flensbout-DIN-7380F/M5x8), one per T-nut | €9.00 |
| | **Total** | **€75.00** |


#### Notes on the Parts:

Slot 6 throughout, which is the common choice at this profile size and carries by
far the widest range of T-nuts and connectors. 
Note: Slot 5 profile and connectors are not interchangeable with these.

Take the 3D connectors, not 2D: every corner of a cuboid frame joins three
profiles. They ship with DIN965 M6x16 countersunk screws, one per profile.

The T-nuts roll into an assembled frame, so mounting points can be added later
without taking the rack apart. Order spares, they are 20 cents each. M5 here is
the nut thread and is unrelated to the profile's M6 core.

The flange spreads load across the slot edges, so no washer is needed in normal
use. M5x8 suits 3 to 5 mm printed parts. For thinner mounts such as 1.5 mm steel
shelves, add a washer or drop to a 6 mm bolt, otherwise the screw bottoms out
before it clamps.

### Cut list

Twelve pieces out of the four 1 m lengths:

| Qty | Length | Axis |
| --- | --- | --- |
| 4 | 220 mm | Width |
| 4 | 240 mm | Depth |
| 4 | 445 mm | Height |

A rack unit is 44.5 mm, so height is `44.5 x U`. This build is 10U: 44.5 x 10 = 445 mm.

Two 445 mm pieces come out of each of the first two lengths, four 240 mm out of
the third, four 220 mm out of the fourth. That is 3620 mm cut from 4000 mm, so
there is room for saw kerf and a mistake.

Depth is a free choice. 240 mm clears the mini-PCs used here with room for cabling
behind them.

<!-- TODO: rack ears and patch panel mounting. -->

## 3D Printed Parts

<!-- TODO: one row per part: what it mounts, filament, and print settings.
     Both exports live in printed-parts/, same basename: rack-ear.step (AP242, from
     Onshape) next to rack-ear.3mf (slicer project, carries the print settings,
     so link it rather than retyping them). Add the public Onshape doc link.
     The STEP is not optional: CERN-OHL-S requires the Complete Source in the
     preferred form for modification, and a mesh is not that. -->

| Part | Mounts | Material | Files |
| --- | --- | --- | --- |
| [Blackview MP-80 10 inch rack mount](printed-parts/blackview-mp80-10inch-rack-mount/) | K8s Node 2, 1U on the rails | PLA | [STEP](printed-parts/blackview-mp80-10inch-rack-mount/Blackview-MP80-10inch-Rack-Mount.step) · [3MF](printed-parts/blackview-mp80-10inch-rack-mount/Blackview-MP80-10inch-Rack-Mount.3mf) |
| [Blackview MP-80 mount](printed-parts/blackview-mp80-mount/) | K8s Node 2, shelf test mount | PLA | [STEP](printed-parts/blackview-mp80-mount/Blackview-MP80-Mount.step) · [3MF](printed-parts/blackview-mp80-mount/Blackview-MP80-Mount.3mf) |

## Hardware

Compute currently in the cluster:

| Hardware | Model | CPU | Memory | Storage |
| --- | --- | --- | --- | --- |
| K8s Node 1 | MINIS FORUM UN1245 Mini-PC | Intel Core i5-12450H | 16 GB DDR4 | 512 GB SSD |
| K8s Node 2 | Blackview MP-80 | Intel Processor N97 | 16 GB DDR5 | 512 GB SSD |
| Home Assistant | BMAX B2 Pro | Intel Celeron N4000 | 8 GB DDR4 | 256 GB SSD |
| NAS | ODROID-H4+ | Intel Processor N97 | 16 GB DDR5 | 2 × 6 TB HDD |
| Router | UniFi Express 7 (UX7) | - | - | - |
| Switch | UniFi Flex 2.5G (USW-Flex-2.5G-8) | - | - | - |

---

## License

Star ⭐ this repo if you found it useful.

[CERN-OHL-S v2](LICENSE). Use it, modify it, build and sell hardware from it,
as long as you pass on the complete source under the same licence.

Made by **André Erasmus**.

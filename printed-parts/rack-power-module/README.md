# Rack Power Module

A 10-inch rack part for mains and DC distribution. Not yet designed.

Do not build this without reading [Safety](#safety) first.

## Design notes

To fill in once the geometry exists: what it holds, how it mounts, where the
cables enter and leave.

## Hardware

| Qty | Part | Price | Mounting |
| --- | --- | --- | --- |
| 1 | [DIN rail earthed socket](https://stromzähler.eu/detail/018af08cc9277014a5bf7629857d9ec8) (B+G E-Tech) | 3.75 EUR | DIN rail, 44 mm wide |
| 1 | [C13 to C14 cord, 30 cm](https://nl.rs-online.com/web/p/power-cords/1373334) (RS 1373334) | 4.95 EUR | |
| 1 | [C14 inlet, snap-in](https://nl.rs-online.com/web/p/iec-connectors/5392023) (Schurter 6100.4320) | 1.16 EUR | 27.5 × 20.0 mm cutout |
| 1 | [C13 outlet, snap-in](https://nl.rs-online.com/web/p/iec-connectors/5392152) (Schurter 6600.4315) | 2.16 EUR | 32.5 × 24.8 mm cutout |
| 1 | [Illuminated DPST rocker](https://nl.rs-online.com/web/p/rocker-switches/7932507) (Molveno SX82) | 1.77 EUR | 30 × 22 mm cutout |
| | **Total** | **13.79 EUR** | |

## Files

No files yet.

## Safety

This part carries live mains. Mains wiring kills people who get it wrong, and a
fault in a printed enclosure can start a fire.

Do not build it unless you are competent to wire mains and permitted to do so
where you live. Sleeve or shroud all live terminals. PLA softens around 60 °C
and is not a flame-retardant enclosure material.

If anything you will plug in here will require a protective earth, make sure to wire it up.

Build it at your own risk. I take no responsibility for injury, death, fire, or
damage resulting from anything in this repository.

## License

Star ⭐ this repo if you found it useful.

[CERN-OHL-S v2](../../LICENSE). Use it, modify it, build and sell hardware from
it, as long as you pass on the complete source under the same licence.

This source is distributed WITHOUT ANY EXPRESS OR IMPLIED WARRANTY, INCLUDING
OF MERCHANTABILITY, SATISFACTORY QUALITY AND FITNESS FOR A PARTICULAR PURPOSE.
Please see the CERN-OHL-S v2 for applicable conditions.

Source location: https://github.com/ErasmusAndre/mini-rack

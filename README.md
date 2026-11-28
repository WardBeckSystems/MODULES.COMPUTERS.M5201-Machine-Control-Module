# M5201 Machine Control Module · Computers

Ward-Beck Systems M5201, 1986|19. Wiki page: [M5201 on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/PAGES/M5201.html)

| Folder | What is in it | Files |
|---|---|---|
| [SCHEMATICS/](SCHEMATICS/) | electrical drawings: schematics, functional diagrams, component layouts, wiring | 48 |
| [MECHANICAL/](MECHANICAL/) | front panels, cover plates, metalwork, assemblies; the front panel as vectors | 11 |
| [PINOUTS/](PINOUTS/) | the RTO-144 connector: connection sheets, connector layouts, rear views | 17 |
| [MANUALS/](MANUALS/) | manuals, manual pages, price lists, brochures, documents | 50 |
| [KICAD/](KICAD/) | KiCad schematics traced from the drawings, the symbol, PCB projects | 10 |
| [OCR/](OCR/) | the note of every file: date, origin, title block, OCR text | 67 |

<!-- module data: tools/module_specs.py, tools/forum_quotes.py -->

## Specifications

From the technical data sheet: [1986 - M5201 - p7.jpg](MANUALS/1986%20-%20M5201%20-%20p7.jpg) page 1 (read by OCR; check against the page). As data: [`Specifications.json`](Specifications.json).

| | |
|---|---|
| **Logic levels** | Standard volt HC series levels. Logic 1: 3.SV min 20 ma source Logic 0: 1V max 20 ma sink. |
| **Status indication** | LED display |
| **Power requirements** | 10/12 volts dc, unregulated 0.5 amp |
| **Circuit protection** | 1.5 amp circuit breaker, current Limiting regulators and overvoltage protecting zener diode. |
| **Discrete control inputs** | Opto-isolators maybe strapped for or 12 to 24 volt operation. 10 ma nominal control current |
| **Discrete control outputs** | Dry relay contacts 24V dc at 50 ma max |
| **Ambient temperature** | to 60 degrees Celsius |
| **Dimensions** | 19.00&quot; wide 1.75&quot; high 16.00&quot; deep (483 mm 44 mm 406 mm) |
| **Weight** | 10 Ibs 5 0z (4.7 kg) |

## Circuit description

From [1986 - M5201 - p26.jpg](MANUALS/1986%20-%20M5201%20-%20p26.jpg) page 1 (read by OCR; check against the pages). As data: [`CircuitDescription.json`](CircuitDescription.json).

<details><summary>Read it</summary>

**5414-161 MACHINE CONTROL ASSEMBLY**

The serialized data at pin of Uz0 feeds two one shot multivibrators UZZA and u338, which forms pulse width generator with the data clock information applied to pins and 9. U31A OR the Iwo varying pulse widths together (approximately 1.3 microsecond pulse idth for logic and 0.5 microsecond pulse with for logic 0 } The output 2t pin 12 of u314 is the display system cata clock pulse width modulated with the serial bit Pattern data for the alphanumeric dor matrix displays. Tne cecocer U24 subdivides the serial data/clock output into blocks each driving 16 display characters on the SA91-029 display assemblies u25 forms data buffer drives with outputs appearing at JIL pin 12,9,5 and respectively reset clocking signa is fed to the SA91-039 display assemblies _ This serves the purpose of synchronizing the column counters on the external display drivers_ The column clocking and reset information is derived from column counter U21 and the one shot multivibrator u22C and U23B _ millisecond reset Pulse is generated each time the column count is 0 U23A forms column count/reset buffer, the output of which drives the isolation network R38 The appropriate drives appear at J14 pins 15, 11, and 3 The display system clock is produced by the oscillator made up of U294,E,F,R31 R32 and C1o_ The oscillator operates at frequency of 330 kHz. u30 (+7) and u32 016) counter generate the required address and clocking information for RAM U17 and EPROM character generator 419 1 ` External Inputs (refer to drawing B14-161-02-001/3 for detail). Thirty-two inputs are provided to feed unitary information into the M5z00 control system. These inputs are used to feed such control functions as mon tor mutes, solo control, remote channel control _ etc as required by particular St Stereo Television console system _ Refer to the console systems documentation for particular detail. ` '.. The opto-isolated inputs are divided into two sets of sixteen appearing on 37 pin &quot;D&quot; connector J4 and J5.

</details>

<!-- /module data -->

## Mechanical

_Mechanical drawings: front panels, cover plates, metalwork and hardware (-03- drawings), AutoCAD files, each with its `(EXTRACTED).svg` vectors; `<module> - front panel.svg` is the front panel as vectors._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUDZEM3hHR0tRVG8/view?resourcekey=0-N5OkLNzT0phhl4NSOpX4mw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUDZEM3hHR0tRVG8&resourcekey=0-N5OkLNzT0phhl4NSOpX4mw" width="240" alt="1986 - M5201 - 5201-04-001 - MACHINE CONTROL MODULE MODULE LAYOUT.jpg"></a><br><sub>1986|19 · 5201-04-001 - MACHINE CONTROL MODULE MODULE LAYOUT · <a href="MECHANICAL/1986%20-%20M5201%20-%205201-04-001%20-%20MACHINE%20CONTROL%20MODULE%20MODULE%20LAYOUT%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## 3-D model

[`MECHANICAL/M5201.stl`](MECHANICAL/M5201.stl) (GitHub turns it in 3-D) · [view, change and generate it on WBSps.ca](https://wardbecksystems.github.io/WBSps.ca/2026/stl.html?m=M5201)

- **Size:** 483 × 44 mm panel, 406 mm deep, 3.2 mm plate (TECHNICAL DATA: 19.00" wide 1.75" high 16.00" deep (483 mm 44 mm 406 mm))
- **From the drawing:** 3 holes and cut-outs, 0 knobs (front panel: `MECHANICAL/M5201 - front panel.svg`)
- Made by `tools/module_models.py` (→ `MECHANICAL/M5201.model.json`) and `tools/stl/make_stl.mjs` in [WBSps.ca](https://github.com/WardBeckSystems/WBSps.ca); the site makes the same STL from the same JSON.

## Schematics

_Electrical drawings: schematics (-02-), functional diagrams (-01-), component layouts (-06-), wiring (-09-), PCB files (.pcb .dsn), and beside each scan its `(EXTRACTED).svg`: the vectors traced from it._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKbF9OS182NXpZZUk/view?resourcekey=0-8eN2USTXf991ddGeQ7kuCw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKbF9OS182NXpZZUk&resourcekey=0-8eN2USTXf991ddGeQ7kuCw" width="240" alt="1986 - M5201 - 5201-02-001 - SMTCHER OISPLAY PORT OPNON.jpg"></a><br><sub>1986|19 · 5201-02-001 - SMTCHER OISPLAY PORT OPNON · <a href="SCHEMATICS/1986%20-%20M5201%20-%205201-02-001%20-%20SMTCHER%20OISPLAY%20PORT%20OPNON%20(EXTRACTED).svg">vectors</a></sub></td></tr>
</table>

## Pinouts

_Pinouts: the RTO-144 edge connector (connection sheets, connector layouts and rear views, strapping), and the pinout / connections drawings made from them. The module root `RTO.json` lists every contact._

## RTO-144 pinout

Read from 3 pinout pictures (each its own `.pinout.json` beside it). Every contact, with where it was read: [`RTO.json`](RTO.json). How a picture becomes this table: [the pinout decision tree](https://github.com/WardBeckSystems/WBSps.ca/blob/main/2026/Engineering/PINOUTS.md).

| Pin | Signal | Kind | Port | Confidence |
|---|---|---|---|---|
| J4-1 | EXT INPUT 1 - | control_in | EXT INPUT 1 - | high |
| J4-2 | EXT INPUT 2 - | control_in | EXT INPUT 2 - | high |
| J4-3 | EXT INPUT 3 - | control_in | EXT INPUT 3 - | high |
| J4-4 | EXT INPUT 4 - | control_in | EXT INPUT 4 - | high |
| J4-5 | EXT INPUT 5 - | control_in | EXT INPUT 5 - | high |
| J4-6 | EXT INPUT 6 - | control_in | EXT INPUT 6 - | high |
| J4-7 | EXT INPUT 7 - | control_in | EXT INPUT 7 - | high |
| J4-8 | EXT INPUT 8 - | control_in | EXT INPUT 8 - | high |
| J4-9 | EXT INPUT 9 - | control_in | EXT INPUT 9 - | high |
| J4-10 | EXT INPUT 10 - | control_in | EXT INPUT 10 - | high |
| J4-11 | EXT INPUT 11 - | control_in | EXT INPUT 11 - | high |
| J4-12 | EXT INPUT 12 - | control_in | EXT INPUT 12 - | high |
| J4-13 | EXT INPUT 13 - | control_in | EXT INPUT 13 - | high |
| J4-14 | EXT INPUT 14 - | control_in | EXT INPUT 14 - | high |
| J4-15 | EXT INPUT 15 - | control_in | EXT INPUT 15 - | high |
| J4-16 | EXT INPUT 16 - | control_in | EXT INPUT 16 - | high |
| J4-17 | N/C | nc |  | high |
| J4-18 | +5 V | power |  | high |
| J4-19 | +5 V | power |  | high |
| J4-20 | EXT INPUT 1 + | control_in | EXT INPUT 1 + | high |
| J4-21 | EXT INPUT 2 + | control_in | EXT INPUT 2 + | high |
| J4-22 | EXT INPUT 3 + | control_in | EXT INPUT 3 + | high |
| J4-23 | EXT INPUT 4 + | control_in | EXT INPUT 4 + | high |
| J4-24 | EXT INPUT 5 + | control_in | EXT INPUT 5 + | high |
| J4-25 | EXT INPUT 6 + | control_in | EXT INPUT 6 + | high |
| J4-26 | EXT INPUT 7 + | control_in | EXT INPUT 7 + | high |
| J4-27 | EXT INPUT 8 + | control_in | EXT INPUT 8 + | high |
| J4-28 | EXT INPUT 9 + | control_in | EXT INPUT 9 + | high |
| J4-29 | EXT INPUT 10 + | control_in | EXT INPUT 10 + | high |
| J4-30 | EXT INPUT 11 + | control_in | EXT INPUT 11 + | high |
| J4-31 | EXT INPUT 12 + | control_in | EXT INPUT 12 + | high |
| J4-32 | EXT INPUT 13 + | control_in | EXT INPUT 13 + | high |
| J4-33 | EXT INPUT 14 + | control_in | EXT INPUT 14 + | high |
| J4-34 | EXT INPUT 15 + | control_in | EXT INPUT 15 + | high |
| J4-35 | EXT INPUT 16 + | control_in | EXT INPUT 16 + | high |
| J4-36 | CONTROL COMMON | ground |  | high |
| J4-37 | CONTROL COMMON | ground |  | high |
| J6-1 | CONTROL OUTPUT 1 A | control_out | CONTROL OUTPUT 1 | high |
| J6-2 | CONTROL OUTPUT 2 A | control_out | CONTROL OUTPUT 2 | high |
| J6-3 | CONTROL OUTPUT 3 A | control_out | CONTROL OUTPUT 3 | high |
| J6-4 | CONTROL OUTPUT 4 A | control_out | CONTROL OUTPUT 4 | high |
| J6-5 | CONTROL OUTPUT 5 A | control_out | CONTROL OUTPUT 5 | high |
| J6-6 | CONTROL OUTPUT 6 A | control_out | CONTROL OUTPUT 6 | high |
| J6-7 | CONTROL OUTPUT 7 A | control_out | CONTROL OUTPUT 7 | high |
| J6-8 | CONTROL OUTPUT 8 A | control_out | CONTROL OUTPUT 8 | high |
| J6-9 | CONTROL OUTPUT 9 A | control_out | CONTROL OUTPUT 9 | high |
| J6-10 | CONTROL OUTPUT 10 A | control_out | CONTROL OUTPUT 10 | high |
| J6-11 | CONTROL OUTPUT 11 A | control_out | CONTROL OUTPUT 11 | high |
| J6-12 | CONTROL OUTPUT 12 A | control_out | CONTROL OUTPUT 12 | high |
| J6-13 | CONTROL OUTPUT 13 A | control_out | CONTROL OUTPUT 13 | high |
| J6-14 | CONTROL OUTPUT 14 A | control_out | CONTROL OUTPUT 14 | high |
| J6-15 | CONTROL OUTPUT 15 A | control_out | CONTROL OUTPUT 15 | high |
| J6-16 | CONTROL OUTPUT 16 A | control_out | CONTROL OUTPUT 16 | high |
| J6-17 | N/C | nc |  | high |
| J6-18 | SPARE | other |  | high |
| J6-19 | SPARE | other |  | high |
| J6-20 | CONTROL OUTPUT 1 B | control_out | CONTROL OUTPUT 1 | high |
| J6-21 | CONTROL OUTPUT 2 B | control_out | CONTROL OUTPUT 2 | high |
| J6-22 | CONTROL OUTPUT 3 B | control_out | CONTROL OUTPUT 3 | high |
| J6-23 | CONTROL OUTPUT 4 B | control_out | CONTROL OUTPUT 4 | high |
| J6-24 | CONTROL OUTPUT 5 B | control_out | CONTROL OUTPUT 5 | high |
| J6-25 | CONTROL OUTPUT 6 B | control_out | CONTROL OUTPUT 6 | high |
| J6-26 | CONTROL OUTPUT 7 B | control_out | CONTROL OUTPUT 7 | high |
| J6-27 | CONTROL OUTPUT 8 B | control_out | CONTROL OUTPUT 8 | high |
| J6-28 | CONTROL OUTPUT 9 B | control_out | CONTROL OUTPUT 9 | high |
| J6-29 | CONTROL OUTPUT 10 B | control_out | CONTROL OUTPUT 10 | high |
| J6-30 | CONTROL OUTPUT 11 B | control_out | CONTROL OUTPUT 11 | high |
| J6-31 | CONTROL OUTPUT 12 B | control_out | CONTROL OUTPUT 12 | high |
| J6-32 | CONTROL OUTPUT 13 B | control_out | CONTROL OUTPUT 13 | high |
| J6-33 | CONTROL OUTPUT 14 B | control_out | CONTROL OUTPUT 14 | high |
| J6-34 | CONTROL OUTPUT 15 B | control_out | CONTROL OUTPUT 15 | high |
| J6-35 | CONTROL OUTPUT 16 B | control_out | CONTROL OUTPUT 16 | high |
| J6-36 | CONTROL COMMON | ground |  | high |
| J6-37 | CONTROL COMMON | ground |  | high |
| P8-1 | COMMON | ground |  | high |
| P8-2 | N/C | nc |  | high |
| P8-3 | N/C | nc |  | high |
| P8-4 | N/C | nc |  | high |
| P8-5 | NSTB3 | bus | DATA BUS | high |
| P8-6 | NSTB1 | bus | DATA BUS | high |
| P8-7 | NCTL | bus | DATA BUS | high |
| P8-8 | NRD | bus | DATA BUS | high |
| P8-9 | COMMON | ground |  | high |
| P8-10 | N/C | nc |  | high |
| P8-11 | N/C | nc |  | high |
| P8-12 | N/C | nc |  | high |
| P8-13 | N/C | nc |  | high |
| P8-14 | COMMON | ground |  | high |
| P8-15 | AD6 | bus | DATA BUS | high |
| P8-16 | AD4 | bus | DATA BUS | high |
| P8-17 | AD2 | bus | DATA BUS | high |
| P8-18 | AD0 | bus | DATA BUS | high |
| P8-19 | COMMON | ground |  | high |
| P8-20 | COMMON | ground |  | high |
| P8-21 | N/C | nc |  | high |
| P8-22 | N/C | nc |  | high |
| P8-23 | NSTB4 | bus | DATA BUS | high |
| P8-24 | NSTB2 | bus | DATA BUS | high |
| P8-25 | NSTB0 | bus | DATA BUS | high |
| P8-26 | NWR | bus | DATA BUS | high |
| P8-27 | COMMON | ground |  | high |
| P8-28 | N/C | nc |  | high |
| P8-29 | N/C | nc |  | high |
| P8-30 | N/C | nc |  | high |
| P8-31 | N/C | nc |  | high |
| P8-32 | COMMON | ground |  | high |
| P8-33 | AD7 | bus | DATA BUS | high |
| P8-34 | AD5 | bus | DATA BUS | high |
| P8-35 | AD3 | bus | DATA BUS | high |
| P8-36 | AD1 | bus | DATA BUS | high |
| P8-37 | COMMON | ground |  | high |

## Manuals and documents

_Manuals and manual pages, price lists, RTO-144 connection sheets, brochures, ads and other document scans._

<table>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKd01qQUlmcGFBQjQ/view?resourcekey=0-FdyzqngFjalZf3yqKCQNfg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKd01qQUlmcGFBQjQ&resourcekey=0-FdyzqngFjalZf3yqKCQNfg" width="240" alt="1986 - M5201 - p1.jpg"></a><br><sub>1986|19 · p1</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdWxQYzQyajV3Nzg/view?resourcekey=0-1_8J3B3rs5i9egp5dynbuA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdWxQYzQyajV3Nzg&resourcekey=0-1_8J3B3rs5i9egp5dynbuA" width="240" alt="1986 - M5201 - p10.jpg"></a><br><sub>1986|19 · p10</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKMVJncjFmSXJKZ1U/view?resourcekey=0-LpiFPg07MM5oJL9NnbftTQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKMVJncjFmSXJKZ1U&resourcekey=0-LpiFPg07MM5oJL9NnbftTQ" width="240" alt="1986 - M5201 - p11.jpg"></a><br><sub>1986|19 · p11</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTnRnR3lrQU1LT2c/view?resourcekey=0-9ONn--JBmKneJHeFmzXeTw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTnRnR3lrQU1LT2c&resourcekey=0-9ONn--JBmKneJHeFmzXeTw" width="240" alt="1986 - M5201 - p12.jpg"></a><br><sub>1986|19 · p12</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKc2lCTHNkRzE3NDg/view?resourcekey=0-vBDZoUfsujQ_QaCHpXcqNw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKc2lCTHNkRzE3NDg&resourcekey=0-vBDZoUfsujQ_QaCHpXcqNw" width="240" alt="1986 - M5201 - p13.jpg"></a><br><sub>1986|19 · p13</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcC16eUJUSVpvaTA/view?resourcekey=0-1MrMmr1kd94oRsPZ6E7zrA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcC16eUJUSVpvaTA&resourcekey=0-1MrMmr1kd94oRsPZ6E7zrA" width="240" alt="1986 - M5201 - p14.jpg"></a><br><sub>1986|19 · p14</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKanZ1cTU4bzBDLTQ/view?resourcekey=0-6GrQXr09orqK7uuGsiMVMw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKanZ1cTU4bzBDLTQ&resourcekey=0-6GrQXr09orqK7uuGsiMVMw" width="240" alt="1986 - M5201 - p15.jpg"></a><br><sub>1986|19 · p15</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcnZ4LVRIX2FWNk0/view?resourcekey=0-iGaj6dAauIlKexoDHKl4rQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcnZ4LVRIX2FWNk0&resourcekey=0-iGaj6dAauIlKexoDHKl4rQ" width="240" alt="1986 - M5201 - p16.jpg"></a><br><sub>1986|19 · p16</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdkxFRFlyMFYwOFU/view?resourcekey=0-ptfdZGVxjsaZ-9meWreb1w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdkxFRFlyMFYwOFU&resourcekey=0-ptfdZGVxjsaZ-9meWreb1w" width="240" alt="1986 - M5201 - p17.jpg"></a><br><sub>1986|19 · p17</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKM0RPOEM1Q1RKTkE/view?resourcekey=0-BXp1BeHh8dFG6mqZyf7aDQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKM0RPOEM1Q1RKTkE&resourcekey=0-BXp1BeHh8dFG6mqZyf7aDQ" width="240" alt="1986 - M5201 - p18.jpg"></a><br><sub>1986|19 · p18</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOWZTOGp6dEFrZFk/view?resourcekey=0-tH0-7vhriWvtZEd6W7TkBg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOWZTOGp6dEFrZFk&resourcekey=0-tH0-7vhriWvtZEd6W7TkBg" width="240" alt="1986 - M5201 - p19.jpg"></a><br><sub>1986|19 · p19</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRnhuekxpRzhkOVU/view?resourcekey=0-6JteBhMaZiSppYwKRT_61A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRnhuekxpRzhkOVU&resourcekey=0-6JteBhMaZiSppYwKRT_61A" width="240" alt="1986 - M5201 - p20.jpg"></a><br><sub>1986|19 · p20</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOXIzdnJSU2FERUk/view?resourcekey=0-7uKiLcTuGnti29XFxdUhRQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOXIzdnJSU2FERUk&resourcekey=0-7uKiLcTuGnti29XFxdUhRQ" width="240" alt="1986 - M5201 - p21.jpg"></a><br><sub>1986|19 · p21</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKeVBSaUcwSEFaMGM/view?resourcekey=0-bvhmt7pccI2tMkKXuPsQNA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKeVBSaUcwSEFaMGM&resourcekey=0-bvhmt7pccI2tMkKXuPsQNA" width="240" alt="1986 - M5201 - p22.jpg"></a><br><sub>1986|19 · p22</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNHdBbF9GWG83VFU/view?resourcekey=0-mYJpNr5Io-AoTLDwtNSGTQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNHdBbF9GWG83VFU&resourcekey=0-mYJpNr5Io-AoTLDwtNSGTQ" width="240" alt="1986 - M5201 - p23.jpg"></a><br><sub>1986|19 · p23</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZi1JNWpONGZwM00/view?resourcekey=0-gWNB8apvysZehK0ZSi_GWw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZi1JNWpONGZwM00&resourcekey=0-gWNB8apvysZehK0ZSi_GWw" width="240" alt="1986 - M5201 - p24.jpg"></a><br><sub>1986|19 · p24</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdmp6YmhuNHJTMkE/view?resourcekey=0-KsU84sD78WmYJopyHDy-Qw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdmp6YmhuNHJTMkE&resourcekey=0-KsU84sD78WmYJopyHDy-Qw" width="240" alt="1986 - M5201 - p25.jpg"></a><br><sub>1986|19 · p25</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKczRoalBLelg0bU0/view?resourcekey=0-y9mZ3YnH1PWRYcnsODZ7YA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKczRoalBLelg0bU0&resourcekey=0-y9mZ3YnH1PWRYcnsODZ7YA" width="240" alt="1986 - M5201 - p26.jpg"></a><br><sub>1986|19 · p26</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKa3hTakNvZkV6dHM/view?resourcekey=0-TX6TuHoDwrFS-zqkqZ9BHw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKa3hTakNvZkV6dHM&resourcekey=0-TX6TuHoDwrFS-zqkqZ9BHw" width="240" alt="1986 - M5201 - p27.jpg"></a><br><sub>1986|19 · p27</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTXlVQnZDQ0J1ejg/view?resourcekey=0-8PXhOHolNRG0gOvSMRkAyw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTXlVQnZDQ0J1ejg&resourcekey=0-8PXhOHolNRG0gOvSMRkAyw" width="240" alt="1986 - M5201 - p28.jpg"></a><br><sub>1986|19 · p28</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKLXl1RldkQllMUGs/view?resourcekey=0-_FurW1G8hUyklOYh-UUoUQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKLXl1RldkQllMUGs&resourcekey=0-_FurW1G8hUyklOYh-UUoUQ" width="240" alt="1986 - M5201 - p29.jpg"></a><br><sub>1986|19 · p29</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQTJpc0dhTFdjOGM/view?resourcekey=0-xMy9aOj9I7OO9qPudBBSjQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQTJpc0dhTFdjOGM&resourcekey=0-xMy9aOj9I7OO9qPudBBSjQ" width="240" alt="1986 - M5201 - p3.jpg"></a><br><sub>1986|19 · p3</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNExmaHcySXNfZE0/view?resourcekey=0-Kt3gcPU4L-NBUfFAv9lOaw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNExmaHcySXNfZE0&resourcekey=0-Kt3gcPU4L-NBUfFAv9lOaw" width="240" alt="1986 - M5201 - p30.jpg"></a><br><sub>1986|19 · p30</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOVA3WmxwT3pHX2s/view?resourcekey=0-JNAwh_rA2NTga9aVuyO2sQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOVA3WmxwT3pHX2s&resourcekey=0-JNAwh_rA2NTga9aVuyO2sQ" width="240" alt="1986 - M5201 - p31.jpg"></a><br><sub>1986|19 · p31</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKV002VG9weWFiRWc/view?resourcekey=0-WmPCJdIC7B_Pnih1MAhUJA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKV002VG9weWFiRWc&resourcekey=0-WmPCJdIC7B_Pnih1MAhUJA" width="240" alt="1986 - M5201 - p32.jpg"></a><br><sub>1986|19 · p32</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKZ3hYLXM3dVRPMVU/view?resourcekey=0-PjB3pUCBEgcVTsS2cgoQ7w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKZ3hYLXM3dVRPMVU&resourcekey=0-PjB3pUCBEgcVTsS2cgoQ7w" width="240" alt="1986 - M5201 - p33.jpg"></a><br><sub>1986|19 · p33</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKV3FiNHpXM3dCb0k/view?resourcekey=0-SpfAFQTBtiHvvOlXHf0fNA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKV3FiNHpXM3dCb0k&resourcekey=0-SpfAFQTBtiHvvOlXHf0fNA" width="240" alt="1986 - M5201 - p34.jpg"></a><br><sub>1986|19 · p34</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKVlotVy1DM2g4N1U/view?resourcekey=0-Y3DxGtJIoPJ9WsJ-gUAsqQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKVlotVy1DM2g4N1U&resourcekey=0-Y3DxGtJIoPJ9WsJ-gUAsqQ" width="240" alt="1986 - M5201 - p35.jpg"></a><br><sub>1986|19 · p35</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOGhTdmU5a2IzaE0/view?resourcekey=0-1alQoSWcs3u6ddhyoZeiWg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOGhTdmU5a2IzaE0&resourcekey=0-1alQoSWcs3u6ddhyoZeiWg" width="240" alt="1986 - M5201 - p37.jpg"></a><br><sub>1986|19 · p37</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdVpjc3FSX0RBU00/view?resourcekey=0-VS5bvJlntAlEjLA4ujxKqg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdVpjc3FSX0RBU00&resourcekey=0-VS5bvJlntAlEjLA4ujxKqg" width="240" alt="1986 - M5201 - p38.jpg"></a><br><sub>1986|19 · p38</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKeHMwTEZWcjgxVk0/view?resourcekey=0-5LXg7dKjs9PnbKhWUoIbug" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKeHMwTEZWcjgxVk0&resourcekey=0-5LXg7dKjs9PnbKhWUoIbug" width="240" alt="1986 - M5201 - p39.jpg"></a><br><sub>1986|19 · p39</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKc050a2pyMHp6eEU/view?resourcekey=0-HF0HyRTOawnvykvc30ivOQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKc050a2pyMHp6eEU&resourcekey=0-HF0HyRTOawnvykvc30ivOQ" width="240" alt="1986 - M5201 - p4.jpg"></a><br><sub>1986|19 · p4</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRzJ6VTlfU2FrMkU/view?resourcekey=0-mzUXuqN0sex7tFtBC8BghQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRzJ6VTlfU2FrMkU&resourcekey=0-mzUXuqN0sex7tFtBC8BghQ" width="240" alt="1986 - M5201 - p41.jpg"></a><br><sub>1986|19 · p41</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKV2Q2YTdkY25vNW8/view?resourcekey=0-KvANZ-EBMvek1MLJG0Kwsw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKV2Q2YTdkY25vNW8&resourcekey=0-KvANZ-EBMvek1MLJG0Kwsw" width="240" alt="1986 - M5201 - p42.jpg"></a><br><sub>1986|19 · p42</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKSFJrcmpJcG9aME0/view?resourcekey=0-kHaojFrJQNDxIgrvjjbwJw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKSFJrcmpJcG9aME0&resourcekey=0-kHaojFrJQNDxIgrvjjbwJw" width="240" alt="1986 - M5201 - p43.jpg"></a><br><sub>1986|19 · p43</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKb0ZWUXJ6Szk4OTA/view?resourcekey=0-kZ88JgottHq_QgyZkqFkOg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKb0ZWUXJ6Szk4OTA&resourcekey=0-kZ88JgottHq_QgyZkqFkOg" width="240" alt="1986 - M5201 - p44.jpg"></a><br><sub>1986|19 · p44</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKNlU3ZDU1OWFSY0E/view?resourcekey=0-SA9HByb3eghQl4V880MVFg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKNlU3ZDU1OWFSY0E&resourcekey=0-SA9HByb3eghQl4V880MVFg" width="240" alt="1986 - M5201 - p45.jpg"></a><br><sub>1986|19 · p45</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKQ3FWYWtacXRFZjQ/view?resourcekey=0-y4Bf-_rXzAFP9GUG9JCkUg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKQ3FWYWtacXRFZjQ&resourcekey=0-y4Bf-_rXzAFP9GUG9JCkUg" width="240" alt="1986 - M5201 - p46.jpg"></a><br><sub>1986|19 · p46</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKS082Sy0tTGtEckU/view?resourcekey=0-Xbh_rwmr7kh6YX0uAUY7TA" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKS082Sy0tTGtEckU&resourcekey=0-Xbh_rwmr7kh6YX0uAUY7TA" width="240" alt="1986 - M5201 - p47.jpg"></a><br><sub>1986|19 · p47</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKS0FCQTRHQS1NNk0/view?resourcekey=0-hKjljznReFEbym_jtjraUw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKS0FCQTRHQS1NNk0&resourcekey=0-hKjljznReFEbym_jtjraUw" width="240" alt="1986 - M5201 - p48.jpg"></a><br><sub>1986|19 · p48</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKcHhiQ1JXN2l0U2s/view?resourcekey=0-7u933VG70CEgxZq9IGVtQQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKcHhiQ1JXN2l0U2s&resourcekey=0-7u933VG70CEgxZq9IGVtQQ" width="240" alt="1986 - M5201 - p5.jpg"></a><br><sub>1986|19 · p5</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKOGdVMXRtcE9MYWc/view?resourcekey=0-gg4oOOM5XE8QihV00cE0OQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKOGdVMXRtcE9MYWc&resourcekey=0-gg4oOOM5XE8QihV00cE0OQ" width="240" alt="1986 - M5201 - p6.jpg"></a><br><sub>1986|19 · p6</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKLUxXX1pmSVVQV2M/view?resourcekey=0-oioGzZG8V0pBoHz7NXQMSw" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKLUxXX1pmSVVQV2M&resourcekey=0-oioGzZG8V0pBoHz7NXQMSw" width="240" alt="1986 - M5201 - p7.jpg"></a><br><sub>1986|19 · p7</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKTFQ2YTFpcEtqbjA/view?resourcekey=0-4ymGIWfPAU5Vh82F6ToTEg" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKTFQ2YTFpcEtqbjA&resourcekey=0-4ymGIWfPAU5Vh82F6ToTEg" width="240" alt="1986 - M5201 - p8.jpg"></a><br><sub>1986|19 · p8</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUjUzVmJmMm56R28/view?resourcekey=0-fVm_okG6c3TSc5gqHsiQew" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUjUzVmJmMm56R28&resourcekey=0-fVm_okG6c3TSc5gqHsiQew" width="240" alt="1986 - M5201 - p9.jpg"></a><br><sub>1986|19 · p9</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKdUFnc1docHZKTnM/view?resourcekey=0-Al0jKi5JMDfiTY4mbQuzag" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKdUFnc1docHZKTnM&resourcekey=0-Al0jKi5JMDfiTY4mbQuzag" width="240" alt="1987 - M5201 - p2.jpg"></a><br><sub>1987|20 · p2</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKUFV4MGFvQ3ktLTQ/view?resourcekey=0-JZmhiO3OmQ7R56cZwIwK0w" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKUFV4MGFvQ3ktLTQ&resourcekey=0-JZmhiO3OmQ7R56cZwIwK0w" width="240" alt="1987 - M5201 - p36.jpg"></a><br><sub>1987|20 · p36</sub></td><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKckRJX0lvUHlXblU/view?resourcekey=0-Qp3p4aoJEFI_aesiB2VtDQ" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKckRJX0lvUHlXblU&resourcekey=0-Qp3p4aoJEFI_aesiB2VtDQ" width="240" alt="1987 - M5201 - p40.jpg"></a><br><sub>1987|20 · p40</sub></td></tr>
<tr><td align="center" valign="top" width="33%"><a href="https://drive.google.com/file/d/0B0yR0b5T78SKRk9uUUFMSHN6NWs/view?resourcekey=0-lJj9wE69ZJbzM-_k_6va0A" title="Open on Google Drive"><img src="https://drive.google.com/thumbnail?sz=w480&id=0B0yR0b5T78SKRk9uUUFMSHN6NWs&resourcekey=0-lJj9wE69ZJbzM-_k_6va0A" width="240" alt="19xx - M5201 - AD - WBSPS - AD - LS series 003.jpg"></a><br><sub>19xx - M5201 - AD - WBSPS - AD - LS series 003</sub></td></tr>
</table>

## KiCad

_KiCad: a schematic (`.kicad_sch`) traced from each electrical drawing, the module symbol (`.kicad_sym`) and its PCB projects. Traced schematics are the line work only: redraw with symbols over them._

- [1986 - M5201 - 5201-02-001 - SMTCHER OISPLAY PORT OPNON.kicad_sch](KICAD/1986%20-%20M5201%20-%205201-02-001%20-%20SMTCHER%20OISPLAY%20PORT%20OPNON.kicad_sch)
- [1986 - M5201 - [DWG 14-089-02-001].kicad_sch](KICAD/1986%20-%20M5201%20-%20%5BDWG%2014-089-02-001%5D.kicad_sch)
- [1986 - M5201 - [DWG 14-141-02-001].kicad_sch](KICAD/1986%20-%20M5201%20-%20%5BDWG%2014-141-02-001%5D.kicad_sch)
- [1986 - M5201 - [DWG 14-161-02-001] - MACHINE' CONTROL ASSEMBLY SCHEMATIC.kicad_sch](KICAD/1986%20-%20M5201%20-%20%5BDWG%2014-161-02-001%5D%20-%20MACHINE%27%20CONTROL%20ASSEMBLY%20SCHEMATIC.kicad_sch)
- [1986 - M5201 - [DWG 14-161-02-001] - UJO UJI FOO ROO.kicad_sch](KICAD/1986%20-%20M5201%20-%20%5BDWG%2014-161-02-001%5D%20-%20UJO%20UJI%20FOO%20ROO.kicad_sch)
- [1986 - M5201 - [DWG 14-161-02-001] - UJSE RJID FUT USF.kicad_sch](KICAD/1986%20-%20M5201%20-%20%5BDWG%2014-161-02-001%5D%20-%20UJSE%20RJID%20FUT%20USF.kicad_sch)
- [1986 - M5201 - [DWG 14-161-02-001].kicad_sch](KICAD/1986%20-%20M5201%20-%20%5BDWG%2014-161-02-001%5D.kicad_sch)
- [1986 - M5201 - [DWG 91-039-02-001] - ASSEMBLY SCHEMATIC.kicad_sch](KICAD/1986%20-%20M5201%20-%20%5BDWG%2091-039-02-001%5D%20-%20ASSEMBLY%20SCHEMATIC.kicad_sch)
- [19xx - 5201-02-001 - MACHINE CONTROL MODULE SCHEMATIC - ISS 1.kicad_sch](KICAD/19xx%20-%205201-02-001%20-%20MACHINE%20CONTROL%20MODULE%20SCHEMATIC%20-%20ISS%201.kicad_sch)
- [M5201.kicad_sym](KICAD/M5201.kicad_sym)

---
Archive: Anthony Peter Kuzub · [WBSps.ca](https://WBSps.ca) · [WBSps.Kuzub.com](https://WBSps.Kuzub.com)

# Ninety4co "Swap Wiring" re-pin sheet (reference copy)

Source: Google Sheet linked in every episode of *The VR6 MK6 Swap* (Ninety4co, Choby / @chobester).
https://docs.google.com/spreadsheets/d/1RIhUj4_f6G1ZhraDKugaOQ0ZXPTq9BtquM9f8qgIkq4/edit
Sheet marked *work in progress, last updated 6/27/2024*. Copied 2026-10-08; cell text is his, including spelling.

His warning, which applies doubly to a Jetta: this is for **his** car only, a **2010 GTI CCTA manual high-line**. Do the re-pins at your own risk, and get **factory VW wiring diagrams for both the recipient car and the donor** to verify every pin. Our Mk6 Jetta's body harness and fuse box differ from a Mk6 GTI, so treat this as a map of *which circuits* need attention, not as pin numbers to copy.

Column meanings: **GTI** = pin on the GTI-side connector; **Action**: `>` move to, `X` remove, `$` stays, `+`/`add` new wire; **BLV** = pin where the 3.6 (BLV) ECU/fuse box expects it.

Connector names: **T94** = engine ECU connector (94-pin); **T40**, **T26**, **T30**, **T14** = connectors on the engine-bay fuse/relay box. He stresses you need the **Passat "high" fuse box** (part 1K0 937 124 K) because it carries the **T40 and T26** connectors the 3.6 harness uses.

## Fuse box wiring

| GTI | Action | BLV | Assignment | Notes |
|-----|--------|-----|------------|-------|
| t40/2 | $ | | | |
| t40/3 | $ | | | |
| t40/13 | > | t40/40 | Fuel pressure regulator /1 | this is a circuit from t14/8 |
| t94/27 | > | t94/33 | | now splice in a wire from your new t94/33 to t40/10 |
| t40/12 | $ | | | |
| t40/16 | $ | | | |
| t40/16 | > | | switched 12V for O2s | |
| t40/17 | $ | | | |
| t40/18 | $ | | | |
| t40/30 | > | t40/20 | terminal 30 | |
| t40/23 | $ | | | |
| t40/24 | $ | | | |
| t40/25 | $ | | | |
| t40/27 | $ | | | |
| t40/38 | > | t40/30 | VECM | terminal 30 |
| t40/31 | $ | | | |
| t40/33 | > | t30/32 | terminal 15 relay 2 | |
| t40/19 | > | t40/33 | ignition coils 12V | this is a circuit off of t14/5 |
| t40/34 | $ | | | |
| t40/15 + 28 | > | t26/7 + 12 | position connection 11 | |
| t40/8 + 11 | > | t40/37 | connection 87 | **DO THIS FIRST** |
| t40/8 | NEW WIRE | t26/3 | recirc pump relay | **DO THIS SECOND** |
| T94/69 | > | t26/4 | ECM relay | |
| t40/26 | > | t26/9 | leak detection pump pin 3 | |
| t14/3 | > | t26/11 | coolant recirc pump | |
| t94/92 | > | t26/12 | position connection 11 | spliced into the existing pin swap on t26/12 (line above) |
| t40/22 | > | t26/14 | position connection 5 | |
| t94/87 | > | t26/24 | ECM relay 2 | splice and add |
| t94/28 | > | t94/32 | ECM relay 2 | |
| T40/9 | > | T26/25 | ECM relay 2 | do this and the line above in this order; GTI t40/9 is tied to the wire moved in the last step |

## Power feeds into the front of the fuse box

Looking at the front of the box, left to right, 10 poles. "Remember you need the Passat high box (T40 and T26 connector)."

| Pole (L→R) | Assignment | Amp |
|-----------|------------|-----|
| 1 | alternator charge-back | 150 or 200 (solid metal maxi-fuse) |
| 2 | power steering | 80 |
| 3 | coolant fan module | 50 |
| 4 | battery | unfused |
| 5 | fuse panel C | 80 |
| 6 | not used | — |
| 7 | battery | 125 |
| 8 | not used | — |
| 9 | not used | — |
| 10 | battery | 80 |

## ECU connector (T94) wiring

| GTI | Action | BLV | Assignment | Notes |
|-----|--------|-----|------------|-------|
| T94/50 | > | T94/28 | coolant fan module | |
| t94/36 | > | t94/26 | coolant temp sensor | |
| t94/49 | > | t94/8 | leak detect pump /2 | |
| t94/44 | > | t94/40 | leak detect pump /1 | LDP/3 is a ground, no switching needed |
| t94/45 | > | t94/18 | cruise | **unverified**; he still needs to revisit, maybe more coding |
| t94/19 | > | t94/25 | brake light switch | |
| t94/30 | > | t94/27 | fuel pump module | |
| t14/7 | > | t94/35 | low fuel pressure sensor | |
| t94/34 | X | | GTI O2 bank 2 | |
| t94/62 | X | | GTI O2 bank 2 | |
| t94/29 | X | | GTI O2 bank 2 | |
| t94/56 | X | | GTI O2 bank 1 | |
| t94/57 | X | | GTI O2 bank 1 | |
| t94/78 | X | | GTI O2 bank 1 | |
| t94/79 | X | | GTI O2 bank 1 | |
| t94/73 | X | | GTI O2 bank 1 | |
| cut | | | GTI B1 O2 pin 4 | cut at the connector; reuse for B1 and B2 O2 sensors pin 4 |
| t94/23 | X | | GTI MAF pin 1 | |
| t94/65 | X | | GTI MAF pin 2 | |
| cut | | | GTI MAF pin 3 | switched power; cut and reuse for the 3.6 MAF |
| add | + | t94/73 | O2 B2 pin 3 | |
| add | + | t94/83 | O2 B2 pin 5 | |
| add | + | t94/59 | O2 B2 pin 1 | |
| add | + | t94/84 | O2 B2 pin 2 | |
| add | + | t94/62 | O2 B2 pin 6 | |
| add | + | t94/51 | O2 B1 pin 3 | |
| add | + | t94/61 | O2 B1 pin 2 | |
| add | + | t94/82 | O2 B1 pin 6 | |
| add | + | t94/81 | O2 B1 pin 5 | |
| add | + | t94/60 | O2 B1 pin 1 | |
| add | + | t94/13 | 3.6 MAF pin 3 | |
| add | + | t94/22 | 3.6 MAF pin 1 | |
| add | + | t94/64 | 3.6 MAF pin 4 | |
| add | + | t94/42 | 3.6 MAF pin 2 | |
| t94/81 | > | t94/58 | throttle pedal pin 1 | |
| t94/82 | > | t94/80 | throttle pedal pin 2 | |
| t94/35 | > | t94/78 | throttle pedal pin 3 | |
| t94/83 | > | t94/79 | throttle pedal pin 4 | |
| t94/11 | > | t94/56 | throttle pedal pin 5 | |
| t94/61 | > | t94/57 | throttle pedal pin 6 | |

## What the sheet tells us, in plain terms

The circuits that had to change when a BLV ECU and harness went into a PQ35 car with a 2.0T body harness:

1. **Power distribution**: terminal 30 (constant), terminal 15 (switched), connection 87, and the two ECM relays sit on different fuse-box pins. The 3.6 also needs the **T26** connector, which only the Passat/VR6 "high" fuse box has.
2. **Coolant after-run (recirculation) pump** and its relay: new circuit, the TSI car has none in this form.
3. **Coolant fan module** and **coolant temp sensor**: ECU pins move.
4. **EVAP leak detection pump**: pins move.
5. **Fuel**: fuel pump module control and the low-pressure fuel sensor move; a fuel pressure regulator circuit is added.
6. **Four O2 sensors become four on two banks**: every GTI O2 wire is removed and the 3.6's bank 1 / bank 2 sensors are pinned fresh.
7. **MAF**: TSI MAF wires removed, 3.6 MAF added on four new pins.
8. **Throttle pedal**: all six pins move (drive-by-wire on both cars, different pinout).
9. **Brake light switch** and **cruise** move; cruise was still unverified as of 6/2024.
10. **Ignition coil 12V** and **switched 12V for the O2 heaters** come from different fuse-box pins.

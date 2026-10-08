# Ninety4co, "The VR6 MK6 Swap" (Parts 1–5): deep analysis

A 3.6L VR6 (BLV, from a B6 Passat) swapped into a **2010 Mk6 GTI** with a **manual 02M** gearbox, done alone in a home garage in North Carolina by Choby (Ninety4co, Instagram @chobester) between **August 2023 and ~March 2024**. Five episodes, released weekly from 6 March to 3 April 2024.

Why it matters for us: it is the closest documented precedent to our plan (3.6 VR6 into a PQ35-family Mk6 car that never had a VR6), and he published a **parts list with VW part numbers** and a **pin-by-pin wiring sheet**. Both are copied into `sources/`.

All five episodes are analyzed from full transcripts (`transcripts/`; YouTube auto-captions, so expect a few misheard words).

| Episode | Length | Released | Covers |
|---|---|---|---|
| [Part 1: Engine Teardown!](https://youtu.be/uERxnHlgF-o) | 20:25 | 2024-03-06 | Engine assessment, teardown to the block, powder coating, head off to the machine shop |
| [Part 2: Drivetrain is Complete!](https://youtu.be/wTqhQoPT48I) | 29:37 | 2024-03-13 | 02M rebuild with steel forks, block paint, timing, long-block assembly, clutch |
| [Part 3: Engine is in! But will it run?](https://youtu.be/Z0YHrkM1E1Q) | 29:05 | 2024-03-20 | TSI out, bay trimmed and painted, VR6 in on junkyard mounts, downpipes, first start |
| [Part 4: Wiring deep dive, final assembly, first drive](https://youtu.be/6Gg6oTTig4Y) | 30:53 | 2024-03-27 | Harness breakdown, fuse box, troubleshooting, cooling plumbing, first drive |
| [Part 5: We did it (goodbye, for now)](https://youtu.be/-DIJFHw3njE) | 11:07 | 2024-04-03 | Tune, permanent mounts partnership, final drive |

Sources: [parts list (Google Doc)](https://docs.google.com/document/d/1lUm4Pee3PA9zaG5dA_x5aLbu-WO3YJs_4todYXtXFYo/edit), [wiring sheet (Google Sheet)](https://docs.google.com/spreadsheets/d/1RIhUj4_f6G1ZhraDKugaOQ0ZXPTq9BtquM9f8qgIkq4/edit), both last updated 2024-06-27. Local copies: `sources/ninety4co-swap-parts-list.md`, `sources/ninety4co-swap-wiring-repins.md`.

---

## 1. The build at a glance

| | What he used | Where it came from |
|---|---|---|
| Recipient | 2010 Mk6 GTI, CCTA 2.0T, 6-speed manual, high-line | His own show car (air ride, trunk battery) |
| Engine | 3.6L VR6 **BLV**, ~171,000 mi | Junkyard B6 Passat 3.6, pulled 8 Aug 2023 |
| Engine rebuild | Full timing kit, new oil pump + one-piece sprocket, head decked and chem-cleaned, valve stem seals, head gasket and bolts, new injectors, new OEM engine harness | FCP Euro, UroTuning, dealer, machine shop |
| Gearbox | **02M 6-speed manual** from a 24V VR6 (FWD), with OEM steel shift forks | Facebook Marketplace, $400 including forks |
| Clutch | South Bend Stage 2 Daily, single-mass flywheel, Mk4 24V application (K70287-HD-DMF) | UroTuning |
| Mounts | PQ35 VR6 engine mount (R32/Eos 3.2/TT 3.2), PQ35 2.5L 5-speed trans mount, stock Mk6 dogbone. Junkyard units first, then **Black Forest Industries** performance mounts (sponsored) in Part 5 | Junkyard Eos 3.2; BFI, Cary NC |
| Axles, shifter | Stock Mk6 manual axles, stock Mk6 shift box and cables | Already in the car |
| Fuel | Passat 3.6 pump module (3C0 906 093 A), 4.0-bar regulator/filter (6Q0 201 051 J) | — |
| Exhaust | USP Mk5 R32 high-flow cat downpipes, cat-back of choice | USP Motorsports |
| Cooling | Mishimoto Mk5 R32 radiator, Gray Fabrication swirl pot (deletes the coolant bottle), 2018 Passat GT hoses, after-run pump | — |
| A/C | Stock Mk6 condenser and high-pressure line; PQ35 VR6 suction line (1K0 820 743 CE); 3.6 compressor (1K0 820 808 F) | Eos 3.2 donor line |
| Electrical | BLV ECU and engine harness; **Passat/VR6 "high" fuse box (1K0 937 124 K)** with its cabling; GTI body harness re-pinned | Junkyard fuse box, dealer harness |
| Tune | Reflect Tuning (Ian, North Carolina), done after the first drives: cleared the remaining codes, "zero lights on the dash." How the immobilizer was handled is never shown on camera | In person or mail-in ECU |
| Time | Teardown Aug 2023 → engine in ~Feb 2024 ("almost 6 months to the day") → driving March 2024 | Solo, around a newborn and a business |

---

## 2. Episode by episode

### Part 1: Engine teardown (20:25)

- **0:00–1:42** Premise. "I want it to be a DIY swap, an at-home swap." No lift, no employees, one camera. The footage starts in August 2023.
- **1:42** Day one. Plan: strip the engine "basically to the block": mount bracket, harness, cooling hoses, accessories, every bracket, intake manifold. Engine shows 171,000 miles. Water in the intake tract, swollen coolant hoses, worm-clamp "repairs" from a previous shop, the plastic coolant "crack pipe" replaced with a metal one.
- **5:04** Valve cover gasket had been leaking "pretty much everywhere." Oil pan off. The 02M has already been bought ("more on that later").
- **6:00–8:00** Both metal timing covers off. **Key fact he repeats across the series: the VR6's timing is on the transmission side.** Someone had been in there before (excess RTV), so he assumed the timing had been done once already but redid it anyway with an OEM-supplier kit: both chains, both tensioners, all guides.
- **8:00–12:14** Powder coating at his shop: satin black for brackets, coolant pipes, accessory bracket, heat shield, mount bracket, oil pan; silver-vein plus gloss clear on the timing covers; valve cover white to match the wheels. Cosmetic, but it is why the engine came apart to the bare block.
- **12:14–18:36** Head removal: cam phasers, chain, HPFP and its drive gear, cam bridge with solenoids, cams. Cam bearings "typical wear for 170,000 miles," no scoring. Twenty head bolts in two lengths (he says 7 and 13). No sludge inside; pistons carboned but nothing blown through. Three-layer head gasket. Head goes to Bush's Automotive (central NC) for decking and a chem bath.
- **18:36** Machine shop confirms the cam caps look fine.

What to take from it: he bought a high-mileage junkyard engine *and* committed to a near-full top-end refresh plus timing before it ever went in. The doc says the minimum is "redo the timing," because once the engine and trans are in the car it cannot be done.

### Part 2: Drivetrain is complete (29:37)

- **1:01** "About 4 months of footage went into this one." He **scrapped the original engine harness** for broken connectors; a new OEM BLV harness was "really cheap at the dealer." Lower timing (crank chain, oil pump, guides) already torn down.
- **2:02** The gearbox: a **24V VR6 02M 6-speed**, which "will bolt right up" to the 3.6, using a Mk4 24V clutch/flywheel application. Found on Marketplace with OEM steel shift forks for **$400** total. (The captions say "Mark V"; his doc says his box is a **Mk4** 02M with the 2-bolt mount pattern. Trust the doc.)
- **2:02–4:40** He splits the case having never done one. Lesson shown rather than said: lay out the gear stacks, photograph everything.
- **4:40–7:41** Powder coats the case anyway, then degreases and pressure washes to get media out. Reassembly: diff, three gear stacks, input shaft, shift tower, gasket maker. **Input shaft and axle seals he bought were the wrong size**; correct ones arrive by 28:10.
- **8:02** 20 September 2023, "about a month in." Block painted with Rustoleum rusty-metal primer and flat black engine enamel, foam brushes, 24 h between coats.
- **12:01** Head back from the machine shop. Carbon was bad enough that the shop pulled every valve, so they did **valve stem seals** too. Head on with a new gasket and new bolts; cams, caps with new hardware, cam bridge, and a **new updated oil pump**, all to spec. Not filmed: "I didn't want to miss anything."
- **14:01** He found the **factory service manual for the BLV in the B6 Passat** (~300 pages) and recommends it for torque specs, procedures, and the reuse/replace list.
- **15:08–17:01 Timing.** New oil-pump chain tensioner and guide, new oil pump, **new one-piece oil pump sprocket and 12.9 bolt ("these are known to back themselves out")**, new upper tensioner and guides, new chain. Marks: 16 rollers between the cam sprocket marks aligned to the notches on the cam bridge; crank mark to the seam on the main cap; two crank revolutions and recount. Cam adjuster sprocket bolts replaced with new from the dealer.
- **17:01** Reality check: 7–8 months in, three days of camera help in total.
- **18:02–23:00 The long block.** Two-piece intake manifold chosen over one-piece so the upper half comes off in the car (with the one-piece, a valve cover gasket would need the front clip off). Rebuilt alternator, new tensioner and idler pulleys and belt, new OEM harness, new crank pulley cover and gasket, fuel rail with new injectors, EVAP hardware taken from a second junkyard car so it stays OEM. **Schimmel Performance (SP Turbo) billet oil filter stand**: converts to a spin-on filter and deletes the plastic anti-drainback valve in the OEM housing, which "is known to fail" and can end up inside the engine.
- **23:00–26:07 Clutch.** South Bend Stage 2 Daily with a lightened single-mass flywheel and new hardware, surfaces cleaned with brake clean, Loctite. He wanted a DKM but none existed for this application. Doc: **do not run a stock 24V clutch; it will not hold the 3.6's torque even untuned.**
- **28:10** Correct seals in, trans bolted on, junkyard Mk4 02M starter. "Fully assembled manual-swapped 3.6 drivetrain." The GTI is already being torn down.

### Part 3: Engine is in (29:05)

- **1:01** TSI removal: coolant drained, **A/C discharged at a shop first**, engine and 02Q out together from below: lower control arms dropped, axles out, downpipe off the turbo.
- **2:08** Bay prep: the **front half of the driver-side mount "bucket" trimmed**, spot welds drilled, unused brackets and studs removed, body filler and seam sealer. Goal "OEM-plus," not a shaved bay; the fuse box stays where it is.
- **3:55** It is now early January 2024. Delays: newborn (Oscar, six months), holidays, and the business taking off.
- **5:34–7:00** Not swap-related but relevant to the first start later: **battery is an Optima relocated to the trunk** behind a plexiglass panel, with a circuit breaker; air tank on an ECS hatch brace. Audi S5 seats.
- **7:00–8:00** More bay trimming: coolant bottle bracket deleted (the swirl pot replaces the bottle), washer-fluid/mount support bracket and frame-rail studs removed, battery tray "ears" cut off, ground tabs relocated, unneeded wiring identified and trimmed.
- **9:00–14:00** Bay painted with Era Paints aerosols in LB9A Candy White: two coats primer, three colour, three 2K clear, two kits exactly. Not sponsored.
- **16:20 Engine in.** The junkyard had an **Eos 3.2**, so he pulled its **VR6 engine mount** and a **Mk5/6 2.5L trans mount** as placeholders until the permanent mounts.
- **18:14 The money quote.** "A Mk5/Mk6 2.5L 5-speed transmission mount works with our 24-valve 02M. I did not have to modify a single thing." "A Mk5/Mk6 VR mount (Mk5 R32, Eos 3.2, Mk2 TT 3.2) bolts onto our engine mount bracket." "Dog bone mount bolts right up." Only complaint: **"tight side to side."**
- **19:00** First fitment problem: the **TSI compressor-to-evaporator A/C line will not fit** the 3.6's lower compressor position. Fix is the Eos 3.2 line (1K0 820 743 CE in the doc).
- **20:02** Install technique: no load leveler, engine walked in slowly with a jack under the trans. "A lot of this stuff is available at junkyards, at the dealer, online, off the shelf."
- **21:00 Downpipes.** USP Mk5 R32 high-flow-cat downpipes, because the BLV has the same angled manifold outlets as the Mk5 R32's 3.2 and the chassis is PQ35. Result: "fitment was not the greatest," and the **shifter cables** need attention near the pipes.
- **22:03 First-start wiring, in his words:** (1) swapped a pin on the GTI body harness so **fuel pump module power** lands where the Passat expects it; (2) **removed all four GTI O2 sensors** with their wiring; (3) **re-pinned the accelerator pedal** (both cars are drive-by-wire, different pinout); (4) **jumped 12 V between body and engine harness** to a few connectors. Full explanation promised for Part 4.
- **23:44–29:00 First start**, with friends Ethan (VW tech) and Ryan (swap veteran). Running "straight battery power with a tender." Fuel pump primes; a fitting is finger-tight and weeps. Key on, throttle body responds to the pedal. Cranking: the starter clicks once and stops; the **trunk-battery circuit breaker trips twice**; "I don't have enough juice." Then it fires.

### Part 4: Wiring deep dive, final assembly, first drive (30:53)

The most useful episode for us. He warns it is "nerdy and techy" and it is.

- **2:01–4:02 The connector map.** The BLV ECU has two connectors: **T60** to the *engine* harness and **T94** to the *body* harness through the firewall. "The T60: we didn't have to do anything to that." All the work is on the T94. The Passat fuse box has a **T40** and a **T26** on its underside. A **T14** connector bridges the engine harness and the body harness (switched 12 V to injectors, coils, PCV heater, fuel pressure regulator, and more).
- **4:02 What he had to work with.** He cut the body harness out of the donor Passat at the firewall, so he owned the Passat T94 connector with every loom and pigtail, plus the Passat fuse box. That is why he could re-pin instead of splice.
- **4:02–6:01 What got the car running in Part 3**, in order: fuel pump module signal wire re-pinned on the T94; GTI upstream and downstream O2 sensors, MAF and MAP removed; Passat MAF and primary O2s added to the T94 as the Passat pins them; one pin jumped from the T14 up to the T94 (he cannot remember which); GTI throttle pedal re-pinned. Pedal note: both cars' pedals have the same pinout and even the same wire colours, so it is six wires moved on the T94.
- **6:01–7:00 Why the Passat fuse box became mandatory.** The car ran, but a relay kept clicking, even key-out. Voltage checks everywhere led to the diagnosis: the GTI box has fewer relays, circuits and pin allocations, so "we were trying to feed too much stuff into too small of a circuit" and relays back-fed and stuck. Hence the **Passat "high box."**
- **7:00–8:02 Pins that move on the T94:** leak detection pump (two of its three pins), coolant temp sensor on the radiator outlet (two pins), cruise control signal, brake light switch. He discovered the last one because **all brake lights including the third were stuck on** after first start. What plugged straight in: the A/C system and the alternator charge-back signal.
- **8:02–9:02 Fuse box rules.** Get the high box from a junkyard so you can chop it out with its T40, T26 and spare wire. "The GTI T40 is basically going to be blasted apart; you're going to move every pin." Make the Passat box exactly as it was in the Passat. Stays the same: headlights, impact sensors, fog lights, ambient temp sensor (A/C circuit), and the **GTI clutch position sensor on the T40** if you keep a manual. "All of your relay triggers on the T94 are going to have to be moved."
- **9:02–11:01 Cost in time and his best advice.** 200–300 hours over ~3 weeks: diagrams, cheat sheets, VCDS scans, continuity chasing, pin swaps. Use **factory VW ElsaWeb wiring diagrams** (about $50 for 24-hour access), VIN-specific for both cars, printed at the library. Mitchell/AllData/ProDemand had wrong pin numbers, wrong colours and missing info.
- **11:01** USP midpipe in, old cat-back cut to length. **Trunk breaker upgraded to an Eaton Bussmann (~$100): "no more Amazon breakers."** VCDS: six ECM faults down to four, three ABS/TCM related, one voltage (alternator not yet connected).
- **12:03–14:02 No starter signal.** Fuel pressure regulator, pumps, coils and injectors all have power, but the ECU does not see the clutch pressed. Cause: the GTI clutch switch feeds **T40 pin 14**, which is **unassigned on the Passat box**, so that circuit had no fuse. Continuity check, **fuse 39 (15 A) added**, and it starts.
- **14:02–16:02** It runs properly for the first time: "hundreds, if not over a thousand hours."
- **17:14–19:02 Final harness.** Everything routed through the cowl grommets to the ECU, unused clips and circuits removed, nylon wrap on every made cable, junkyard bare-aluminium A/C lines dressed in loom. All cooling hoses arrive from the dealer; only the swirl pot is outstanding.
- **19:02–21:01 Cooling plumbing.** The upper + lower radiator hose with the coolant temp sensor is **one expensive part number** (1K0 121 049 CM in the doc). Coolant bottle branch removed and capped with an Oetiker clip. A generic question-mark-shaped 5/8" hose from O'Reilly ($25). Heater core lower hose runs to the inline swirl pot. **Heater core upper is a factory Mk6 GTI hose**: cut off the stepped end and it fits the coolant flange, much cheaper than the Passat one. Crack-pipe nipple capped.
- **22:12** Filmed Saturday 8 March 2024. Off camera: aftermarket fenders replaced with OEM junkyard fenders resprayed ("OEM or bust"), badged grille with a 3D-printed VR6 badge. Alternator confirmed at 14.5 V.
- **26:05–28:04 First heat cycle.** Gray Fab swirl pot sits inline with the coolant hard line that bolts to the side of the head, Moroso pressure cap, distilled water first in case of leaks. Car on the ground for the first time since Thanksgiving, clutch bled. No leaks, **no check-engine light**, burps air with the heat on full.
- **29:10** First drive.

### Part 5: We did it (11:07)

- **1:01 Tune.** Done by Ian at **Reflect Tuning** (NC; he also takes mailed-in ECUs), who "has done a lot of refinement on 3.6 swaps." Result: codes eliminated, "fully functioning manual-swap 3.6 VR6 Mk6 GTI with zero lights on the dash." No mention of how the immobilizer was dealt with, here or anywhere in the series.
- **2:00 Mounts.** **Black Forest Industries** (Cary, NC) partnered on the build and supplied engine mounts: higher-durometer rubber, less wheel hop, sharper throttle response, "a huge improvement even over a brand-new OEM mount." Also a junk hood for now.
- **4:00** Last video for a while. Released on his 30th birthday (3 April 2024; "Ninety4" = born 1994). He had been **daily driving it for two weeks with the baby seat in the back**: "aside from a couple issues that tuning took care of, I have had zero problems." Filmed and edited entirely on an iPhone in iMovie; the swap was done on jack stands.
- **7:43** First wash in a year, blind-spot mirrors, hood strut borrowed from his wagon, and a drive.

### Part 5: We did it (11:07) **[pending transcript]**

Chapters: 1:14 tuning updates; 2:04 partnership and mounts; 3:58 project conclusion; 5:04 final test drive; 7:42 wash and final thoughts. Description links **Black Forest Industries** (mounts) and **Reflect Tuning** (tune). This is where the permanent mount solution and the ECU/tune situation are explained.

---

## 3. Why the swap works mechanically

1. **Transverse VR6 mounting points are a PQ35 standard.** The Mk5 R32, Eos 3.2 and Mk2 TT 3.2 all put a VR6 into this engine bay from the factory. The BLV uses the same engine-mount bracket geometry, so a PQ35 VR6 mount (1K0 199 262 AR) bolts straight on.
2. **The 02M is a PQ34/PQ35 crossover.** Its trans-mount pattern matches the PQ35 2.5L 5-speed/09G mount (1K0 199 555 AP) in the Mk4-sourced 2-bolt form, and the stock Mk6 dogbone, shift box, cables and manual axles all mate to it.
3. **The BLV's exhaust manifolds mimic the Mk5 R32's**, so R32 downpipes are the starting point, with massaging.
4. **The B6 Passat is the closest cousin.** His argument for the BLV over other 3.6 variants (B7/NMS Passat and CC CDVB, Touareg longitudinal units, Atlas): the B6 is PQ46, the sibling platform of PQ35, so the ECU generation, fuse box family and harness style are nearest to the Mk5/6. (Earlier in our chat I suggested a 2012–2018 NMS Passat donor. That is a CDVB 3.6 in a different body (we first called it CDVB; that is the Atlas code); the engine is still transverse, but the harness, ECU and accessories need to be checked against Choby's BLV findings before assuming the same parts.)
5. **Everything that did not bolt on was small**: one A/C line, downpipe massaging, bay bracket trimming for appearance, and wiring.

## 4. What actually had to change (the wiring)

Mechanically it is bolt-on. Electrically it is a re-pin job on the recipient's body harness plus a fuse box swap. The engine side is untouched: a new BLV engine harness plugs into the BLV ECU's **T60** and into the engine, done. Everything below happens on the ECU's **T94** (body side), the **T14** bridge, and the fuse box's **T40/T26**. From the sheet (`sources/ninety4co-swap-wiring-repins.md`) and Part 4:

- **Fuse box:** the GTI's E-box has no **T26** connector; the BLV needs the Passat/VR6 "high" box, **1K0 937 124 K**, taken from a junkyard car with its cabling and connectors intact.
- **Power distribution:** terminal 30, terminal 15, connection 87 and two ECM relays move pins; the **coolant after-run pump and its relay** are new circuits.
- **Sensors moved:** coolant temp, fan module, EVAP leak detection pump (two pins), brake light switch, cruise (unverified by him as of mid-2024).
- **Fuel:** fuel pump module control and low-pressure fuel sensor move; a fuel-pressure-regulator circuit is added.
- **Removed and re-added:** all GTI O2 wires out, 3.6 bank 1/bank 2 sensors pinned fresh; TSI MAF out, 3.6 MAF in on four new pins; all six throttle pedal pins move.

- **Manual-specific gotcha:** the recipient's clutch position switch lands on T40 pin 14, which is unassigned in the Passat box (the B6 3.6 was automatic-only in North America). Add a fuse for it (his: fuse 39, 15 A) or there is no starter signal.
- **Diagnostic story:** the car ran on the GTI box but a relay chattered and stuck even key-out, and the brake lights were stuck on. The first was the undersized GTI box back-feeding relays; the second was the brake switch pins on the T94.

His process: ~200–300 hours over three weeks, factory ElsaWeb diagrams for both VINs printed and laid out, a cheat sheet built pin by pin, VCDS scans and continuity checks between swaps. He did it with factory wiring diagrams for both cars and still marks the sheet "use at your own risk."

## 5. What went wrong, and the lesson in each

| Problem | Where | Lesson |
|---|---|---|
| Original engine harness had broken connectors | P2 1:01 | Price a new OEM harness before repairing a junkyard one; his was cheap at the dealer |
| Wrong input shaft/axle seals ordered | P2 7:41 | Confirm the 02M variant (Mk4 vs Mk5/TT) before ordering seals and mounts |
| TSI A/C suction line does not fit | P3 19:00 | Budget the PQ35 VR6 line (1K0 820 743 CE) from day one |
| R32 downpipes fit poorly, shifter cables in the way | P3 21:00 | Expect fabrication at the downpipe/midpipe joint and cable routing |
| Starter clicks, circuit breaker trips | P3 27:00 | Starter inrush through a trunk-battery breaker and long cable; size the breaker and cable for cranking, or feed the starter unfused |
| Weeping fuel fitting at prime | P3 25:00 | Torque every fuel fitting before first key-on |
| Relay chattering and sticking, even key-out | P4 6:01 | The GTI fuse box cannot carry the 3.6's circuits; fit the Passat high box from the start instead of discovering it |
| All brake lights stuck on after first start | P4 7:00 | Brake light switch runs through the ECU's T94; move its pins |
| No starter signal, clutch not recognised | P4 12:03 | Clutch switch circuit lands on an unassigned Passat pin; add fuse 39 (15 A) |
| Cheap trunk-battery breaker | P4 11:01 | He replaced it with an Eaton Bussmann unit; cranking current needs a real breaker |
| Voltage fault in VCDS | P4 12:03 | Alternator not connected yet; connect and verify charge-back before chasing codes |
| Months of delay | P3 3:55 | Life. The build took ~7 months of calendar time for ~weeks of work |
| **Spun rod bearing 4 months after first drive** | follow-up videos, Aug 2024 | See section 6 |

## 6. What happened after the series

Same car, same channel, in order:

| Date | Video | Why it matters |
|---|---|---|
| 2024-04-26 | [How Much Did My Manual 3.6L VR6 MK6 Swap Cost?](https://youtu.be/7LxC1nn25Yg) (20:48) | Full cost breakdown by category, parts sold, net cost. Worth pulling next. |
| 2024-06-21 | [EVERYTHING DONE TO MY 3.6L VR6 MK6!](https://youtu.be/SZKrv8SIRkI) (17:56) | Has an "Engine Issues" chapter at 10:21, two months after completion |
| 2024-08-06 | [I BROKE MY 3.6 VR6 MK6 GTI](https://youtu.be/WeMtltphD1o) (10:25) | Engine noise while fixing minor issues |
| 2024-08-09 | [I FOUND WHAT'S WRONG (It's not good)](https://youtu.be/JBCkB3V5hrw) (9:49) | **Spun rod bearing** confirmed; rebuild options weighed |
| 2024-08-15 | [SLAPPING ROD BEARINGS IN MY 3.6](https://youtu.be/2nl2_9P_jUQ) (17:27) | Budget in-car fix: polish the journal, new bearings |
| 2024-08-29 | [FINISHING OUR MK6 3.6 VR6 ROD BEARINGS](https://youtu.be/7uPvX-1Qw2U) (9:54) | Start-up and oil flushes; did it survive |
| late 2024–2025 | "Ultimate MK6 Street Car" PT.1–3, AWD transmission and rear end, "World's first manual AWD 3.6 MK6", first drive | He converts the car to **manual AWD** (02M 4Motion path) |
| 2025-05-30 | [What Does it Cost to Build a Manual AWD 3.6L VR6 MK6 GTI?](https://youtu.be/slvrr_6RqNs) (16:00) | Cost of the AWD phase |
| 2025 | Cams, long-tube header, custom exhaust, "Fixing everything broken", "Time to sell the 3.6?" | Ongoing |

The bearing failure is the most important fact in the whole channel for us. In Parts 1–2 he rebuilt the top end and timing of a 171,000-mile engine but **left the rotating assembly alone** (no rod bearings, no main bearings on camera). Four months after the first drive a rod bearing spun. Whether the cause was worn bearings, oil starvation, or something else is in the August 2024 videos, which we have not watched yet. Either way: **rod bearings while the engine is on the stand** goes on our list, and we should hear his diagnosis before buying an engine.

## 7. What transfers to a Mk6 Jetta, and what does not

His car is a Mk6 **Golf** GTI (PQ35). Ours is a Mk6 **Jetta** (2011–2018, NCS/A6), which is PQ35-derived but longer, with its own front-end sheet metal, cooling pack, electrical architecture and fuel tank. This is the bridge to the parts research. Confidence: **Yes** = chassis-independent, **Likely** = same platform family, verify part number, **Verify** = known to differ between Golf and Jetta, must be researched.

| Item from his list | Transfers? | Notes |
|---|---|---|
| BLV engine, rebuild scope, timing, oil pump sprocket, oil filter stand, two-piece manifold | **Yes** | Engine-side only |
| 02M 6-speed + South Bend clutch + steel forks | **Yes** (gearbox side) | Chassis side below |
| Engine mount 1K0 199 262 AR, trans mount 1K0 199 555 AP, dogbone | **Likely** | Mk6 Jetta front mounts are 1K0-family PQ35 parts; confirm the Jetta 2.5L/GLI mount numbers and bracket geometry match |
| Stock Mk6 manual axles | **Verify** | Jetta axles are Jetta-specific part numbers; confirm length/spline match for an 02M in a Jetta (GLI 02Q axles are the likely answer) |
| Stock Mk6 shift box and cables | **Verify** | Works if the Jetta has an 02Q (GLI manual). A 2.5L 5-speed (0A4) uses different cables and tower |
| Fuse box 1K0 937 124 K + GTI body harness re-pins | **Verify** | The concept transfers (the Jetta also never had a VR6, so it also lacks the VR6 circuits). The pin numbers do not: the Jetta's body harness, BCM and gateway differ from the GTI |
| Stock Mk6 fans, condenser, high-pressure A/C line | **Yes, as "use the Jetta's own"** | Check the Jetta fan shroud fits whatever radiator is chosen |
| A/C suction line 1K0 820 743 CE | **Verify** | Golf geometry; Jetta Mk6 A/C lines are Jetta-specific |
| Mishimoto Mk5 R32 radiator + Passat GT hoses + swirl pot | **Verify** | Jetta Mk6 radiator and lock carrier differ from the Golf's; the radiator may not drop in |
| Passat 3.6 fuel pump module 3C0 906 093 A, 4-bar regulator | **Verify** | Jetta tank is not the Golf tank; confirm the flange/sender fits, or whether a Jetta module with a 4-bar regulator does the job |
| USP R32 downpipes | **Likely with fabrication** | Engine-side fit is the same; the Jetta's longer wheelbase means a Jetta-length midpipe/cat-back |
| Battery relocation | **Not needed** | The R32/Eos keep the battery in the bay; his relocation was a show-car mod. "Tight side to side" may be tighter with a battery in place |
| Immobilizer / ECU coding | **Not shown** | The Passat ECU ran the GTI from the first start, but how the immobilizer was handled is never explained on camera. Reflect Tuning later cleared the remaining codes (ABS/TCM-related). Top research item |
| Heater core upper hose: factory Mk6 GTI hose, end trimmed | **Verify** | Jetta heater hoses are Jetta-specific; the same trick may work with the Jetta's own hose |
| DSG path | **Not covered** | His build is manual. Our earlier GLI-DSG + Passat-DSG idea has no precedent in this series |

## 8. How this changes our plan

- The series proves the **manual 02M route** is bolt-on mechanically and cheap on the gearbox side ($400 box, ~$1,000 clutch). Our earlier plan was a DSG GLI plus a wrecked Passat's DSG. Both are viable; the manual route has a documented parts list, the DSG route does not (yet).
- **Engine choice:** he argues BLV (2006–2010 B6 Passat). Our earlier donor idea was a 2012–2018 NMS Passat (CDVB). Decide this before anything else; it changes the ECU, harness and fuse box research.
- **Add to the rebuild scope:** rod and main bearings, oil pump pickup inspection, and the updated oil pump sprocket and bolt. His bearing failure is the cautionary tale.
- **Wiring is the real work.** Plan on factory wiring diagrams for both the Jetta and the donor, a junkyard VR6 "high" fuse box with its harness tail, and a weekend per circuit group.
- **Budget the small fit items up front:** A/C suction line, downpipe fabrication, mounts, fuel module, seals.

## 9. Open questions the series does not answer

1. **Immobilizer.** The Passat ECU runs with the GTI's cluster and keys from the first start, and he never says how. Options are an immobilizer delete in the ECU file, or adapting the ECU to the GTI's immobilizer with VCDS/ODIS. Ask him (Instagram @chobester) or Reflect Tuning before buying an ECU.
2. **The one T14→T94 jumper** he could not remember (P4 5:03). The wiring sheet's T14/3 → T26/11 (coolant recirc pump) and T14/7 → T94/35 (low fuel pressure sensor) lines are the candidates.
3. **Cruise control** is still marked unverified on his sheet.
4. **What the three ABS/TCM faults were** and whether the tune suppressed them or fixed them.
5. **Final cost by category** (cost video, 26 Apr 2024) and **what caused the rod bearing failure** (Aug 2024 videos). Both are next to pull.

## Appendix: method and limits

- Transcripts are YouTube auto-captions, pulled with yt-dlp; expect misheard words ("BR6" = VR6, "Pat" = Passat, "Mark V" = Mk4, "Atlas oil pump" is probably "updated oil pump"). Timestamps are accurate to the minute.
- Captions were fetched with yt-dlp's `web_embedded` player client and the `en-orig` track; the plain `en` track yt-dlp lists first for these videos is an auto-translation and should not be used.
- Part numbers come from his doc, not from VW's catalogue, and have not yet been verified for our car. That is the next task.

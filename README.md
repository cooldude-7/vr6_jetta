# VR6 Jetta

Build plan: put a 3.6L VR6 and DSG from a wrecked Passat V6 into a Mk6 Jetta GLI.

All prices are rough estimates in CAD for a DIY build. They are not quotes. Check
Kijiji, AutoTrader and salvage auctions (Copart, IAA) for local prices before buying.

## The plan

1. **Base car: Mk6 Jetta GLI with DSG (2012–2018).** It already has the DSG shifter,
   PRNDS dash coding, the gear readout and the right pedal box. It also has the
   multilink rear suspension and bigger brakes, which you want with a VR6.
2. **Donor engine: a 3.6 VR6 from a wrecked Passat.** Two candidates, compared in
   `reports/Mk6 Jetta CDVC VR6 swap parts.md`:
   - **BLV** (2006–2010 B6 Passat, Bosch MED9): the engine Ninety4co used; the only one
     with off-the-shelf manual swap tunes. **Current recommendation.**
   - **CDVB** (2012–2018 NMS Passat, Bosch MED17; we first mislabelled it "CDVC", which is
     the Atlas code): newer, same electrical generation as the Mk6 Jetta, but DSG-only from
     the factory and no tuner yet sells a manual swap file for it. Flip to it only with a
     written tuner quote in hand, or if the car stays DSG.
   Buy the whole donor car, not parts: engine, gearbox, ECU, harness, fuse box, keys and
   cluster all matched.
3. **Drive the GLI stock first.** Do the swap later, when you have the money, space
   and time. The car will be off the road for weeks to months.

A non-DSG Jetta (manual or Aisin automatic) works too, but you would also have to
convert the shifter, pedals and part of the coding.

## Research

- `research/ninety4co-vr6-mk6-swap-series.md`: deep analysis of Ninety4co's five-part
  *VR6 MK6 Swap* series (3.6 BLV + manual 02M into a Mk6 GTI), what broke afterwards,
  and what transfers to a Mk6 Jetta.
- `research/sources/`: his swap parts list (with VW part numbers) and wiring re-pin sheet.
- `research/transcripts/`: timestamped transcripts of the episodes.
- `reports/Mk6 Jetta CDVC VR6 swap parts.md`: the parts-compatibility report for a 3.6 VR6 +
  Mk4 24V 02M into a 2015–2018 GLI, with part numbers, sources, a BLV-vs-CDVB engine
  decision and a staged shopping/verification list. Raw notes in `research_notes/`.
- `reports/Audi A3 8V VR6 swap parts.md`: the same study for a 2015–2020 Audi A3 8V (MQB)
  with an Atlas 3.6. Verdict: no precedent, no OEM parts set, custom AWD driveline and an
  ECU calibration nobody sells; ~CA$30,000–56,000 net for a car slower than a stock S3.
  Build the Jetta, or buy an S3 if AWD matters more than the VR6. Partly superseded by:
- `reports/Audi A3 8V VR6 with stock gearbox.md`: follow-up after finding real 8V VR6 builds
  (TuneZilla's S3, Malaka's RS3). Stock-power plan: Atlas 3.6 + its own ECU on the A3 quattro's
  own 6-speed DSG via a 4WD VR6 DSG bellhousing (likely, unproven), ~CA$10,100–24,000 net
  excluding the car. Cost list in `research/a3-stock-power-vr6-cost-estimate.md`.

## Problems to solve

- [ ] **Immobilizer.** The Passat engine computer is paired to the Passat keys.
      Disable it with a tune, or adapt it to the Jetta.
- [ ] **CAN bus and coding.** Code the Jetta's gateway, ABS, steering and dash for the
      new engine with VCDS or OBDeleven. Expect trial and error.
- [ ] **DSG.** Keep the gearbox and engine computer from the same donor. The DSG's
      control unit expects that engine.
- [ ] **Tune.** Pick a tuner who supports the 3.6 before you start. The tune handles
      the immobilizer delete, fan settings and fault cleanup.
- [ ] **Mounts and axles.** The Mk5 R32 (same platform family) came with a transverse
      VR6 and DSG, so R32 parts and swap write-ups are a good starting point.
- [ ] **Exhaust.** Adapt the Passat manifolds and downpipes to the Jetta's underbody.
- [ ] **Insurance.** Tell your insurer about the swap before the car goes back on the road.

## Cost estimate (CAD)

Updated 2026-10-08 from Ninety4co's cost video (his receipts, USD, 2023–24) and the parts
report. Exchange assumed ≈ 1.37; HST and shipping on US-sourced parts added at ~15–20%.
Plan: manual 2015–2018 GLI + BLV + Mk4 24V 02M, DIY labour.

### Ninety4co's actual numbers (USD)

| Item | Cost |
| --- | ---: |
| Junkyard BLV (171k mi) with harness, ECU, alternator, A/C compressor | 300 |
| Mk4 24V 02M with steel forks | 440 |
| Rebuild parts: FCP Euro, UroTuning (incl. South Bend clutch), dealer (incl. hoses) | ~5,400 |
| Head machining 350, Gray Fab swirl pot 300, Schimmel parts 475, exhaust 520, misc ~970 | ~2,600 |
| Non-swap items in his total (bay paint, fenders, battery relocation, trunk, lights) | ~1,570 |
| **Raw receipts** | **10,262** |
| Parts sold (2.0T engine + 02Q + clutch 3,000, K04 650, intakes, cage, hood, …) | −6,095 |
| **Out of pocket** | **4,127** |

Not in his total: USP downpipes (traded, ~800), BFI mounts (sponsored, ~330–670), the tune
(never priced), and wholesale discounts. Swap-only at retail ≈ 10,000 USD.

### Our build

| Item | Low | High |
| --- | ---: | ---: |
| 2015–2018 GLI, manual | 13,000 | 20,000 |
| Donor: B6 BLV (scarce) or NMS CDVB (1,700–2,500 salvage) | 1,500 | 4,000 |
| Rebuild + chassis + cooling + A/C + exhaust parts (his ~10k USD retail) | 11,000 | 14,000 |
| Added scope: rod/main bearings, custom A/C discharge line, custom midpipe, Jetta radiator | 1,200 | 2,500 |
| Tune + immo-off + erWin diagrams + VCDS | 1,200 | 2,500 |
| HST / shipping / duty on US parts | 1,800 | 3,000 |
| **Swap subtotal** | **~15,000** | **~22,000** |
| Optional Wavetrac LSD | +1,600 | +1,800 |
| **All-in before resale** | **~30,000** | **~46,000** |
| Resale: GLI 2.0T + 02Q + accessories, donor leftovers | −4,000 | −6,500 |
| **Net, DIY** | **~25,000** | **~40,000** |
| Shop labour instead of DIY | +10,000 | +15,000 |

The engine and gearbox are the cheap part (~1,000 together). The rebuild parts, the newer
GLI, and the software and paperwork are the cost. Tell the insurer before the first drive.

### Lean build: target CA$5,000–6,000 (excluding the car)

Updated 2026-10-08. The table above prices a full Ninety4co-level rebuild at retail plus a bought
tune. Built lean (whole junkyard engine with its harness/ECU/fuse box, rebuild only what can't be
reached later, self-tuned with tools already owned), the swap lands near the target:

| Item (manual GLI + BLV + Mk4 24V 02M) | Low | High |
| --- | ---: | ---: |
| Junkyard BLV with harness, ECU, alternator, A/C compressor, intake, cats | 500 | 2,000 |
| Junkyard B6 "high" fuse box (1K0 937 124 K) with harness tail, EVAP bits, A/C suction line | 100 | 400 |
| Used Mk4 24V 02M with starter | 550 | 1,400 |
| Timing set, one-piece oil-pump sprocket + bolt, water pump, thermostat, gaskets, seals | 700 | 1,500 |
| Rod and main bearings | 150 | 400 |
| South Bend K70287 Stage 2 Daily clutch + single-mass flywheel (VR6 10-bolt) | 950 | 1,100 |
| Slave cylinder (0A5 141 671 E/F), seals, gear oil | 150 | 300 |
| Mounts 1K0 199 262 AR + 1K0 199 555 AP | 450 | 600 |
| Radiator 5K0 121 251 H (CSF 3777) | 250 | 350 |
| Cooling hoses + coolant; bottle OEM or Gray Fab | 300 | 1,300 |
| Custom A/C discharge line + recharge | 200 | 500 |
| Fuel filter/regulator 6Q0 201 051 J (J538 usually comes with the engine) | 50 | 300 |
| Exhaust: junkyard R32/Eos downpipes + local mid-pipe, up to the USP kit | 300 | 1,200 |
| erWin diagrams (both VINs) + pins, terminals, loom | 150 | 400 |
| Tune (self) | 0 | 0 |
| Fluids, hardware, misc | 300 | 600 |
| **Gross** | **~5,100** | **~12,400** |
| Sell the GLI's 2.0T engine + 02Q | −2,500 | −4,500 |
| **Net, excluding the car** | **~2,600** | **~7,900** |

To stay at CA$5–6k: buy the engine whole with its harness, ECU and fuse box attached (Ninety4co's
was US$300 at a U-Pull); rebuild only the timing, bearings, water pump and gaskets; skip cosmetic
work; sell the GLI's 2.0T and 02Q as a running pair. The clutch is the one part that must be
aftermarket (a stock 24V clutch won't hold the 3.6).

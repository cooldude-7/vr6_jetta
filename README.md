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

### Cars

| Item | Low | High |
| --- | ---: | ---: |
| Mk6 GLI with DSG | 8,000 | 15,000 |
| Wrecked FWD Passat V6 donor | 2,000 | 5,000 |

2012–2014 GLIs sit at the low end, 2015–2018 at the high end.

### Swap

| Item | Low | High |
| --- | ---: | ---: |
| Timing chains, gaskets, water pump, plugs (before install) | 1,000 | 2,000 |
| Mounts, axles, adapter parts | 800 | 2,000 |
| Exhaust adaptation | 500 | 1,500 |
| Tune with immobilizer delete | 800 | 2,000 |
| Coding tool (OBDeleven or VCDS) | 150 | 600 |
| Fluids, DSG service, small parts | 500 | 1,000 |
| **Swap subtotal** | **~4,000** | **~9,000** |

### Totals

| | Low | High |
| --- | ---: | ---: |
| All-in (both cars + swap) | 12,000 | 25,000 |
| Resale of leftovers (GLI 2.0T, unused Passat parts) | −2,000 | −5,000 |
| **Net, DIY** | **~10,000** | **~20,000** |
| Extra if a shop does the labour | +6,000 | +12,000 |

# 2013 Audi A3 (8P) + 3.6 VR6 BLV + Mk4 24V 02M: plan, parts and lean budget

Plan dated 2026-10-08. Recipient: a **2013 Audi A3 2.0T front-drive with the 6-speed manual** (the 8P Sportback hatch). Engine: **BLV 3.6 VR6** from a 2006–2010 B6 Passat, self-tuned (Bosch MED9.1.1). Gearbox: **Mk4 24V VR6 02M** 6-speed manual. This is Ninety4co's documented Mk6 GTI recipe (`research/sources/`) on the same platform.

## Why the 8P works

- **It's a Golf underneath.** The 8P A3 is PQ35, the same platform as the Mk5/Mk6 Golf/GTI that Ninety4co swapped, and Golf length (2,578 mm wheelbase), so his radiator, axle, exhaust and A/C choices apply more directly than to a Mk6 Jetta.
- **Audi built a VR6 version.** The 2006–2009 A3 3.2 quattro (250 hp, S tronic only) means a VR6 engine mount, A/C line and downpipes already exist as A3 fitments. USP's R32 downpipes are listed for the "Mk5 R32 and A3 3.2L"; the 1K0 199 262 AR VR6 mount is sold for "A3 TT Eos Passat R32".
- **The 2013 front-drive 2.0T has a 6-speed manual.** Standard in Canada for 2013; quattro and TDI were S tronic only ([AutoTrader.ca 2013 A3](https://heavytruck.autotrader.ca/research/audi/a3/2013), [Cars.com](https://www.cars.com/research/audi-a3-2013/), [TrueDelta](https://www.truedelta.com/Audi-A3/specs-8-2013)). Read the build sheet; a VIN decoder confirms manual cars exist ([decodethis](https://decodethis.com/web/vin/WAUFFAFM2CA015703)).
- **Same engine and electrics family as Ninety4co's GTI.** The North American 2009–2013 A3 2.0T uses the same EA888 Gen1 2.0T family as his 2010 GTI (CCTA), and the BLV's MED9 era matches the 8P's electrical generation.

## Watch-outs

- **Manual 2013s are rare.** Five 2013 A3s on Kijiji Ontario (2026-10-08) asked CA$5,000–9,800; none said manual ([Kijiji](https://www.kijiji.ca/b-cars-trucks/ontario/audi-a3-2013/k0c174l9004)). Widen to Quebec or the northern US, or accept a 2009–2012 manual (the same car).
- **Headroom at 6'6".** No 8P headroom figure was found. Many have the large "Open Sky" sunroof. Sit in one before buying.
- **Rust and age.** It's 13 years old in Ontario salt; check rockers, rear arches, subframe.
- **Body wiring is Audi, not VW.** Ninety4co's pin sheet is for a 2010 GTI body harness. Same platform and generation, but every pin must be re-checked against erWin diagrams for the A3's VIN and the donor Passat's VIN.
- **Battery.** Ninety4co's battery was already in the trunk and he called the fit "tight side to side". Budget a trunk relocation in case the BLV's airbox and battery don't fit together.
- **If no manual car turns up:** an S tronic A3 is not a dead end, but it's a different project (VR6 DSG or a pedal-box conversion). Don't buy an S tronic car for this plan.

## Parts list

Part numbers are from Ninety4co's list and the Jetta research; labels as in `reports/Mk6 Jetta CDVC VR6 swap parts.md`. Verify each against the A3's VIN at a dealer counter before ordering.

| Area | Part | Number / source | Note |
|---|---|---|---|
| Engine | BLV 3.6 VR6 with ECU, engine harness, intake, MAF, fuel/EVAP lines, sensors, alternator, A/C compressor | B6 Passat 3.6 (2006–2010), whole from a U-Pull/wrecker | Take the B6 "high" fuse box with harness tail and the body-side ECU connector too |
| Engine rebuild | Timing chains, tensioners, guides; one-piece oil-pump sprocket + 12.9 bolt; water pump; thermostat; gaskets; seals; **rod and main bearings** | OEM-supplier timing kit (e.g. ES2784782), dealer bolts | Timing is on the gearbox side: now or never. His spun a rod bearing |
| Gearbox | Mk4 24V VR6 02M 6-speed (2002.5–2005 GTI/GLI 24V), steel shift forks | used | Check 2-bolt vs 3-bolt mount bosses |
| Clutch | South Bend K70287 Stage 2 Daily, single-mass flywheel, **VR6 10-bolt** | UroTuning ~US$684 | Stock 24V clutch won't hold the 3.6 |
| Slave | Concentric slave 0A5 141 671 E/F | | Same family as the A3's 02Q |
| Starter | Mk4 02M starter (Valeo 438152) | junkyard | |
| Engine mount | 1K0 199 262 AR (PQ35 VR6) | FEBI ~US$145 | Listed for A3 3.2 |
| Trans mount | 1K0 199 555 AP (2-bolt 02M) or 1K0 199 555 Q (3-bolt) | | Shared PQ35 console |
| Dogbone, axles, shift box/cables | The A3's own (manual car) | | Ninety4co reused his GTI's with the 02M |
| Fuse box | B6 Passat "high" box 1K0 937 124 K with harness tail | junkyard | Adds the T26 connector the 3.6 needs |
| Fuel | J538 3C0 906 093 A (usually with the engine); 4.0-bar filter/regulator 6Q0 201 051 J | | |
| Cooling | R32/A3 3.2-size radiator (Mishimoto MMRAD-Mk5-08 or OEM-style); hoses 1K0 121 049 CM, 1K0 122 086 B, 1K0 122 157 HE, 3C0 121 063 E; after-run pump 1K0 965 561 B; Gray Fab bottle optional | | Hose numbers are REPORTED only; confirm by VIN |
| A/C | Suction line 1K0 820 743 CE (PQ35 VR6); compressor 1K0 820 808 F or the donor's; discharge line likely custom | | |
| Exhaust | USP-32L-CAT1 (Mk5 R32 / A3 3.2 downpipes) or junkyard R32/A3 3.2 downpipes; local mid-pipe to the A3 cat-back | ~US$800 new | |
| Electrical | erWin wiring diagrams for both VINs | ~US$35/day each | |
| Tune | Self, MED9.1.1 (immo off, manual, deleted 2.0T sensors) | | |

## Lean budget (CAD, excluding the car)

| Item | Low | High |
|---|---:|---:|
| Junkyard BLV, whole, with harness, ECU, alternator, compressor, intake, cats | 500 | 2,000 |
| B6 "high" fuse box with harness tail, EVAP bits, A/C suction line | 100 | 400 |
| Used Mk4 24V 02M with starter | 550 | 1,400 |
| Timing set, oil-pump sprocket + bolt, water pump, thermostat, gaskets, seals | 700 | 1,500 |
| Rod and main bearings | 150 | 400 |
| South Bend clutch + single-mass flywheel | 950 | 1,100 |
| Slave cylinder, seals, gear oil | 150 | 300 |
| Mounts 1K0 199 262 AR + 1K0 199 555 AP | 450 | 600 |
| Radiator (R32/A3 3.2 size) | 300 | 550 |
| Cooling hoses + coolant; bottle OEM or Gray Fab | 300 | 1,300 |
| Custom A/C discharge line + recharge | 200 | 500 |
| Fuel filter/regulator (J538 usually comes with the engine) | 50 | 300 |
| Exhaust: junkyard downpipes + local mid-pipe, up to the USP kit | 300 | 1,200 |
| erWin diagrams + pins, terminals, loom | 150 | 400 |
| Battery relocation, if needed | 0 | 800 |
| Tune (self) | 0 | 0 |
| Fluids, hardware, misc | 300 | 600 |
| **Gross** | **~5,150** | **~13,350** |
| Sell the A3's 2.0T + 02Q | −1,500 | −3,500 |
| **Net, excluding the car** | **~3,650** | **~9,850** |

The car: 2013 A3s asked CA$5,000–9,800 in Ontario (none confirmed manual). **All-in, car included: roughly CA$8,650–19,650**, against CA$15,600–27,900 for the Mk6 GLI version (CA$13,000–20,000 car + CA$2,600–7,900 net swap).

## First steps

1. Find a manual 2013 (or 2009–2012) A3 2.0T FWD; sit in it with the seat down; check rust.
2. Find a B6 Passat 3.6 at a U-Pull or as a Kijiji parts car; buy the engine whole with harness, ECU, fuse box and the body-side ECU connector.
3. Buy erWin for both VINs before pulling anything; map Ninety4co's pin sheet onto the A3's harness.
4. Line up a 24V 02M (Marketplace) and the South Bend clutch.

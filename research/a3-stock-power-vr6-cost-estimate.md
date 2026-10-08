# A3 8V stock-power VR6 swap: cost list, excluding the car

Build: 2015–2020 Audi A3 2.0T quattro with its own 6-speed DSG (0D9 / DQ250), keeping its transfer case, prop shaft, Haldex rear, axles, trans mount and dogbone. Engine: VW Atlas 3.6 VR6 (CDVC) with its own Bosch MED17.1.62 ECU, self-tuned. Stock VR6 power (276 hp / 266 lb-ft).

Estimate dated 2026-10-08, CAD. Conversions: USD × 1.37, EUR × 1.55, GBP × 1.80. Sources are the research notes in `research_notes/Audi A3 8V VR6 swap parts/` and `research_notes/Audi A3 8V VR6 with stock gearbox/`. Lines marked *estimate* have no quote behind them.

| # | Item | Low | High | Basis |
|---|---|---:|---:|---|
| 1 | Donor: wrecked 2018–2021 Atlas 3.6 (front undamaged) via a Copart.ca broker, incl. fees, HST, tow. Gives engine, ECU, harness, engine mount, A/C compressor, cats, sensors | 6,500 | 15,000 | Copart Canada Atlas 3.6 sales CA$5,200–13,700 + ~CA$1,000–2,000 fees |
| 2 | Engine refresh before install: timing chains/tensioners/guides (trans-side, now or never), water pump, thermostat housing, PCV, gaskets, seals, intake-valve cleaning | 2,000 | 4,500 | FCP Atlas timing kits US$397–1,056, pump US$213 |
| 3 | Gearbox: VR6 DSG front case / bellhousing 02E 301 107 (from an R32, A3 3.2, TT 3.2 or CC/Passat 3.6 DSG), VR6 DSG dual-mass flywheel, seals, DSG fluid and filter; full split and re-shim of the A3's 0D9 (DIY or a DSG shop) | 1,200 | 3,500 | Front case €140–210 used; flywheel and shop time *estimate*. **Unproven fit**: no source confirms the 0D9 internals drop into a VR6 02E front case |
| 4 | DSG (TCU) tune to lift the 350 Nm clamp and fix shift points | 550 | 1,300 | TuneZilla / APR / IE / HPA MQB DQ250 tunes US$399–965 |
| 5 | Your ECU tuning tools for a Tricore MED17.1.62: bench/boot read-write tool + WinOLS. Skip if you already own them | 2,000 | 8,000 | KESS3 £540 + protocol activations, bFlash £2,499+, WinOLS €1,034. Cheaper fallback: an immo-off service US$135–350 |
| 6 | Diagnostic/coding tool (OBDeleven or VCDS) for gateway list, basic settings | 150 | 600 | |
| 7 | Engine mount: Atlas 3QF 199 262 G/H + block console 022 199 354 T (reuse the donor's, or new) | 0 | 700 | TuneZilla proved the Atlas mount bolts to the 8V rail |
| 8 | Cooling: S3-pattern radiator stack, expansion tank or Gray Fab bottle, custom/adapted hoses | 1,100 | 2,500 | Radiators US$162–699, aux US$125–230, bottle US$280 |
| 9 | A/C: custom compressor hoses, evacuate and recharge | 400 | 900 | *estimate* |
| 10 | Exhaust: custom Y/mid-pipe from the Atlas cats into the A3/S3 cat-back, keep all four O2 sensors | 1,000 | 2,500 | *estimate*; Ninety4co paid US$300 for exhaust welding |
| 11 | Fuel: fittings/adapters (the A3 quattro pump and controller feed a stock 3.6) | 100 | 300 | |
| 12 | Intake: airbox/MAF housing adaptation | 200 | 600 | *estimate* |
| 13 | Battery relocation to the trunk (cable, breaker, box, battery) | 400 | 800 | Ninety4co: US$250 supplies + US$300 battery |
| 14 | Wiring: erWin diagrams for both VINs, pins, terminals, wire, loom | 300 | 600 | erWin ~US$35/day per brand |
| 15 | Front springs rated for the heavier VR6 nose | 300 | 1,000 | *estimate* |
| 16 | Fluids, hardware, gaskets, consumables | 500 | 1,000 | *estimate* |
| 17 | HST, shipping, duty on US/EU parts | 800 | 2,000 | ~15–20% |
| | **Gross, excluding the A3** | **~17,500** | **~45,800** | |
| | Sell the A3's 2.0T engine + Simos ECU + intercooler, and the Atlas leftovers (8-speed, transfer case, parts) | −4,000 | −10,000 | *estimate*; Ninety4co sold his 2.0T + gearbox for US$3,000 |
| | **Net, excluding the A3** | **~13,500** | **~35,800** | |

## What moves the number

- **Already own tuning tools:** subtract up to CA$8,000 (line 5).
- **Cheap donor:** a front-undamaged Atlas near CA$6,500 is the biggest single saving (line 1).
- **If the VR6 front case does not fit the 0D9** (line 3 is unproven), the fallback is the documented DQ500 route: used RS3/TT RS DQ500 + VR6 bell machining and adapter (€550–950) + VR6 DQ500 flywheel (€550–1,600) + transfer-case bracket (£190). That replaces line 3 and adds roughly **CA$4,000–7,000**. HPA's complete VR6 DQ500 kit is US$11,699 (~CA$16,000).
- **Not included:** the A3 itself (Ontario 2.0T quattro asks CA$10,500–20,000), insurance, shop labour, and anything for power above stock.

For comparison, the Mk6 Jetta GLI plan (BLV + Mk4 02M) is roughly CA$8,500–18,000 net excluding the car, from `README.md`.

# A3 8V stock-power VR6 swap: cost list, excluding the car

Build: 2015–2020 Audi A3 2.0T quattro with its own 6-speed DSG (0D9 / DQ250), keeping its transfer case, prop shaft, Haldex rear, axles, trans mount and dogbone. Engine: a loose VW Atlas 3.6 VR6 (CDVC) plus its Bosch MED17.1.62 ECU (no donor car). The builder already owns tuning tools and tunes both the ECU and the DSG himself. Stock VR6 power (276 hp / 266 lb-ft).

Estimate updated 2026-10-08, CAD. Conversions: USD × 1.37, EUR × 1.55, GBP × 1.80. Sources are the research notes in `research_notes/Audi A3 8V VR6 swap parts/` and `research_notes/Audi A3 8V VR6 with stock gearbox/`. Lines marked *estimate* have no quote behind them.

| # | Item | Low | High | Basis |
|---|---|---:|---:|---|
| 1 | Loose Atlas 3.6 complete engine from a recycler, plus shipping to Ontario, duty and HST | 3,000 | 4,500 | Transend recycled 2018 Atlas 3.6 complete assembly, 103k mi, US$1,787–1,994 ([listing](https://transend.us/products/engine/cylinder-block-components/engine-complete-assembly/engines100179265)); PartRequest lists 54k–112k mi units, unpriced ([catalog](https://www.partrequest.com/catalog/complete-engines/volkswagen/volkswagen-atlas)) |
| 2 | What a loose engine may not include: Atlas ECU (03H 906 026 xx), engine harness, MAF/airbox, throttle body, O2 sensors, manifolds/cats, A/C compressor | 800 | 2,500 | *estimate*; ask the recycler exactly what is on the engine |
| 3 | Engine refresh before install: timing chains/tensioners/guides (trans-side, now or never), water pump, thermostat housing, PCV, gaskets, seals, intake-valve cleaning | 2,000 | 4,500 | FCP Atlas timing kits US$397–1,056, pump US$213 |
| 4 | Gearbox: VR6 DSG front case / bellhousing 02E 301 107 (from an R32, A3 3.2, TT 3.2 or CC/Passat 3.6 DSG), VR6 DSG dual-mass flywheel, seals, DSG fluid and filter; full split and re-shim of the A3's 0D9 | 1,200 | 3,500 | Front case €140–210 used; flywheel and shop time *estimate*. **Fit unproven** — under investigation |
| 5 | Engine mount: Atlas 3QF 199 262 G/H + block console 022 199 354 T | 200 | 700 | TuneZilla proved the Atlas mount bolts to the 8V rail |
| 6 | Diagnostic/coding tool, if not already owned | 0 | 600 | |
| 7 | Cooling: S3-pattern radiator stack, expansion tank or Gray Fab bottle, custom/adapted hoses | 1,100 | 2,500 | Radiators US$162–699, aux US$125–230, bottle US$280 |
| 8 | A/C: custom compressor hoses, evacuate and recharge (+ compressor if not on the engine) | 400 | 1,400 | *estimate* |
| 9 | Exhaust: custom Y/mid-pipe from the Atlas cats into the A3 cat-back, keep all four O2 sensors | 1,000 | 2,500 | *estimate* |
| 10 | Fuel: fittings/adapters (the A3 quattro pump and controller feed a stock 3.6) | 100 | 300 | |
| 11 | Intake: airbox/MAF housing adaptation | 200 | 600 | *estimate* |
| 12 | Battery relocation to the trunk | 400 | 800 | Ninety4co: US$250 supplies + US$300 battery |
| 13 | Wiring: erWin diagrams for both VINs, pins, terminals, wire, loom | 300 | 600 | erWin ~US$35/day per brand |
| 14 | Front springs rated for the heavier VR6 nose | 300 | 1,000 | *estimate* |
| 15 | Fluids, hardware, gaskets, consumables | 500 | 1,000 | *estimate* |
| 16 | Shipping/duty/HST on other US/EU parts | 600 | 1,500 | ~15–20% |
| | ECU and DSG tuning | 0 | 0 | Self-tuned with tools already owned |
| | **Gross, excluding the A3** | **~12,100** | **~28,500** | |
| | Sell the A3's 2.0T engine, Simos ECU, intercooler and turbo parts | −2,000 | −4,500 | *estimate*; Ninety4co sold his 2.0T + gearbox for US$3,000 |
| | **Net, excluding the A3** | **~10,100** | **~24,000** | |

## What moves the number

- **Bellhousing (line 4) is the big unknown.** If a VR6 DSG front case does not fit the 0D9, the documented fallback is a used RS3/TT RS DQ500 with a machined VR6 bellhousing and adapter (€550–950), a VR6 DQ500 flywheel (€550–1,600) and a transfer-case bracket (£190). That replaces line 4 and adds roughly **CA$4,000–7,000**.
- **Engine mileage:** a sub-60k-mile engine costs more, but a cheap high-mile engine still needs the same timing and cooling refresh.
- **Not included:** the A3 itself (Ontario 2.0T quattro asks CA$10,500–20,000), insurance, shop labour, anything for power above stock.

Earlier version of this estimate (whole Atlas donor car, bought tools and tunes): CA$13,500–35,800 net. For comparison, the Mk6 Jetta GLI plan (BLV + Mk4 02M) is roughly CA$8,500–18,000 net excluding the car, from `README.md`.

# The VW Atlas / Atlas Cross Sport 3.6 VR6 (CDVC, MQB, 2018–2023) as a swap engine for a 2015–2020 Audi A3/S3 8V: engine identity, ECU, MQB immobilizer, tuning/immo-off, rebuild list

Research date: 2026-10-08. Donor: North American Atlas 3.6 (FWD or 4Motion, 2018–2023) and Atlas Cross Sport 3.6 (2020–2023). Recipient: 2015–2020 Audi A3/S3 8V, ideally quattro. This file builds on `/home/user/vr6_jetta/research_notes/Mk6 Jetta CDVC VR6 swap parts/engine_ecu_immobilizer.md` (the "Jetta file") and `.../precedents_vendors_salvage.md` (the "precedents file"). PQ35/NMS-specific material is not repeated; where an older finding is needed it is cross-referenced in one line.

Labels used on every claim:
- **VERIFIED** = read in a VW/Audi factory document (NHTSA-hosted bulletins and tech tips, fetched as PDF and text-extracted on 2026-10-08), a vendor product page fetched today, a Ross-Tech wiki page fetched today, or a parts-catalog/firmware-catalog page.
- **REPORTED** = forum, owner-report aggregator, dealer/used-car listing, or a search-engine summary of a page that could not be opened (marked "search snippet; page not opened").
- **INFERRED** = my reasoning from the cited material.

Sources that could not be read this run: Ross-Tech wiki pages "VW_Atlas_(CA)", "Audi_A3_(8V)" and "Component_Protection" (all HTTP 404 under those titles); go-parts.com (403); ECS Tuning and FCP Euro category pages (403); oemwolf pages for 03H906026E and 03H907309K (404); lessandmore/itunesystem/activemotion tuning-spec pages (404 today, although they were cited from search snippets in the Jetta file). VWVortex, r/vwatlas and YouTube were not used. The most useful new material is **six NHTSA-hosted VW documents** that name the Atlas engine code and list the ECU software part numbers by model year.

---

## Key question 1: Atlas / Atlas Cross Sport / Teramont 3.6 engine codes, output, compression, ECU family and part numbers by year (and the MED17.1.6 vs MED17.1.62 conflict)

### Takeaway
Every VW of America document found, from the 2018 launch to the end of the 2021 VIN range, calls the US Atlas and Atlas Cross Sport 3.6 **CDVC**, and lists ECU software part numbers only from the **03H 906 026 xx** family: 2018 E/F/J/S, 2019 R/AA/AH, 2020 AG/AF (Atlas and Cross Sport), 2021 AJ. A firmware catalogue ties 03H 906 026 E, the earliest 2018 unit, to **Bosch MED17.1.62**. So the claim in the earlier notes that "2018–19 = MED17.1.6 / 11.4:1, 2020+ = MED17.1.62 / 12.0:1" is very probably wrong. The two numbers that seemed to show a change are explained more simply:
- **Output:** "280 hp" is 280 PS (206 kW), which is the same engine as "276 hp". There was no output change.
- **Compression:** 12.0:1 is listed for the 2018 Atlas itself. 11.4:1 is the NMS Passat CDVB figure from VW's SSP.

The US Atlas has always been CDVC, MED17.1.62 and 03H 906 026 xx. The NMS Passat is CDVB, MED17.1.6 and 03H 906 023 xx. **CDVD** never appears in a US VW document. It shows up only in a third-party manual index and in reseller listings, so it is probably a non-US (Teramont) or late variant. No source documents it for 2022–2023 US cars.

### Cited Findings

**Engine code by year (VW documents)**
- **VERIFIED (VW Technical Bulletin 01 18 14, 2052606, 4 Oct 2018, NHTSA-hosted)** — "Atlas 2018, 3.6L (CDVC)". Update for P0300–P0306 and P068A ("ECM/PCM Power Relay De-Energized Performance – Too Early"). SVM table: old and new software part numbers **03H 906 026 E** (new SW version 6695), **03H 906 026 F** (6696) and **03H 906 026 J** (6697). Old versions were 3987/4192/4744/6024, 3988/4193/4745/6025 and 3989/4195/4748/6026. SVM code 41C6. — [NHTSA MC-10149916-9999.pdf](https://static.nhtsa.gov/odi/tsbs/2018/MC-10149916-9999.pdf)
- **VERIFIED (VW TSB 01-21-09, 2063514/3, released 6 Apr 2022)** — "Update Programming DTC's P0456 or P2407". Applies to Atlas 2018–2021 3.6L (CDVC), VIN CA_JC000001 to CA_MC599110, and Atlas Cross Sport 2020–2021 3.6L (CDVC), VIN CA_LC000001 to CA_MC234854. ECU software part numbers by year:
  - 2018 Atlas: **03H906026E, 03H906026F, 03H906026J, 03H906026S** (old versions 9970/9971, new 9972).
  - 2019 Atlas: **03H906026R, 03H906026AA, 03H906026AH** (new 9972; SVM code 455B appears beside this group).
  - 2020 Atlas: **03H906026AG, 03H906026AF** (new 9973).
  - 2020 Atlas Cross Sport: **03H906026AG** (new 9973).
  - 2021 Atlas / Atlas Cross Sport: **03H906026AJ** (old 0454/0638/1017, new 1689).
  — [NHTSA MC-10210224-0001.pdf](https://static.nhtsa.gov/odi/tsbs/2022/MC-10210224-0001.pdf)
- **VERIFIED (VW Tech Tip 17-18-02TT, 16 Nov 2018)** — "Atlas 2019 … 2.0L, 3.6L (DCGA, CDVC)": "the applicable oil type and viscosity has changed since the previous model year", per the under-hood sticker. — [NHTSA SB-10161178-9999.pdf](https://static.nhtsa.gov/odi/tsbs/2019/SB-10161178-9999.pdf)
- **VERIFIED (VW on-car analysis list, from 1 Dec 2021)** — "Atlas, Atlas Cross Sport 20-21, 3.6L (CDVC)": MIL with P0087, P0148 and P053F. — [NHTSA MC-10205521-0001.pdf](https://static.nhtsa.gov/odi/tsbs/2021/MC-10205521-0001.pdf)
- **VERIFIED (VW Tech Tip 20-19-01TT, 22 Feb 2019)** — "Atlas 2018, 3.6L (CDVC), All VIN": cold-start concern, with P102000 and P053F00. See Key question 6. — [NHTSA MC-10157341-9999.pdf](https://static.nhtsa.gov/odi/tsbs/2019/MC-10157341-9999.pdf)
- **VERIFIED (VW Tech Tip 01-19-01TT, 1 Mar 2019)** — "Atlas 2018-2019, 3.6L (CDVC)": coolant pump faults. See Key question 2. — [NHTSA MC-10155420-0001.pdf](https://static.nhtsa.gov/odi/tsbs/2019/MC-10155420-0001.pdf)
- **REPORTED (search snippet; third-party manual index)** — One VW 3.6 L 4V repair manual covers Atlas 2017, Atlas 2020 and Atlas (PA) 2020, "Engine code: CDVC, CDVD". — [vwts.ru](https://vwts.ru/vw_teramont_0a.html)
- **REPORTED (reseller/eBay listings, from the Jetta file)** — Oil pan 03H103601AK listed as fitting "Atlas Passat CDVC CDVD CDVB". Another listing pairs "Teramont 3.6L CDVC/CDVD 2018–2023". — [eBay 386433484222](https://www.ebay.de/itm/386433484222); [reseller page](https://sitio.usanjose.edu.co/item-tag/gc0751024/)
- **REPORTED (used-engine vendor, from the Jetta file)** — VIN position 5: "R" = Atlas 2018–2023, "E" = Atlas Cross Sport 2020–2023. — [transend.us](https://transend.us/products/engine/cylinder-block-components/engine-complete-assembly/engines100179265)
- **REPORTED (Wikipedia)** — VR6 applications: "2017–2024 Volkswagen Atlas; 2017–2024 Volkswagen Teramont; 2021–2024 Volkswagen Talagon". China also has a separate 2.5 L turbo VR6 (still EA390, 220 kW / 500 N·m) for the Teramont and Talagon. — [Wikipedia, VR6 engine](https://en.wikipedia.org/wiki/VR6_engine)

**ECU family**
- **VERIFIED (firmware catalogue, from the precedents file)** — "VW Atlas (CA) 3.6L VR6 FSI CDVC 206kW 280PS, **MED17.1.62**, 10SW059936, **03H906026E**". The Teramont CDVC is listed as MED17.1.61 with 03H906026AE. — [c4ip 145555](https://c4ip.ru/en/vw/145555-vw-atlas-ca-3-6l-vr6-fsi-cdvc-206kw-280ps-med17-1-62-10sw059936-03h906026e-9970-stock-eeprom-bin); [c4ip 148397](https://c4ip.ru/en/vw/148397-vw-teramont-3-6fsi-at-cdvc-med17-1-61-10sw043173-03h906026ae-6687-stock-full-flash-bin)
- **REPORTED (search snippet; parts guide, page 403)** — 2020–2021 Atlas Cross Sport 3.6: "match the part number (03H906026AG or **03H907309K**) and ensure the module is for the 3.6L engine, not the 2.0L". Used units cost $100–300. "A replacement ECM generally has to be programmed to the vehicle's immobilizer system unless it's bought pre-programmed." — [go-parts Atlas Cross Sport ECM](https://www.go-parts.com/garage/engine-control-module-ecm-volkswagen-atlas-cross-sport-2020-2021)
- **REPORTED (search snippets; tuning-file sites)** — "Atlas 2017–2019 3.6 V6 280hp: MED17.1.6, 11.4:1" and "Atlas 2020+ 3.6 V6 276hp: MED17.1.62, 12.0:1, engine code CDVC". These are the sources of the earlier conflict; the pages returned 404 on 2026-10-08. — [lessandmore 2017–2019](https://lessandmore.file-service.com/tuning-specs/volkswagen/atlas/2017-2019/36-v6-280hp); [activemotion 2020+](https://activemotion-performance.file-service.com/en/tuning-specs/volkswagen/atlas/2020-g/36-v6-276hp)
- Cross-reference (Jetta file, VERIFIED there): the NMS Passat 3.6 runs MED17.1.6, part 03H 906 023 DC, hardware **03H 907 309 A**, and is coded CDVB in VW's own 2016 Passat maintenance material.

**Output and compression**
- **REPORTED (search snippets: MotorWeek, TrueCar, cars.com spec page)** — 2018 Atlas 3.6: "276 @ 6200 SAE Net Horsepower", "266 @ 2750 SAE Net Torque", 8-speed automatic. — [cars.com 2018 Atlas specs](https://www.cars.com/research/volkswagen-atlas-2018/specs/393085/); [MotorWeek 2018 Atlas](https://motorweek.org/road_tests/2018-volkswagen-atlas/); [TrueCar 2018 Atlas](https://www.truecar.com/volkswagen/atlas/2018)
- **VERIFIED (Unitronic product page)** — "STOCK POWER: 276HP / 266LB-FT For Volkswagen Atlas Cross Sport 3.6 L EA390", 2020–2023. — [Unitronic Atlas Cross Sport 3.6](https://www.getunitronic.com/ecu-tuning/atlas-cross-sport-3.6-2020)
- **REPORTED (search snippets; dealer listings using manufacturer data feeds)** — 2018 Atlas 3.6L V6 SEL: "Compression ratio: 12.00 to 1 … bore x stroke: 89.0mm x 96.4mm". — [Autopark Honda listing](https://www.autoparkhonda.com/used/Volkswagen/2018-Volkswagen-Atlas-e7504aeeac18381b30e2fd5aef1234c5.htm); [Audi Central Houston listing](https://www.audicentralhouston.com/used/Volkswagen/2018-Volkswagen-Atlas-houston-tx-b070542cac182d59c0f767e2b895628c.htm)
- Cross-reference (Jetta file, VERIFIED there): VW SSP 800153 gives the NMS 3.6 as 11.4:1, 280 hp (206 kW) at 6600 rpm, 258 lb-ft, MED17.1, ULEV 2.

### Inferences
- **INFERRED (arithmetic)** — 206 kW = 280 PS = 276 hp (206 × 1.341 = 276.3; 206 ÷ 0.7355 = 280). The "280 hp 2017–2019 / 276 hp 2020+" split on tuning-file sites is a PS-versus-hp labelling artifact. The firmware catalogue labels the 2018 03H906026E unit "206kW 280PS", while the US documents rate the same 2018 engine at 276 hp. **There was no output change across 2018–2023.**
- **INFERRED** — On the ECU family, VW's own bulletins show 2018 Atlases with 03H 906 026 E/F/J/S, and the catalogue identifies 03H 906 026 E as MED17.1.62. The "MED17.1.6 for 2017–2019" entry on the tuning-file site is therefore a generic-family label, not evidence of a different ECU. Treat **every 2018–2021 US Atlas and Cross Sport as MED17.1.62 in the 03H 906 026 family**. No 2022–2023 bulletin was found, but nothing suggests a change.
- **INFERRED** — On compression, 12.0:1 is attached to the 2018 Atlas in dealer data, and 11.4:1 is VW's own NMS Passat figure. The "11.4:1 on 2018–19 Atlas" claim is probably carried over from the Passat spec block. Two consequences:
  - The Atlas CDVC probably differs from the NMS CDVB in pistons and/or combustion chamber as well as in ECU family.
  - An Atlas engine should be run on its own Atlas calibration (03H 906 026 xx), not on a Passat 03H 906 023 xx file.
- **INFERRED** — Hardware numbers point to the same Bosch hardware family: 03H 907 309 **A** for the Passat MED17.1.6 and 03H 907 309 **K** for the Atlas MED17.1.62 per the parts guide. That is consistent with one physical housing/connector family that carries different processors or software.
- **INFERRED — buying guidance by year:**
  - Any 2018–2021 Atlas CDVC is the same engine and ECU family.
  - The 2020–2021 cars (03H 906 026 AG/AF/AJ) carry the newest base software. They were still subject to the 2022 EVAP update, so ask whether it was done.
  - The 2020+ cars also avoid the 2018–2019 sunroof-drain and plenum water problem (Key question 3). That makes a **2020–2021 Atlas or Cross Sport** the cleanest donor, a 2022–2023 car acceptable but less documented, and a 2018–2019 car fine if the ECU is inspected for water corrosion.

### Gaps
- **Emissions certification level:** no source found for the 2018–2023 Atlas 3.6 (SULEV/ULEV/LEV III bin).
- **CDVD:** what it is (market, years, difference from CDVC) is not stated by any VW document. Read the code on the donor's engine label or service-data sticker.
- **2022–2023 US cars:** no VW document gives their engine code or ECU part numbers.
- **Bosch number:** no Bosch 0261Sxxxxx is tied to any 03H 906 026 xx. The Bosch repair-service catalogue search found only MED17.1.6 03H 906 023 units.

---

## Key question 2: Physical and accessory differences between the Atlas CDVC and the NMS Passat CDVB / B6 BLV

### Takeaway
Hard catalog data on Atlas-versus-Passat hardware is still thin. What the VW documents do show is that the Atlas engine carries MQB-era thermal-management and diagnostic content the BLV never had:
- an ECM-monitored **Heater Support Pump V488** and a coolant pump with ECM rpm feedback (P194A, P16C6);
- an HPFP driven from a **drive-chain sprocket** whose timing matters (P102000/P053F00 when mis-set);
- **start-stop** on later cars.

Alternator listings for the Atlas 3.6 span 140, 150 and 180 A units with MQB-family cross-references (04L 903 021 A, 03L 903 023 K, 04L 903 024 S), so the charging hardware is MQB-generation. The Atlas is an MQB vehicle with MQB-pattern engine mounts; one aftermarket mount kit is sold specifically for "MQB Atlas 3.6 8-speed". Intake manifold, injectors and HPFP part numbers, oil-filter housing, exhaust manifolds/cats and vacuum pump were **not** found for the Atlas in any catalog this run.

### Cited Findings
- **VERIFIED (VW Tech Tip 01-19-01TT, 2053847/2, 1 Mar 2019; Atlas 2018–2019 CDVC)** — "If either fault P16C600 (Heater Support Pump Dry Running) or P194A0 (Coolant Pump RPM Too High) are present in Engine/Motor Control Module -J623- … there may be air trapped [in] Heater Support Pump -V488-." The fix is a vacuum fill with VAS6096 and repeating the drain/fill with the vehicle's front raised. — [NHTSA MC-10155420-0001.pdf](https://static.nhtsa.gov/odi/tsbs/2019/MC-10155420-0001.pdf) (earlier revision: [MC-10157339-9999.pdf](https://static.nhtsa.gov/odi/tsbs/2019/MC-10157339-9999.pdf))
- **VERIFIED (VW Tech Tip 20-19-01TT)** — "This condition can be caused if the high pressure pump drive socket is not installed in the correct position … Check that the high pressure pump drive chain sprocket is in the correct position. See repair manual group 15 Cylinder Head, Valvetrain." — [NHTSA MC-10157341-9999.pdf](https://static.nhtsa.gov/odi/tsbs/2019/MC-10157341-9999.pdf)
- **REPORTED (search snippet; certified-used dealer listing)** — 2023 Atlas SE 3.6 VR6: "DOHC 24-Valve … direct fuel injection", start-stop system. — [overfuel dealer printout](https://api.overfuel.com/api/1.0/dealers/1428/printout/12/1621563)
- **REPORTED (search snippets; aftermarket catalog fitment tables)** — Alternators listed for the 2018–2020 Atlas 3.6L V6:
  - Remanufactured 140 A (MPA 11915), cross-referenced to **04L 903 021 A**;
  - Bosch reman 140 A (AL0170X), cross-referenced to **03L903023K** and **04L903024S**, with fitment note "To 140 Amp Alternator; with Bosch Unit";
  - Bosch new 180 A AL0935N ($568.64);
  - "Valeo 180 Amp" and "Valeo IR/IF 180 Amp" units;
  - Remy 11355 150 A, cross-referenced to Bosch 0-125-716-013/-014.
  — [partcatalog MPA 11915](https://www.partcatalog.com/products/mpa-electrical-11915-alternator); [partcatalog Bosch AL0170X](https://www.partcatalog.com/products/bosch-al0170x-alternator); [partcatalog Bosch AL0935N](https://www.partcatalog.com/products/bosch-al0935n-alternator); [partcatalog Remy 11355](https://www.partcatalog.com/products/remy-11355-alternator)
- **REPORTED (search-result title; page not opened)** — "BFI MQB – Engine Mount Kit – Atlas 3.6 – 8 Speed Auto – Stage 2". — [ACM Technik](https://acmtechnik.com/products/bfi-mqb-engine-mount-kit-atlas-3-6-8-speed-auto-stage-2)
- **REPORTED (owner-report aggregator)** — The Atlas 3.6 water pump is belt-driven on the passenger side. "the plastic thermostat housing/coolant flange" is a common leak source. — [au7o Atlas](https://au7o.io/known-issues/volkswagen-atlas?year=2022); [shopdap Atlas 3.6 water pump](https://shopdap.com/blog/post/vw-atlas-36-v6-water-pump.html)
- Cross-reference (Jetta file, REPORTED there): the lower oil pan **03H 103 601 AK/AD** is shared by Atlas CDVC/CDVD and Passat CDVB. The Spectra VWP61A aluminum pan lists the Atlas, Atlas Cross Sport, CC, Passat and Teramont. Valve cover **03H 103 429** family (C/B current, D/H/L superseded). Eurowise: "Engines with a 3.6L displacement have a different rear block mounting surface" than the 2.8/3.2.
- Cross-reference (Jetta file, VERIFIED there): the NMS SSP lists a one-part oil-pump sprocket, non-engaged chain tensioner, 3.6 bar oil pressure, 89 °C thermostat, 32° exhaust cam adjuster and 7-bolt damper. The Jetta file's electrical notes record that the NMS gateway J533 "controls the alternator charging via LIN-Bus".

### Inferences
- **INFERRED** — The Atlas engine is an MQB-integrated EA390. Its ECM supervises an auxiliary heater pump (V488) and coolant-pump speed, and the alternator family cross-references to MQB 03L/04L units. In an **A3 8V (also MQB)** this is an advantage: the A3's gateway and E-box are designed for LIN/BEM-managed alternators and ECM-driven auxiliary pumps. Keep the Atlas alternator, V488 and their wiring together. Do not fit the BLV-era 06F 903 023 alternator that the PQ35 builds used.
- **INFERRED** — Start-stop on the Atlas implies an AGM battery, a battery monitoring control unit and a start-stop-rated starter. The A3 8V also has start-stop on many trims, so the A3's battery-sensor, BEM and gateway infrastructure is already present. Disabling start-stop in the ECU (several bench services list "Start/Stop Disable", Key question 4) removes a source of faults if the A3's coding disagrees.
- **INFERRED** — A mount kit sold as "MQB Atlas 3.6" suggests the Atlas long block wears MQB-style engine and gearbox mount brackets. That is closer to the A3 8V's mounting scheme than the NMS/PQ46 Passat engine is. The Atlas, however, is the long-wheelbase MQB37W, so mount positions relative to the A3's rails are unverified. This belongs to the mounts researcher.
- **INFERRED** — The Atlas 4Motion transfer case (PTU) bolts to the Aisin 8-speed, not to the engine. FWD and 4Motion engines are therefore the same long block. Only the gearbox and PTU differ.

### Gaps
- No Atlas-specific part numbers or design notes were found for: intake manifold (one-piece vs two-piece), injectors, HPFP (number and drive detail beyond "drive chain sprocket"), oil-filter housing, vacuum pump (if any), engine-side mount bracket, A/C compressor bracket and belt layout, or exhaust manifolds and close-coupled catalysts. All need an ETKA VIN pull (oemwolf returned 404 for the ECU numbers tried; ECS and FCP returned 403).
- Atlas alternator OE part number and whether it is LIN-regulated: only aftermarket cross-references were found. 04L/03L numbers suggest MQB LIN units, but this is unverified.
- No VW SSP for the Atlas or its 3.6 engine was found online.

---

## Key question 3: ECU location and connectors on the Atlas, harness pieces to cut from the donor, and whether a MED17.1.62 pinout exists

### Takeaway
No source states where J623 sits in the Atlas or gives its connector pin counts, and no public MED17.1.62 pinout was found (rusEFI, ecuconnections and tuner wikis returned nothing; only paid "pinout tool" bundles exist). Two indirect clues apply:
- The 2018–2019 Atlas had a VW service action for **front sunroof drains routed through the plenum chamber**, and a parts guide says water from sunroof and A/C drains corrodes Atlas ECMs. Inspect the donor ECU and its connectors for water.
- The Atlas ECU hardware number family (03H 907 309 x) matches the NMS Passat's MED17.1.6 (03H 907 309 A), which in turn uses VAG's Bosch two-connector housing. This is consistent with a T94 + T60 pair, but that is unverified for MED17.1.62.

### Cited Findings
- **VERIFIED (VW Service Action 60E2, rev. 27 Feb 2024)** — "Front Sunroof Drain Cleaning & Modification – USA ONLY", 2018–2019 ATLAS. The procedure removes the plenum chamber covers and works "along the outer edge of the plenum … the plenum chamber on the left side". — [NHTSA MC-10250760-0001.pdf](https://static.nhtsa.gov/odi/tsbs/2024/MC-10250760-0001.pdf)
- **REPORTED (search snippet; parts guide, page 403)** — Atlas ECMs: "Inspect the old ECM for corrosion as water damage is a likely cause of failure". Leaks come from sunroof and A/C drains. — [go-parts Atlas ECM 2018–2022](https://www.go-parts.com/garage/engine-control-module-ecm-volkswagen-atlas-2018-2022)
- **REPORTED (NHTSA recall coverage)** — Recalls 18V-537 and 21V-892 involved water from the A/C drain reaching the **airbag** control module (not the ECM) on Atlas and Atlas Cross Sport. — [NHTSA 18V-537 report](https://static.nhtsa.gov/odi/rcl/2018/RCLRPT-18V537-1160.PDF); [recallcheck 21V892000](https://recallcheck.net/recall/21V892000)
- **REPORTED (search results)** — The only "MED17 pinout" sources are paid bundles of unknown quality: Payhip (mostly EDC17 listed) and a Gumroad "EDC17/MED17/MEV17/MEVD17/ME17/MEDG" tool. — [Payhip](https://payhip.com/b/DgiyP); [Gumroad](https://jaybeekeylock.gumroad.com/l/EcuPinOutsSoftwareBootBenchGpt1Gp2)
- Cross-reference (Jetta file, VERIFIED there): the AIM note for MED17.5.5 describes "a 60-position T60 and a 94-position T94"; "CAN communication protocol is on T94"; CAN-H pin 68, CAN-L pin 67. MED9.1 also uses T94 + T60 (rusEFI). The NMS Passat MED17.1.6 has hardware 03H 907 309 A (VCDS log).

### Inferences
- **INFERRED** — Treat the donor ECU as **T94 (engine harness) + T60 (vehicle harness)** until the plugs are counted on the donor. Hardware family 03H 907 309 x, shared with the NMS MED17.1.6, suggests the same Bosch case, but pin assignments are certainly different from the A3 8V's own ECU (Simos 18 on the 1.8/2.0 TFSI; the recipient ECU was not researched here).
- **INFERRED (cut list for an A3 8V recipient)** — From the donor take:
  - the complete engine harness with ECU and both plugs, cut back to the E-box/plenum bulkhead with long tails;
  - the engine-bay E-box (fuse/relay carrier) section that feeds terminal 30/15/87, ECM relay(s) and ignition/O2-heater supplies;
  - the accelerator-pedal pigtail;
  - the fuel-pump control module (J538) and low-pressure sensor pigtails;
  - V488 heater-support-pump and coolant-pump pigtails;
  - fan-control pigtail; alternator LIN/charge pigtail; battery monitoring sensor and start-stop starter pigtails;
  - both O2 sensor pairs' pigtails; the brake-switch pigtail.
  Take the **Atlas wiring diagram (erWin, "Atlas 2018–2023 3.6L") and the A3 8V diagram** before cutting anything. The A3 body side stays.
- **INFERRED** — Because the A3 8V and Atlas are both MQB, body-side CAN signals the ECU needs (ABS wheel speeds and torque intervention, steering angle, cluster, gateway, brake switch over CAN) use the same MQB message catalogue. This makes the "foreign ECU on powertrain CAN" problem smaller than in the PQ35 Jetta case. The remaining mismatches are vehicle-specific coding (gateway installation list, transmission type) and the immobilizer (Key question 4).

### Gaps
- Physical location of J623 in the Atlas (plenum/E-box vs engine-bay bracket): no source.
- Connector pin counts and any MED17.1.62 pinout: none public. A bench read of the donor's connector, or erWin diagrams (subscription), is required.
- Whether the A3 8V body-side ECU connector shell is the same as the Atlas's: not researched (needs the A3 recipient ECU identity).

---

## Key question 4: The MQB immobilizer (Immo 5) and component protection: master module, online adaptation of an Atlas ECU to an A3 8V, cost, and independent immo-off / clone services

### Takeaway
Both MQB cars use **Immobilizer 5**, with the immobilizer data held in the **instrument cluster** (Abrites: "immobiliser integrated into the instrument cluster" for MQB). The ECU and the transmission control unit are immobilizer participants. Ross-Tech states it **does not support Immobilizer 5** procedures at all.

VW's own MQB procedures require **ODIS online** for immobilizer adaptation, and the test plan asks for the purchaser's information and online login. That is the GeKo/FAZIT route. On paper a dealer can adapt a used Atlas ECU to an A3 8V's cluster, because both are MQB Immo 5. No dealer price or third-party online-account price was found, and no one has documented it for a cross-model (VW engine ECU into an Audi) case.

The 8V (2015–2020) predates SFD, which VW applies to the A3 **8Y**, Q3 F3 and Q4. That removes the newest lock-out.

Independent routes are well supplied:
- VinnieBuilt sells a **MED17.1.62 clone** ($175, currently sold out) with bench "IMMO Off", "VIN Change" and "Start/Stop Disable" add-ons.
- eBay sellers list "MED17.1.62 IMMO OFF" mail-in services from about $27.
- Abrites' professional MQB licences (€600 for 5A/5B data extraction, €1,800 for 5C) provide immobilizer data for ECU/TCU replacement with an extra parts-adaptation licence.

### Cited Findings
- **VERIFIED (Ross-Tech wiki, Immobilizer)** — "In most vehicles the Immobilizer Control Module is integrated into the Instrument Cluster. Upper Class Vehicles like the current Audi A5, A6, A8 and Q7 have a separate Immobilizer in Address 05 – Acc/Start Authorization." "Newer Audi Models also have the Transmission as Part of the Immobilizer." "Immobilizer Generation 5: Ross-Tech does not support Immobilizer 5 procedures at this time." Its procedure chart lists "ECU Swapping (Used)" for Immobilizer 5 as "N/A". On PINs: "The GeKo System sends it directly to the Dealers' Scan Tool … without ever showing the PIN to anyone." — [Ross-Tech wiki Immobilizer](https://wiki.ross-tech.com/wiki/index.php/Immobilizer)
- **VERIFIED (VW Tech Tip TT 96-14-05, 2015–2016 Golf/GTI/Golf R/SportWagen, MQB)** — Keys are adapted with the ODIS "Adapt Immobilizer" test plan, under "Elect. Immobilizer 5A". "Once the purchaser's information is entered and valid login credentials are provided, the adaptation status of all immobilizer components is displayed." — [NHTSA MC-10121095-9999.pdf](https://static.nhtsa.gov/odi/tsbs/2016/MC-10121095-9999.pdf)
- **VERIFIED (VW Tech Tip 57-21-01TT, rev. 3/10/2022)** — "MQB Vehicle, KESSY Key Adaptation". Covers Golf family 2015–2021, **Atlas 2018–2021, Atlas Cross Sport 2020–2021**, Tiguan LWB, Jetta 2019–2021, Arteon and Taos. "ODIS must show connection to internet services … run the Adapt Immobilizer test plan." — [NHTSA MC-10209098-0001.pdf](https://static.nhtsa.gov/odi/tsbs/2022/MC-10209098-0001.pdf)
- **VERIFIED (Audi TSB 2069282/1, 27 Jan 2023)** — "MQB/MEB: SFD requirement". Applies to Q3 2021–2024 and A3/S3/RS 3/Q4 2022–2024. "In order to service a vehicle with SFD (currently A3 (8Y), Q3 (F3 since MY2021), or Q4 (F4)), an ODIS login with SFD privileges is required." Replacing parts without privileges "may cause the new part to be irrevocably become unusable due to it being locked against manipulation". — [NHTSA MC-10230921-0001.pdf](https://static.nhtsa.gov/odi/tsbs/2023/MC-10230921-0001.pdf)
- **VERIFIED (Ross-Tech wiki, SFD)** — "SFD appeared first in MY 2020 and was at first limited to newly introduced Models and/or Control Modules." Ross-Tech also recommends opening the hood on "all MY 2015 and newer" to drop the diagnostic firewall. — [Ross-Tech wiki SFD](https://wiki.ross-tech.com/wiki/index.php/SFD)
- **VERIFIED (Abrites VN026 product page)** — €600 ex-VAT: "immobiliser data extraction for key learning, module replacement, and retrofit procedures on MQB Immo 5A/5B vehicles", including "ECU, TCU and ESL replacement support", for VW/Audi/Škoda/SEAT MQB 2012–2026. — [Abrites VN026](https://abrites.com/partial/vn026)
- **VERIFIED (Abrites VN025 product page)** — €1,800 ex-VAT, MQB Immo 5C: "MQB vehicles with HiTag PRO keys and immobiliser integrated into the instrument cluster". It provides "immobiliser data required for supported ECU and TCU replacement procedures". Supported modules: "DCM6.2, Simos 18.x, Bosch ECUs up to approximately 2021, DQ381, DQ200, DQ250, DQ500". "The VN002 Parts Adaptation license is required to complete ECU and TCU adaptation." — [Abrites VN025](https://abrites.com/partial/vn025)
- **VERIFIED (vendor page, fetched 2026-10-08)** — VinnieBuilt "MED17.1.62 ECU Clone": regular price **$175.00**, "Sold out". It "transfers all critical data — maps …" onto a replacement ECU. Bench add-ons listed: "DTC Off", "IMMO Off – Disable immobilizer system", "Stage 1 & Stage 2 Tuning", "VIN Change", "Start/Stop Disable", "Speed Limiter Removal". The URL slug names "audi-rs-med17-1-62". Miami, FL. — [VinnieBuilt MED17.1.62 clone](https://www.vinniebuilt.net/products/audi-rs-med17-1-62-clone-and-programming-service-miami)
- **REPORTED (search snippets; eBay and tool vendors; pages not opened)** — An eBay store lists "VAG BOSCH MED17.1.62 IMMO OFF" at $27.00. A separate ME17/MED17 immo-off listing says the shop "performs programming only", the "ECU is not included", and customers mail in their ECU. OBDSTAR DC706 (May 2025) "adds EDC17 MED17 … IMMO OFF function". Abrites VN004 lists MED17 immo-off and cloning. — [eBay store clesauto72 (snippet)](https://www.ebay.com/str/clesauto72/Music/_i.html); [eBay 125875874032](https://ebay.com/itm/125875874032); [obdii365 blog](https://blog.obdii365.com/2025/05/07/obdstar-dc706-adds-edc17-med17-pcr2-1-sim2k-immo-off/); [Abrites blog](https://abrites.com/blog/edc17-med17-in-vag-all-there-for-you)
- **REPORTED (from the precedents file; MHH Auto, search snippet)** — A swapped 2018 Atlas CDVC "fires up, stays running for a few seconds, then cuts out". A 2023 reply says owners have done MED17.1.62 immo-off themselves "for several years". — [MHH Auto](https://mhhauto.com/Thread-2018-VW-Atlas-SE-3-6-immo-off-Help)
- **REPORTED (search snippets; German workshop blog and VW Group erWin notice)** — The FAZIT/GeKo function covers "immobiliser calibration for units such as the engine ECU, component protection, and vehicle keys". Access requires a registered identity with a diagnostics role, and offline tools cannot clear component protection. — [kfz-dietrich component protection](https://kfz-dietrich.com/blog/vw-komponentenschutz-csp-odis-freischaltung/); [erWin FAZIT/GeKo notes](https://erwin.lamborghini.com/erwin/showOnlineServices.do)
- Cross-reference (precedents file, VERIFIED there): 06A Technik immo defeat $135 (MED9/MED17; 03H 906 026 not on its list). Speedo Solutions $250 + $100 for MED17.1; identity clone $300; "Off Road / Race / Diagnostic Applications ONLY".

### Inferences
- **INFERRED** — **Master module in the A3 8V:** the instrument cluster (J285). The A3 is not one of the "upper class" Audis with a separate address-05 immobilizer, and Abrites describes MQB immobilizer data as integrated in the cluster. Engine ECU, S tronic/DSG mechatronic (on Audis, the transmission is an immobilizer participant) and steering lock/KESSY are the slave components.
- **INFERRED** — **Three legitimate ways to make the Atlas ECU start in the A3:**
  1. **Dealer or independent ODIS-online adaptation** of the used Atlas ECU into the A3's Immo 5 ("Adapt Immobilizer" test plan with GeKo login and owner verification). Both cars are MQB Immo 5A/5B era and the 8V has no SFD, so the procedure exists. Whether GeKo accepts an engine ECU whose software is for a different model (VW Atlas) on an Audi VIN is unknown.
  2. **Bench immo-off** of the Atlas ECU (VinnieBuilt add-on; eBay mail-in MED17.1.62 services; MHH reports DIY is common). The A3 keeps its own cluster immobilizer for the rest of the car. Expect an immobilizer warning in the cluster unless the A3's immobilizer component list is edited to drop the engine ECU.
  3. **Professional MQB immobilizer-data route** (Abrites VN026 + VN002 at a locksmith or tuner) to adapt the used ECU as a replacement component. This is the most "factory-like" offline path and costs a shop roughly €600–2,400 in licences, so it would be done as a paid service.
- **INFERRED** — Recommended order: (2) bench immo-off combined with the same tuner's swap calibration, so it is one file, then (1) as a fallback if an Audi-aware shop with GeKo access will try it. **Component protection** applies to infotainment and comfort modules, not to the engine ECU. As long as the A3's own cluster, gateway and MMI stay, CP is not triggered by the engine swap.
- **INFERRED** — **Haldex and TCU:** the A3 quattro keeps its own Haldex 5 controller (which only needs engine torque and rpm on CAN) and, if a DSG is retained, its own TCU. The Atlas Aisin TCU and Atlas Haldex unit are **not** needed by the ECU for immobilizer purposes. The real problem is that the Atlas ECU software expects an Aisin automatic on CAN (Key question 5).

### Gaps
- Dealer labour/price for adapting a used engine ECU through GeKo on an Audi, and any third-party "online ODIS account" price: none found.
- Whether 03H 906 026 xx units are "TriCore tamper-protected" (locked for bench writing) on later software: no source found. TuneZilla's OBD flash of 2018–2022 units (Key question 5) shows at least OBD write access exists for stock software.
- Which exact Immo 5 sub-generation (5A, 5B or 5C) a 2015–2020 A3 8V and a 2018–2023 Atlas use: not found for either car. Abrites places 5C on HiTag-PRO-key cars "produced approximately between 20…" (text truncated on the page).

---

## Key question 5: Tuning software for the Atlas 3.6 (APR, IE, Unitronic, Malone, 034, others), swap features, and a standalone-ECU option

### Takeaway
The only shipping Atlas 3.6 tune found is **TuneZilla's Stage 1 ECU + TCU bundle**: $799, 2018–2021 (UroTuning) or 2018–2022 (NGP), 302 hp / 303 lb-ft, OBD flash via FlashZilla Pro. Its listing says "TCU Tuning is required to run the Stage 1 ECU tune", which ties the ECU file to an Aisin TCU being present.
- **Unitronic** lists the Atlas Cross Sport 3.6 EA390 (2020–2023) as "Stage 1: Under Development".
- **APR's** MED17 3.6 file covers Passat 12–18, CC, Touareg and Cayenne, not the Atlas.
- Generic file services list Atlas stage-1 maps (about 299 hp).
- No IE, 034 or Malone Atlas VR6 software was found.

**No tuner advertises swap features** (TCU/Haldex/ABS/cluster delete, manual-gearbox logic or immo off) for the Atlas ECU. The only swap-adjacent offer is VinnieBuilt's bench add-on menu (IMMO Off, DTC Off, Start/Stop Disable). For standalone ECUs, direct injection is the obstacle. Syvecs sells DI standalones (S7D-6 at about £3,700 ex-VAT) and VAG TFSI kits, but none for the 3.6. Forum users note that DI-capable MoTeC/Link units lack VAG CAN integration, and rusEFI's DI support is unconfirmed.

### Cited Findings
- **VERIFIED (NGP product page)** — TuneZilla "Stage 1 ECU & TCU Tune Bundle", "Fitment/Applications: 2018-2022 VW Atlas 3.6L". "Power is increased to 302 HP and 303 FT-LB." Flashed with the "TuneZilla Portal App and FlashZilla Pro dongle". "Requirements: TCU Tuning is required to run the Stage 1 ECU tune." "TuneZilla does not remove or modify factory readiness monitors." "If your ECU has been tuned previously, please return it to stock." Page price data **$799.00**. — [NGP TuneZilla Atlas 3.6](https://store.ngpracing.com/products/tunezilla-ecu-software-tune-vw-atlas-3-6l-vr6)
- **VERIFIED (UroTuning product page)** — "TuneZilla Performance ECU & TCU Tune – VW Atlas 3.6L (2018-21)", **Part# 36-VR6-CDVC-280-001**, "Stage 1 ECU & TCU Bundle (302 hp / 303 lb-ft)", $799.00, "clearance item is FINAL SALE". — [UroTuning](https://www.urotuning.com/products/tunezilla-performance-ecu-tune-vw-atlas-3-6l-2018-21)
- **VERIFIED (Unitronic page)** — "Unitronic Stage 1 : Under Development – STOCK POWER: 276HP / 266LB-FT For Volkswagen Atlas Cross Sport 3.6 L EA390"; the page title covers 2020–2023. — [Unitronic Atlas Cross Sport 3.6](https://www.getunitronic.com/ecu-tuning/atlas-cross-sport-3.6-2020)
- **VERIFIED (APR product page via search, also in the Jetta file)** — ECU-36L-EA390-MED17: "Porsche Cayenne 11-18; Volkswagen CC 12-16, Passat 12-18, Touareg 11-17". No Atlas. — [goapr ECU-36L-EA390-MED17](https://www.goapr.com/products/software/ecu_upgrade/gasoline/6/vr6/parts/ECU-36L-EA390-MED17)
- **REPORTED (search snippets; file-service sites)** — ECU Technologies: Atlas 2017–2019 "280hp" to 299 hp (370 to 399 Nm), with "stage 1, stage 2, decat" options; Atlas Cross Sport 2020+ 276 hp to 299 hp (361 to 385 Nm). — [ecutech Atlas 2017–2019](https://ecutech.file-service.com/account/en/specs-pages/volkswagen/atlas/2017-2019/36-v6-280hp); [ecutech Atlas Cross Sport 2020+](https://ecutech.file-service.com/account/en/specs-pages/volkswagen/atlas-cross-sport/2020-g/36-v6-276hp)
- **REPORTED (search snippets; Syvecs and reseller)** — Syvecs S7D-6 direct-injection standalone £3,700 ex-VAT. Syvecs sells a "full standalone kit for all 4 Cylinder TFSI equipped cars, with full Direct Injection and Pump Control" and an RS3/TTRS 8V2 kit "with support for full direct injection control and up to 10 injectors". No 3.6 VR6 kit is listed. — [Syvecs S7D-6 (reseller)](https://www.garagewhifbitz.co.uk/?p=111553); [Syvecs direct-injection tag](https://www.syvecs.com/product-tag/direct-injection); [Syvecs Audi S3 TFSI plug-in](https://www.syvecs.com/?p=4856)
- **REPORTED (HP Academy forum)** — "you'd be hard pressed … to find an ECU that will support DI plus offer easy integration with the rest of the car's CAN comms"; "MoTeC and Link both offer DI support but neither offer the CAN comms support". — [HP Academy "help standalone direct injection"](https://hpacademy.com/forum/general-tuning-discussion/show/help-standalone-direct-injection)
- **REPORTED (rusEFI forum/wiki, conflicting)** — The wiki lists direct injection as a feature. A forum post says "As of April 2019, rusEfi is quite far from GDI". — [rusEFI forum](https://www.rusefi.com/forum/viewtopic.php?p=44094); [rusEFI wiki](https://wiki.rusefi.com/)
- **REPORTED (press)** — MQB precedent for a VR6: HGP put a twin-turbo 3.6 VR6 into a Golf 7 R with an RS3 transmission. It is TÜV-approved, the conversion costs about $110,000 without the donor, and the MQB car "took considerably more engineering work" than HGP's Golf 6 R version. — [The Drive](https://www.thedrive.com/news/31234/watch-a-two-door-vr6-swapped-vw-golf-r-touch-220-mph-on-the-autobahn.md); [CAR magazine](https://www.carmag.co.za/news/this-bi-turbo-vr6-powered-golf-7-r-makes-550-kw/)
- Cross-reference (Jetta file, VERIFIED there): Ross-Tech's Uwe says transmission type lives in engine coding Byte 1, a different gearbox needs gateway-list edits, and "a number of other modules will start complaining about missing messages from the TCU". United Motorsport takes swaps only as custom requests through NGP and lists the 3.6 for MED9 only.

### Inferences
- **INFERRED** — For an A3 8V the gearbox decision drives the ECU problem:
  - **Atlas Aisin 8-speed + Atlas TCU:** the ECU is happy and the TuneZilla file applies. The Aisin/PTU does not fit an A3 tunnel or the Haldex driveline (other researchers own this).
  - **A3 DSG (DQ250/DQ381) or a manual:** the Atlas ECU sees no Aisin TCU. It needs Byte-1 coding (if the software accepts it) plus a custom calibration that suppresses TCU messages and adds clutch-switch or DSG torque-interface logic. Nobody sells this off the shelf. It is custom WinOLS work: an independent MED17 tuner, United Motorsport by custom request, or the bench service that does the immo-off.
- **INFERRED** — The A3 quattro's own Haldex 5 controller and ABS/ESC are MQB modules that read engine torque and rpm over CAN, and the Atlas ECU already broadcasts the MQB message set for an Atlas 4Motion Haldex. A **Haldex delete is not needed**. The Atlas Haldex controller stays in the Atlas.
- **INFERRED — standalone budget (no 3.6 precedent):** about £3,700 for a Syvecs S7D-6 plus harness, DI injector/HPFP calibration, a CAN gateway emulation for the MQB cluster, EPS, ABS and Haldex, and dyno time. That plausibly totals **US$8,000–12,000**, against roughly **$175–350 for an immo-off/clone plus an unpriced custom swap calibration** on the OEM ECU. MQB EPS and ABS need engine-running and torque messages on CAN, so a standalone without full MQB CAN emulation would lose power steering and stability control. The OEM-ECU route is strongly preferred.

### Gaps
- No price or scope from any tuner for an Atlas MED17.1.62 **swap** file (TCU-delete, manual or DSG adaptation, Haldex/ABS fault handling).
- No published IE, 034, Malone or HP Tuners support for the Atlas 3.6 was found (Malone's "FSI VR6 280" listing in the Jetta file has unverified fitment).
- Whether the TuneZilla ECU file can be ordered without the TCU half: not stated.
- MaxxECU, Haltech and Link DI driver suitability for the 3.6's injectors and HPFP: unverified.

---

## Key question 6: Reliability and rebuild list for the Atlas 3.6, recalls/TSBs, recommended donor year and mileage, timing and gasket part numbers

### Takeaway
VW's own Atlas CDVC documents identify five software and service items:
- ECM software updates for misfires/P068A (2018) and EVAP P0456/P2407 (2018–2021);
- HPFP drive-chain-sprocket mispositioning causing cold-start fuel-pressure faults (2018);
- an oil-spec change for 2019;
- air-trapped Heater Support Pump V488 faults after coolant service (2018–2019);
- a 2020–21 helpline case for P0087/P0148/P053F (low fuel rail pressure).

Owner aggregates add timing-chain stretch (upper chain and tensioner first, $2,000–4,500) and coolant leaks from the water pump and plastic thermostat housing. Shared EA390 timing parts (iwis 066109503C, Febi 25404, oil-pump chain 021109465B, INA tensioner 066109507D) and Atlas-specific FCP kits are catalog-listed. The prudent donor is a **2020–2021 Atlas or Atlas Cross Sport** under about 60,000 miles with service records. Plan a full timing job, water pump, thermostat housing and valve cover/PCV before install regardless.

### Cited Findings
- **VERIFIED (VW TB 01 18 14)** — 2018 Atlas CDVC: P0300–P0306 and P068A from "Current Engine Control Module (ECM) software causing erroneous faults". Fixed with 03H 906 026 E/F/J software 6695/6696/6697 or higher. — [NHTSA MC-10149916-9999.pdf](https://static.nhtsa.gov/odi/tsbs/2018/MC-10149916-9999.pdf)
- **VERIFIED (VW TSB 01-21-09)** — 2018–2021 Atlas and 2020–2021 Cross Sport CDVC: P0456 or P2407, because the software "is allowing the diagnosis of some EVAP faults" (software table in Key question 1). — [NHTSA MC-10210224-0001.pdf](https://static.nhtsa.gov/odi/tsbs/2022/MC-10210224-0001.pdf)
- **VERIFIED (VW Tech Tip 20-19-01TT)** — 2018 Atlas CDVC: "At cold start the engine RPM fluctuates heavily, the EPC light is ON", with P102000 "Fuel Pressure Regulation Limit Exceeded" and P053F00 "Cold Start Fuel Pressure Performance". Cause: the HPFP drive sprocket not in the correct position. — [NHTSA MC-10157341-9999.pdf](https://static.nhtsa.gov/odi/tsbs/2019/MC-10157341-9999.pdf)
- **VERIFIED (VW on-car analysis list, Dec 2021)** — Atlas and Atlas Cross Sport 20–21 3.6L CDVC: "MIL-on with P0087 P0148 P053F" (low fuel rail pressure / fuel delivery error / cold-start fuel pressure). Requires a VW Helpline call before repair. — [NHTSA MC-10205521-0001.pdf](https://static.nhtsa.gov/odi/tsbs/2021/MC-10205521-0001.pdf)
- **VERIFIED (VW Tech Tip 17-18-02TT)** — 2019 Atlas CDVC oil type and viscosity changed from 2018; follow the under-hood sticker. — [NHTSA SB-10161178-9999.pdf](https://static.nhtsa.gov/odi/tsbs/2019/SB-10161178-9999.pdf)
- **VERIFIED (VW Tech Tip 01-19-01TT)** — 2018–2019 Atlas CDVC: V488 Heater Support Pump air-lock, P16C600 and P194A00. Fill with VAS6096 and the front raised. — [NHTSA MC-10155420-0001.pdf](https://static.nhtsa.gov/odi/tsbs/2019/MC-10155420-0001.pdf)
- **VERIFIED (VW Service Action 60E2)** — 2018–2019 Atlas front sunroof drain cleaning and modification (plenum water). — [NHTSA MC-10250760-0001.pdf](https://static.nhtsa.gov/odi/tsbs/2024/MC-10250760-0001.pdf)
- **REPORTED (owner-report aggregator)** — Atlas 3.6 "timing chain stretch, causing a rattle on startup", upper chain and tensioner "more prone to wear", repairs $2,000–4,500. Coolant leaks from the water pump and "plastic thermostat housing/coolant flange". The German page cites "TSB 15-18-03" for chain noise and says onset is more common from about 60,000 miles (TSB not seen). — [au7o Atlas 2023](https://au7o.io/known-issues/volkswagen-atlas?year=2023); [au7o Atlas 2022](https://au7o.io/known-issues/volkswagen-atlas?year=2022); [au7o DE](https://au7o.io/de/known-issues/volkswagen-atlas)
- **REPORTED (shop blog)** — The Atlas 3.6 water pump fails mostly by leak, "in many cases the bearings fail"; failures are "less common compared to the 2.0T". — [shopdap Atlas 3.6 water pump](https://shopdap.com/blog/post/vw-atlas-36-v6-water-pump.html)
- **REPORTED (BITOG forum, Passat EA390)** — PCV diaphragm failure shows as oil consumption or an idle change when the port near the diaphragm is blocked. Low-tension ring sticking was also suggested. Carbon on DI intake valves was discussed. — [BITOG VR6 Passat GDI intake valves](https://bobistheoilguy.com/forums/threads/how-bad-are-these-vr6-passat-gdi-intake-valves.407652/post-7614231)
- Cross-reference (Jetta file, VERIFIED there from the FCP Euro Atlas Timing category):
  - iwis timing chain **066109503C** ($79.99) and Febi **25404** ($76.99), both listing Atlas;
  - iwis oil-pump chain **021109465B** ($62.99);
  - INA upper-chain tensioner **066109507D** ($33.31);
  - Atlas kits FCP KIT-00290 ($561.77), OE-supplier KIT-00299 ($397.10), KIT-00298 ($704.26), Genuine VW KIT-00291 ($1,056.38);
  - Hendrick VW lists genuine timing chain **03H 109 503 B** for "3.2L and 3.6L" (REPORTED);
  - Febi switchable water pump 95810603302 ($204.99) appears on ECS's Atlas page (REPORTED, number not verified against VW ETKA);
  - lower oil pan 03H 103 601 AK/AD; valve cover/PCV 03H 103 429 family.
  — [FCP Euro Atlas Timing](https://www.fcpeuro.com/Volkswagen-parts/Atlas/Timing/); [shopdap Atlas water pump guide](https://shopdap.com/blog/post/vw-atlas-water-pump.html)

### Inferences
- **INFERRED (donor choice)** — Buy a **2020–2021 Atlas or Atlas Cross Sport** (VIN position 5 "R" or "E"; base ECU 03H 906 026 AG/AF/AJ). The reasons:
  - it avoids the 2018 launch-software, HPFP-sprocket and V488 air-lock items and the 2018–2019 sunroof-drain water risk to the ECU;
  - it falls inside the 2022 EVAP-software TSB, so you can confirm the ECU is at SW 9973 or 1689 or higher before a tuner reads it.
  Prefer under about 60,000 miles (the aggregator's chain-stretch onset) and documented oil changes. FWD and 4Motion engines are equivalent (Key question 2).
- **INFERRED (pre-install list, in priority order)** —
  1. Full timing set while the engine is out, ordered by OE number, not vehicle filter: upper chain 03H 109 503 B or 066109503C equivalent, lower chain, oil-pump chain 021109465B, upper tensioner 066109507D, all rails and guides. Verify and mark the **HPFP drive-chain sprocket position** per Tech Tip 20-19-01TT.
  2. Water pump (verify OE number by VIN; the Febi 958… number is Porsche-numbered), thermostat/coolant flange housing, all coolant hoses; refill with the V488 bleed procedure.
  3. Valve cover/PCV (03H 103 429 family) and the oil-separator diaphragm.
  4. Walnut-blast the intake valves (DI engine; carbon not documented by VW for the Atlas).
  5. HPFP and injector seals; the fuel-pressure faults P0087/P053F appear in VW's 2020–21 helpline list.
  6. Inspect the ECU and its plugs for water corrosion; replace the engine harness if connectors are brittle.
  7. Rear main seal and oil-pan sealing (03H 103 601 AK pan).
  8. A bearing inspection if the core is over about 100,000 miles (the BLV spun-bearing precedent is in the local baseline).

### Gaps
- Gasket and timing-cover part numbers (03H 109 xxx covers, head and valve-cover gaskets, upper and lower tensioner and rail OE numbers) could not be pulled. ECS, FCP and oemwolf were blocked for these pages. An ETKA VIN lookup is needed.
- No VW TSB on Atlas 3.6 timing-chain stretch, oil consumption, PCV or carbon was found as a primary document. "TSB 15-18-03" is cited only by an aggregator.
- No VW recall on the Atlas 3.6 engine itself was found. The Atlas recalls found concern airbag-module water ingress (18V-537, 21V-892).

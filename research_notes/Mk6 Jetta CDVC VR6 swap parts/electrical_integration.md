# Electrical integration of a 3.6 VR6 CDVC (2012–2018 NMS Passat) ECU into a 2015–2018 Mk6 Jetta GLI manual

Scope: engine-bay fuse box (E-box), CAN gateway (J533), instrument cluster, ABS/ESC incl. XDS, power steering type by trim/year, body harness and ECU body-side connector, charging/starting, cooling-fan control, and factory wiring-diagram access. North American vehicles only. Donor = 2012–2018 NMS Passat 3.6 (engine code CDVC per the precedents file; Bosch MED17.1.6x, ECU family 03H 906 026 x). Recipient = 2015–2018 Mk6 Jetta GLI 6-speed manual (EA888 Gen3, 02Q), with 2.5L/1.8T/TDI notes.

Labels: **VERIFIED** = parts-catalog fitment data, factory document, Ross-Tech wiki or vendor product page; **REPORTED** = forum/build thread/marketplace listing/press repost; **INFERRED** = my reasoning from the cited material. Local baseline files are cited by path. Access limits this run: erwin.vw.com redirects to vw-us.erwin-store.com, whose price pages require a login (no prices visible); parts.centralvalleyvw.com returned 403; no VW dealer catalog page with fitment lists could be opened, so most part numbers below are marketplace/vendor numbers and are labelled accordingly. No part number in this file is invented; where none was found the item is in Gaps.

Already covered in `precedents_vendors_salvage.md` (not repeated here except where needed for context): MED17 immobilizer services and pricing, CDVC ECU hardware numbers, tuner support, Stance Dubs swap-harness requirements, Mk6 Jetta cluster/gateway forum lore.

## Key question 0: Do the Mk6 Jetta and the NMS Passat share one electrical generation, making this swap simpler than Ninety4co's 2010 GTI + 2006-era BLV job?

### Takeaway
Yes at the architecture level: Ross-Tech documents the 2011+ Jetta (16/AJ) and the 2012+ Passat NMS (A3) with the same Golf-Mk6-generation module set (MK60EC1 ABS with the identical label file, BCM with the comfort system merged in, AirbagVW10 5K0 959 655, Steering Assist at address 44, cluster family shared with the Golf 5K), whereas Ninety4co's donor was a B6 Passat (3C, 2006–2008, MED9, separate comfort module, 3C0 gateway). The engine ECU itself is the big difference: CDVC is MED17 like the Jetta's own EA888 Gen3 ECU, while BLV was MED9. "Same generation" does not mean "same pinout": the Jetta's cluster and body harness differ from the Golf's, so Ninety4co's pin numbers still cannot be copied.

### Cited Findings
- **VERIFIED** — Ross-Tech: VW Jetta (16/AJ), platform VW36X, MY2011+ (US 2011+); modules: 01 engine, 02 02E DSG/09G, 03 brakes MK60EC1 and MK70M, 05 access/start, 08 manual HVAC/Climatic, 09 BCM (doors must be unlocked to communicate), 15 AirbagVW10 (5K) and AirbagVW11 (replacement needs online configuration, not supported by VCDS), 17 cluster (linked to the Golf 5K/52 cluster page), 19 gateway, 25 immobilizer, 2B steering column lock, 44 Steering Assist, 46 comfort "merged into the BCM and no longer a separate address", 65 TPMS not used on 2011–2012 NAR cars (indirect TPMS runs in the MK60EC1). — [Ross-Tech wiki, VW Jetta (16/AJ)](https://wiki.ross-tech.com/wiki/index.php/VW_Jetta_(16/AJ))
- **VERIFIED** — Ross-Tech: VW Passat (NMS/A3), platform VW411, MY2012+ NAR only (RoW B7 is on the 3C page); modules: 02 02E DSG (02E-300-0xx.LBL) or 09G; 03 MK60EC1, label 1K0-907-379-60EC1F.CLB; 08 manual HVAC label 5C0-820-047.CLB; 09 BCM linked to the Golf 5K BCM page, comfort system 46 now part of the BCM; 15 AirbagVW10 label 5K0-959-655.clb; 16 steering wheel 1K0-953-549 / 5K0-953-569; 17 cluster linked to the Golf 5K/52 cluster page; 19 gateway; 44 Steering Assist linked to the Golf (1K) Steering Assist page; also 1C, 25, 2B, 2E, 42, 47, 4F, 52, 77. — [Ross-Tech wiki, VW Passat (NMS/A3)](https://wiki.ross-tech.com/wiki/index.php/VW_Passat_(NMS/A3))
- **VERIFIED** — The MK60EC1 page both cars link to says ABS coding "is normally done through Software Version Management (SVM)" (long coding, dealer tool), that a readable old module's coding is copied to the new one, and that steering-angle (G85) basic setting and steering-limit-stop adaptation must follow coding. — [Ross-Tech wiki, Golf (1K) Brake Electronics (MK60EC1)](https://wiki.ross-tech.com/wiki/index.php/VW_Golf_(1K)_Brake_Electronics_(MK60EC1))
- **VERIFIED** — NMS Passat 3.6: EA390 3,597 cc VR6 FSI, 280 hp / 258 lb-ft, **6-speed DSG only**, offered MY2012–2018, dropped after 2018; platform listed as PQ46 ("an extended version of the European car's platform"); 2016 facelift added MIB II, rear camera, post-collision braking and driver-assist options. No power-steering statement on the page. — [Wikipedia, Volkswagen Passat (North America and China)](https://en.wikipedia.org/wiki/Volkswagen_Passat_(North_America_and_China))
- **VERIFIED (firmware catalogue)** — Atlas CDVC: Bosch MED17.1.62, hardware 03H 906 026 E (from the precedents file). — [c4ip.ru](https://c4ip.ru/en/vw/145555-vw-atlas-ca-3-6l-vr6-fsi-cdvc-206kw-280ps-med17-1-62-10sw059936-03h906026e-9970-stock-eeprom-bin)
- **REPORTED (local baseline)** — Ninety4co's donor was a B6 Passat 3.6 BLV with MED9-era harness; his recipient a 2010 GTI CCTA; he needed the B6/VR6 "high" E-box 1K0 937 124 K for its T26 and T40 connectors and re-pinned ~30 fuse-box and ~45 T94 positions. — [ninety4co-swap-wiring-repins.md](/home/user/vr6_jetta/research/sources/ninety4co-swap-wiring-repins.md), [ninety4co-swap-parts-list.md](/home/user/vr6_jetta/research/sources/ninety4co-swap-parts-list.md)
- **REPORTED (marketplace)** — Gateway numbers on both cars are in the 7N0 907 530 family: 7N0 907 530 AM sold as a 2012 Passat SE gateway; 7N0907530T and 7N0907530P listed for 2012–2015 Passat B7 (NMS); 7N0907530L listed for 2011–2012 CC 2.0/3.6; 7N0907530AN listed "for VW Jetta Golf MK6"; 7N0907530M for Golf Mk6 2009–2012. — [eBay seller feedback (7N0 907 530 AM)](https://www.ebay.com/usr/glenlar-97); [FridayParts 7N0907530L](https://www.fridayparts.com/can-bus-gateway-control-module-7n0907530l-for-volkswagen-cc-2-0l-l4-3-6l-v6-2011-2012); [eBay 7N0907530AJ listing cross-referencing AN](https://www.ebay.de/itm/395869643406)
- **REPORTED (forum, from precedents file)** — Mk6 Jetta cluster shares the Golf's plug but not its pinout ("the Golf cluster will physically mount up and plug in, it won't function at all"). — [VWVortex 7149179](https://www.vwvortex.com/threads/mk6-cluster-in-a-mk4-or-mk5.7149179/)
- **REPORTED (marketplace)** — Same E-box cover for both cars: "Fusebox Cover For 2011-2018 Volkswagen VW Jetta Passat Beetle 5C0937132A". — [eBay 400555801413](https://www.ebay.com/itm/400555801413)

### Inferences
- **INFERRED** — The 2011 Jetta, 2012 Beetle (5C) and 2012 NMS Passat were all engineered on the Golf Mk6 (5K) electrical generation ("PQ35 Gen 2": BCM with integrated comfort functions, MK60EC1 ABS, 7N0 gateway, MED17 engine ECUs, 5C0/5K0 part prefixes). The B6 Passat BLV that Ninety4co used belongs to the previous generation (3C0 gateway, separate 46 comfort module, MED9.1). So the generational mismatch he fought (power-distribution relays, LDP, fan-module pins, pedal pinout) should be smaller for a CDVC ECU, whose MED17.1.6x shares the Bosch MED17.1 I/O architecture with the Jetta GLI's MED17.5.
- **INFERRED** — "Simpler" has limits: (a) the Jetta's body harness and E-box population are engine-specific and differ from both the Golf and the Passat; (b) the CDVC only ever ran with a DSG in North America, so the manual-transmission inputs (clutch switch, reverse light, no TCU on CAN) are new territory for its software; (c) the immobilizer (Immo 4, cluster-based) still has to be defeated or matched.

### Gaps
- No factory document (SSP, erWin) was retrievable to confirm the architecture statement directly; it rests on the Ross-Tech module lists above.
- Whether the NMS Passat 3.6 and the Jetta GLI use the same ECU connector housing (94-pin body side + 60-pin engine side) could not be verified from a published source.

## Key question 1: Engine-bay fuse/relay box (E-box)

### Takeaway
No catalog fitment list for any Mk6 Jetta or NMS Passat E-box carrier could be opened. Marketplace data shows both cars use the PQ35-family 1K0 937 12x carrier with a 5C0 937 132 x cover, and that the GLI's box differs from the other Jettas' ("except GLI" listings). Whether a Jetta box carries the T26/T40 connectors the 3.6 harness needs is unknown; the donor Passat's box, cut out with its harness tail as Ninety4co did, remains the safe plan.

### Cited Findings
- **REPORTED (local baseline)** — Ninety4co: the Mk6 GTI E-box lacked the T26 connector; he fitted the PQ35 VR6 "high" box 1K0 937 124 K ("get a used one and cut it out with its cabling and connectors", "very expensive new"); the 3.6 harness uses T40 and T26 on the box; his front-feed pole table (L→R): alternator 150/200 A, power steering 80 A, coolant fan module 50 A, battery unfused, fuse panel C 80 A, not used, battery 125 A, not used, not used, battery 80 A. — [ninety4co-swap-wiring-repins.md](/home/user/vr6_jetta/research/sources/ninety4co-swap-wiring-repins.md)
- **REPORTED (marketplace)** — A 1K0 937 125 D / 1K0 937 629 A relay-board set is sold for 2006–2011 Mk5 Jetta with the note "not fit GLI", seller asks for VIN. — [eBay 175362670376](https://www.ebay.com/itm/175362670376)
- **REPORTED (marketplace)** — 1K0937125 tagged as the OEM number of a box for "VW Jetta III (1K2) 1.6 petrol", build range 2004–2013. — [autoparts-24](https://www.autoparts-24.com/item/A_0047_KH5352/?pos=11)
- **REPORTED (marketplace)** — 5C0937132B described as "Jetta engine fuse box '14, except GLI". By VW numbering (937 124/125 = carrier, 937 132 = cover) this is most likely the cover, so the "except GLI" note says the GLI's box top differs. — [eBay 395998205872](https://www.ebay.de/itm/395998205872)
- **REPORTED (marketplace)** — 5C0937132A fuse-box cover listed for 2011–2018 Jetta, Passat, Beetle. — [eBay 400555801413](https://www.ebay.com/itm/400555801413)
- **VERIFIED (vendor page, no fitment shown)** — FCP Euro lists a genuine "Audi VW Fuse and Relay Center 1K0937125A" in its fuse-strip category. — [FCP Euro fuse strip category](https://www.fcpeuro.com/Volkswagen-parts/Fuse-Strip/)
- **VERIFIED (vendor page)** — FCP Euro lists the fuse-box cover 1K0937701B for CC, Passat, Jetta, Eos, Rabbit (cover only). — [FCP Euro Rabbit fuse box cover](https://www.fcpeuro.com/Volkswagen-parts/Rabbit/Fuse-Box-Cover/)
- **REPORTED (fuse-diagram sites, from precedents file)** — Mk6 Jetta engine-bay fuse assignments change by model year (2011–2013 vs 2014–2017), and a 2015 diagram is marked valid "up to June 2015". — [fuseandrelay.com Jetta 6](https://fuseandrelay.com/volkswagen/jetta-6.html); [bolidenforum 2015 Jetta](https://www.bolidenforum.de/portal/fuse-box/volkswagen/jetta/2015/); [bolidenforum 2012 GLI](https://www.bolidenforum.de/portal/fuse-box/volkswagen/gli/2012/)

### Inferences
- **INFERRED** — Because the Jetta Mk6, Beetle and NMS Passat share the 5C0 937 132 cover family and the Golf/Jetta Mk5–6 share the 1K0 937 12x carrier, all of these E-boxes are one physical family and a donor NMS Passat 3.6 box should drop into the Jetta's tray as the B6 box did into Ninety4co's GTI. Take the Passat box **with its harness tail and the engine-harness connectors (T40/T26 equivalents) attached**; that sidesteps the question of whether the GLI box is populated for a V6.
- **INFERRED** — The GLI-specific box ("except GLI" listings) is probably populated for the EA888 Gen3's extra circuits (electric coolant pump, turbo wastegate actuator, etc.), which does not make it VR6-ready; the 3.6 needs a bank-2 O2 heater feed, an after-run pump relay and an ECM relay 2 that the 4-cylinder box may not carry.

### Gaps
- Mk6 Jetta E-box carrier part numbers by year/engine (GLI, 2.5, 1.8T, TDI) and the NMS Passat 3.6 carrier number: no dealer catalog page could be opened (parts.centralvalleyvw.com 403; parts.vw.com needs a vehicle-specific URL). erWin/ETKA by VIN is the way to get them.
- Whether 1K0 937 124 K itself appears in the NMS Passat 3.6 fitment list (no hit in any catalog or listing).
- Which of Ninety4co's ten front-feed poles are present on the Jetta GLI box (his table is for the GTI/B6 high box).

## Key question 2: CAN gateway (J533)

### Takeaway
Both cars use 7N0 907 530-family gateways; the Jetta's gateway only routes CAN and holds the installation list, so it can stay. Nobody has documented coding a Jetta gateway for a CDVC ECU; the known risk is not the gateway but the message set the CDVC ECU exchanges with the Jetta's cluster, BCM and ABS.

### Cited Findings
- **REPORTED (marketplace)** — 7N0907530AN "For VW Jetta Golf MK6"; 7N0907530AJ "Golf, Jetta, Passat, Tiguan" cross-referencing AN; 7N0907530M Golf Mk6 2009–2012; 7N0907530L CC 2.0/3.6 2011–2012; 7N0 907 530 AM 2012 Passat SE; 7N0907530T/P 2012–2015 Passat B7; 7N0907530BL is for CC/Eos/Scirocco/Passat (no Jetta); 1K0 907 530 AD is a different gateway for 2005–2014 Jetta/Golf ("part number must match exactly"); European 2016+ Passat B8 uses 5Q0 907 530 (not the NMS). — [eBay 395869643406](https://www.ebay.de/itm/395869643406); [FridayParts 7N0907530L](https://www.fridayparts.com/can-bus-gateway-control-module-7n0907530l-for-volkswagen-cc-2-0l-l4-3-6l-v6-2011-2012); [eBay seller glenlar-97](https://www.ebay.com/usr/glenlar-97)
- **VERIFIED** — Ross-Tech lists address 19 Gateway on both the Jetta 16/AJ and the Passat NMS pages without coding detail. — [Ross-Tech Jetta (16/AJ)](https://wiki.ross-tech.com/wiki/index.php/VW_Jetta_(16/AJ)); [Ross-Tech Passat (NMS/A3)](https://wiki.ross-tech.com/wiki/index.php/VW_Passat_(NMS/A3))
- **VERIFIED** — Ross-Tech's RNS310 retrofit page shows gateway revision matters on the 3C Passat ("only gateways 3C0-907-530-E or newer are known to be compatible"). — [Ross-Tech RNS310 retrofitting](https://wiki.ross-tech.com/wiki/index.php/Navigation_System_(RNS310)_Retrofitting)
- **REPORTED (forum, from precedents file)** — Mk6 Jetta gateway location and even existence as a separate box vary by trim; one SEL TDI owner claims non-GLI/non-Hybrid Jettas keep gateway duties in the BCM (unverified); advice is to read the gateway part number from a VCDS autoscan. — [VWVortex 8200257](https://www.vwvortex.com/threads/can-bus-gateway-mk-6-jetta.8200257/)

### Inferences
- **INFERRED** — Keep the Jetta GLI gateway. Its installation list already contains 01 engine; a manual car has no 02 entry, and the CDVC ECU will appear at 01 regardless of gateway coding. Fitting the Passat's gateway would import an installation list (DSG, Passat BCM variant, park assist etc.) that does not match the Jetta and would generate "missing module" faults.
- **INFERRED** — Gateway "acceptance" of the ECU is not the issue; the ECU is simply a node on powertrain CAN. The failure mode seen in the Mk6 Jetta cluster/BCM swap thread (start-then-stall, "nothing communicating with the cluster or immobilizer", [VWVortex 9547984](https://www.vwvortex.com/threads/instrument-cluster-upgrade.9547984/)) is an immobilizer/cluster pairing failure, not a gateway failure, and is the same symptom the MHH Atlas-CDVC swap thread shows (precedents file).

### Gaps
- Catalog gateway part numbers for the 2015–2018 Jetta GLI and the NMS Passat 3.6 (only marketplace numbers found).
- Any documented case of a Jetta gateway running with a CDVC ECU.

## Key question 3: Instrument cluster

### Takeaway
Keep the Jetta GLI cluster (5C6 920 973 B per forum). RPM, coolant temperature and MIL/EPC lamps arrive over CAN from the ECU, so a six-cylinder ECU needs no tach "scaling"; the real work is the Immo 4 pairing between the CDVC ECU and the Jetta cluster, or an immo-off on the ECU. A Passat cluster is the wrong answer because the Jetta cluster pinout is Jetta-specific.

### Cited Findings
- **REPORTED (forum, from precedents file)** — Mk6 Jetta cluster numbers quoted: 5C6-920-973-A (TDI), 5C6-920-973-B (GLI); lowline/midline/highline Jetta clusters believed to share pinouts and be plug-and-play once the immobilizer is coded. — [VWVortex 7050827](https://www.vwvortex.com/threads/upgrade-mkvi-jetta-tdi-instrument-cluster.7050827/)
- **REPORTED (forum, from precedents file)** — Golf Mk6 cluster plugs into a Jetta Mk6 but "won't function at all" (different pinout). — [VWVortex 7149179](https://www.vwvortex.com/threads/mk6-cluster-in-a-mk4-or-mk5.7149179/)
- **VERIFIED** — The cluster page both cars link to documents only service-interval adaptation (ESI, FIX, SID/SIA channels, PR codes QI4/QI6/QI7) and says coding information "is available while connected to the vehicle with VCDS using the Long Coding Helper"; it lists no engine-type, cylinder-count or tachometer coding. — [Ross-Tech Golf (5K) Instrument Cluster](https://wiki.ross-tech.com/wiki/index.php/VW_Golf/Golf_Plus_(5K/52)_Instrument_Cluster)
- **VERIFIED** — Ross-Tech immobilizer page (cited in the precedents file): Gen 4 covers the 1K Golf/Jetta family; "VWZ" variants adapt, "VWX"/no-serial variants use a rotating challenge and are not supported by VCDS; adapting a used Immo-4 ECU needs the car's PIN and the used ECU's PIN; dealers no longer see PINs (GeKo). — [Ross-Tech Immobilizer](https://wiki.ross-tech.com/wiki/index.php/Immobilizer)
- **VERIFIED** — Ross-Tech: erWin "offers some immobilizer solutions through authorized Pass-Thru (J2534) devices"; VCDS "cannot be used as a Pass-Thru and cannot perform most procedures on challenge-type immobilizer systems." — [Ross-Tech Official Factory Repair Information](https://wiki.ross-tech.com/wiki/index.php/Official_Factory_Repair_Information)
- **REPORTED (forum, from precedents file)** — After a Jetta Mk6 cluster + BCM swap with copied long coding, the car shut off ~1 s after start; scans showed nothing communicating with the cluster/immobilizer. — [VWVortex 9547984](https://www.vwvortex.com/threads/instrument-cluster-upgrade.9547984/)

### Inferences
- **INFERRED** — On this generation the tachometer, coolant gauge, MIL, EPC and oil-pressure warnings are CAN signals; the ECU broadcasts engine speed in rpm, so a 6-cylinder ECU drives the Jetta tach correctly. Where the Passat cluster differs (e.g., a different redline band on the dial face) is cosmetic.
- **INFERRED** — Two workable paths, in order of precedent: (1) immo-off on the CDVC ECU (vendors and prices in the precedents file), with the Jetta cluster left as-is; (2) dealer/ODIS online adaptation of the donor ECU to the Jetta's cluster, which needs both component-protection/immobilizer data and a dealer willing to adapt an engine ECU that is not listed for the VIN. The Passat cluster + Passat ECU pair (bringing the donor's immobilizer with it) is the Mk4-era trick and would require re-pinning the Jetta's cluster connector; not recommended.

### Gaps
- No published Mk6 Jetta cluster long-coding byte map (Ross-Tech defers to the Long Coding Helper).
- No documented CDVC-ECU-on-Jetta-cluster case; the only CDVC swap thread (MHH, precedents file) never resolved its start-then-stall.

## Key question 4: ABS/ESC and the XDS brake-based differential

### Takeaway
XDS was standard on the Jetta GLI from its 2012 launch through 2017 and lives in the MK60EC1 software and coding, not in the engine; keep the Jetta's ABS module and coding and XDS survives on paper. The ABS does need torque/RPM messages from the engine ECU for ASR/ESC and XDS intervention; the CDVC ECU talked to an MK60EC1 in the Passat, which is a better starting point than Ninety4co's MED9 BLV, but no swap has proven it.

### Cited Findings
- **REPORTED (press reposts)** — 2012 GLI launch material: "XDS cross differential system that debuted on the Volkswagen GTI, that helps prevent inside wheel spin during cornering"; "standard on the Jetta GLI"; uses the stability-control hardware to brake the inside wheel. — [Conceptcarz (VW release repost)](https://www.conceptcarz.com/z19472/view/canAm/canAm.aspx); [AutoGuide](https://www.autoguide.com/auto-news/2011/02/2012-volkswagen-jetta-gli-revealed-with-200-hp-and-a-proper-rear-suspension.html); [Autoblog](https://www.autoblog.com/2011/02/08/2012-volkswagen-jetta-gli-revealed-chicago-2011/)
- **REPORTED** — 2016 GLI Autobahn review: "XDS cross differential enhances handling… uses ABS to reduce understeer"; 2017 dealer copy: "XDS Cross Differential System is standard on GLI"; Davis Enterprise: XDS "seems just to apply the brakes on the inside spinning wheel", can overheat brakes on track. — [Auto123 2016 GLI](https://www.auto123.com/en/car-reviews/2016-volkswagen-jetta-gli-autobahn/63076/); [2017 dealer listing](https://communityautoconnection.record-eagle.com/tn/smyrna/volkswagen/jetta/vin-3VW2K7AJ8DM240898); [Davis Enterprise](https://www.davisenterprise.com/news/business/automotive/the-return-of-the-jetta/article_73fb355b-1747-5879-9d8b-bebf5b476f04.html)
- **VERIFIED** — Jetta 16/AJ brakes: MK60EC1 and MK70M; 2011–2012 NAR indirect TPMS runs inside the MK60EC1 (address 65 unused, reset button in glovebox). Passat NMS brakes: MK60EC1 (1K0-907-379-60EC1F.CLB). — [Ross-Tech Jetta (16/AJ)](https://wiki.ross-tech.com/wiki/index.php/VW_Jetta_(16/AJ)); [Ross-Tech Passat (NMS/A3)](https://wiki.ross-tech.com/wiki/index.php/VW_Passat_(NMS/A3))
- **VERIFIED** — MK60EC1 coding is done via SVM (long coding); copy the old module's coding; then G85 steering-angle basic setting (security code 40168), G200 lateral, G201 brake-pressure and G251 longitudinal (AWD/Hill-Hold cars) basic settings; hydraulic-unit valve basic settings only with a new/used ABS unit and DTC 00003; DTC 01486 needs an ESP function test drive. — [Ross-Tech MK60EC1](https://wiki.ross-tech.com/wiki/index.php/VW_Golf_(1K)_Brake_Electronics_(MK60EC1))
- **VERIFIED** — For the older short-coded MK60 (Golf/Jetta 1K) the engine term is part of the coding sum: +2048 for 1.4/1.6/1.6 FSI, +4096 for 1.9 TDI PD/2.0 FSI/2.0 SDI "and any car with automatic transmission", +6144 for 2.0 TDI PD; model term 0 for Golf/Jetta 1K/A3/Leon/Octavia; coding cannot be transferred from a -D to a -K or newer module. This table is for MK60, not the long-coded MK60EC1. — [Ross-Tech Golf (1K) Brake Electronics (MK60)](https://wiki.ross-tech.com/wiki/index.php/VW_Golf_(1K)_Brake_Electronics_(MK60))
- **VERIFIED** — Jetta 16/AJ tweaks: on MK60EC1 cars Hill Hold Assist can be altered via Adaptation channel 10 ("at your own risk"). — [Ross-Tech Jetta (16/AJ) Tweaks](https://wiki.ross-tech.com/wiki/index.php/VW_Jetta_(16/AJ)_Tweaks)
- **REPORTED (forum, from precedents file)** — A 4Motion donor adds ABS and yaw/pitch sensor work (not applicable to an FWD NMS 3.6). — [VWVortex 6957680](https://www.vwvortex.com/threads/product-review-oe-tuning-dyno-tune-for-med17-passat-3-6.6957680/)
- **VERIFIED (vendor page, from precedents file)** — United Motorsport swap tuning handles "deleted or missing ABS" among other swap deletes, i.e., ABS-related CAN faults are a known swap problem on VR6 swaps. — [United Motorsport swap tuning](http://unitedmotorsport.net/products/united-motorsport-swap-tuning/)

### Inferences
- **INFERRED** — The MK60EC1 long coding has engine/torque-class bytes (the short-coded MK60 already needed an engine term); a 3.6's torque curve is outside what the GLI coding describes, so ASR/ESC and XDS intervention thresholds will be mis-calibrated even if no fault is set. Expect the ESC to work but with GLI-tuned torque reduction requests that the CDVC ECU may not honour identically.
- **INFERRED** — Likely swap fault codes, by mechanism rather than precedent: ABS "engine control module implausible signal / no communication" if the CDVC's torque/RPM CAN frames differ from what the Jetta MK60EC1 expects; cluster "ABS/ESC" lamp from the same; and, because XDS/ASR request torque reduction via CAN, ESC intervention may be one-sided (brakes only). No thread documents the exact DTCs for a CDVC-in-PQ35 car.

### Gaps
- MK60EC1 long-coding byte map (engine bytes, XDS enable bit): Ross-Tech defers to SVM/Long Coding Helper.
- Whether XDS on the 2015–2018 GLI is enabled by coding bit or by part number (a VW spec sheet for MY2015–2018 was not retrieved; 2016/2017 evidence is review/dealer copy).
- Whether the NMS Passat 3.6 MK60EC1 has XDS enabled (not researched; the GLI unit stays anyway).

## Key question 5: Power steering type by Mk6 Jetta trim and year; NMS Passat 3.6; the swap-friendly recipient

### Takeaway
2011–2013 gasoline Jettas with the 2.0 8V and 2.5 (S/SE/SEL) have an engine-driven hydraulic pump (5C0 422 152 family); TDI and GLI have electromechanical steering (address 44 present, no pump). For 2014 the 1.8T SE/SEL went electromechanical while the base S 2.0 kept hydraulic; sources conflict on the 2015 S, and nothing confirms the 2016+ 1.4T. The NMS Passat moved fully to electromechanical steering for 2014. The 2015–2018 GLI has no pump, so a GLI recipient with a pump-less donor needs no steering work; a hydraulic Jetta would need a pump drive the NMS 3.6 does not have.

### Cited Findings
- **VERIFIED (vendor page)** — Urotuning sells a remanufactured hydraulic power-steering pump 5C0 422 152 J / 5C0 422 152 G titled "VW / 2.5L / Beetle / Mk6 Jetta / B7 Passat" (fitment tab collapsed). — [Urotuning 5C0422152J](https://www.urotuning.com/products/power-steering-pump-vw-2-5l-beetle-mk6-jetta-b7-passat-5c0422152j-mav)
- **REPORTED (marketplace)** — A-Premium pump replacing 5C0422152G/5C0422152H, "Jetta 2011–2013 L5 2.5L (SE or SEL Model)", Passat 2012–2014, Beetle 2012–2014, cross-ref Cardone 21-659; Cardone 21-659 on Walmart "fits 2012–2014 Passat, 2011–2013 Jetta SE"; another 21-659 listing claims "Jetta 1.8/2.0/2.5L 2011–2015". Reservoir 5C0 422 371 listed as genuine Jetta part. — [Carrefour A-Premium listing](https://www.carrefouruae.com/mafuae/en/air-compressor-power-converter/a-premium-power-steering-pump-compatible-with-volkswagen-jetta-saveiro-2011-2015-passat-2012-2014-beetle-2012-2014-crossfox-2007-2009-2011-2013-1-8l-2-0l-2-5l-replace-5c0422152g-5c0422152h/p/3233001737394); [Walmart Passat pump category](https://www.walmart.com/c/auto/volkswagen-passat-power-steering-pump); [BuyAutoParts 86-03032R (2011 Jetta SE/SEL 2.5)](https://www.buyautoparts.com/buynow/86-03032-r)
- **REPORTED** — Repair-tutorial pages show adding power-steering fluid on a 2011 Jetta S 2.5 and 2011 Jetta SE 2.5 (hydraulic). — [carcarekiosk 2011 Jetta SE 2.5](https://carcarekiosk.com/video/2011_Volkswagen_Jetta_SE_2.5L_5_Cyl._Sedan/power_steering_fluid/add_fluid)
- **REPORTED (press)** — Autobytel on the 2011 redesign: "the electric power steering was replaced with a hydraulic system." — [Autobytel 2015 Jetta road test](https://www.autobytel.com/volkswagen/jetta/2015/reviews/2015-volkswagen-jetta-road-test-review-127900/)
- **VERIFIED** — Ross-Tech lists address 44 Steering Assist (EPS_ZFLS, J500) on the Jetta 16/AJ and on the Passat NMS, with adaptation channels (curve, torque-steer compensation, Park Assist, lane assist) and a TSB note about US 2012–2014 Passat NMS pulling on flat roads; the page does not say which trims have it. Example rack part numbers on that page: 1K1 909 144 F, 1K0 909 144 P, 1K0 909 144 J (Golf). — [Ross-Tech Golf (1K) Steering Assist](https://wiki.ross-tech.com/wiki/index.php/VW_Golf_(1K)_Steering_Assist)
- **REPORTED (TSB index)** — VW tech tips list "2009–2015 Jetta, Eos, Rabbit, Golf, GTI, Passat, CC, Tiguan equipped with electromechanical power steering"; a 2014 bulletin notes the G85 sensor is in the rack on EPS cars. — [carcomplaints TSB index](https://m.carcomplaints.com/Volkswagen/Jetta/2009/tsbs); [NHTSA SB-10070364-2280](https://static.nhtsa.gov/odi/tsbs/2014/SB-10070364-2280.pdf)
- **REPORTED (press)** — 2014 Jetta: "electro-mechanical power steering, replacing the existing hydraulic setup" (lineup-level wording); 1.8T replaces the 2.5 on SE/SEL, not offered on S; whole lineup gets IRS. — [cars.com, 2014 Jetta what's changed](https://www.cars.com/articles/2014-volkswagen-jetta-whats-changed-1420663061543); [AutoGuide 2014 pricing](https://www.autoguide.com/auto-news/2013/09/2014-volkswagen-jetta-priced-from-17540.html)
- **REPORTED (press)** — 2014: "electric assist now replaces the hydraulic rack and pinion in all Jettas except for the base S model"; CarGurus: EPS "on all but the base variant (which keeps the old hydraulic steering system)"; HeraldNet: hydraulic steering "on 1.8T models" swapped for electric assist. — [TFLcar 2014 Jetta 1.8T](https://tflcar.com/?p=43231); [CarGurus 2014 Jetta](https://jobs.cargurus.com/research/2014-Volkswagen-Jetta-c24142); [HeraldNet](https://www.heraldnet.com/?p=452589)
- **REPORTED (conflicting)** — 2015 Jetta S 2.0: a Reddit commenter says "2015 S has hydraulic power steering"; a dealer printout for a 2015 Jetta 2.0L S lists "Electric Power steering". — [r/jetta thread (mirror)](https://cal1.lr.ggtyler.dev/r/jetta/comments/1gs304l/power_steering_fluid); [dealer listing 2015 Jetta 2.0L S](https://www.vwleessummit.com/used-Lees+Summit-2015-Volkswagen-Jetta-20L+S-3VW2K7AJ7FM332541)
- **REPORTED (weak)** — A repair-tutorial page says the 2017 Jetta S 1.4T uses electric power steering. — [carcarekiosk 2017 Jetta S 1.4T](https://carcarekiosk.com/video/2017_Volkswagen_Jetta_S_1.4L_4_Cyl._Turbo/power_steering_fluid/add_fluid)
- **REPORTED (Wikipedia-derived)** — NMS Passat: "The 2014 Passat also now uses electro-mechanical steering, instead of the previous hydraulic setup." — [HandWiki, Volkswagen Passat NMS](https://handwiki.org/wiki/Engineering:Volkswagen_Passat_NMS)
- **REPORTED (forum, from precedents file)** — Mk4-era 3.6 swap advice: "a 24V accessory bracket is needed to keep power steering" on a 3.6 (the FSI 3.6 accessory drive has no pump position). — [precedents_vendors_salvage.md](/home/user/vr6_jetta/research_notes/Mk6%20Jetta%20CDVC%20VR6%20swap%20parts/precedents_vendors_salvage.md)
- **REPORTED (local baseline)** — Ninety4co's GTI E-box front feeds include an 80 A "power steering" pole (the EPS rack feed on a Mk6 GTI). — [ninety4co-swap-wiring-repins.md](/home/user/vr6_jetta/research/sources/ninety4co-swap-wiring-repins.md)

### Inferences
- **INFERRED** — Trim/year matrix for NAR Mk6 Jettas: 2011–2013 2.0 8V (S) and 2.5 (S/SE/SEL/Sportwagen): hydraulic pump 5C0 422 152 x; 2011–2018 GLI (2.0T) and 2011–2015 TDI (and Hybrid): electromechanical (address 44); 2014–2018 1.8T SE/SEL/Sport: electromechanical; 2014 S 2.0 8V: hydraulic (three press sources); 2015 S 2.0: unresolved (one forum vs one dealer sheet); 2016–2018 S 1.4T: probably electromechanical (the 2.0 8V and its pump left with the 1.4T launch) but unproven. The 2012–2014 Passat pump listings (Cardone 21-659) match the 2.5L Passat, which is consistent with the Passat 2.5 being the hydraulic car and the 2014 1.8T change making the whole NMS line electromechanical.
- **INFERRED** — The 2012–2013 NMS 3.6: the pump listings cover the 2.5 only, and the 3.6 FSI accessory drive is the same pump-less layout as the B6 3.6 (Ninety4co needed no pump), so the NMS 3.6 was almost certainly electromechanical from 2012; the HandWiki sentence refers to the remaining hydraulic (2.5) cars. This is reasoning, not a spec sheet.
- **INFERRED** — Swap-friendly recipient: a 2015–2018 GLI (electromechanical, 80 A EPS feed already in the E-box, EA888 Gen3 MED17 harness, 02Q manual). A 2011–2013 2.5 S/SE/SEL would lose steering assist unless a pump is adapted to the 3.6 (no known OEM bracket; B6/NMS 3.6 never had one).

### Gaps
- No VW spec sheet or owner's-manual page was retrieved to settle the 2015 Jetta S 2.0 and 2016–2018 1.4T S steering type; the EPS rack part number for the Jetta Mk6 (5C0/5C1/5C2 909 144 family would be the expected prefix) was not found and is not asserted.
- No catalog fitment list for the hydraulic pump 5C0 422 152 J/G/H by Jetta trim (Urotuning's tab is collapsed; the other listings are aftermarket).
- NMS Passat 3.6 steering rack part number: not found.

## Key question 6: Body harness and ECU body-side connector

### Takeaway
No published body-side pinout for the CDVC (03H 906 026 x, MED17.1.6x) or the Jetta GLI (MED17.5.x) ECU was found; the only connector-level data is Ninety4co's MED9 BLV sheet and a partial MED9.1 T94 table for the B6 Passat 2.0T. The circuit groups that move are known from his sheet; the pins must come from erWin diagrams for both VINs.

### Cited Findings
- **REPORTED (local baseline)** — Ninety4co's T94 moves for BLV into a Mk6 GTI: fan module T94/50→28; coolant temp T94/36→26; LDP T94/49→8 and 44→40 (LDP/3 ground); cruise T94/45→18 (unverified); brake switch T94/19→25; fuel pump module T94/30→27; low fuel-pressure sensor T14/7→T94/35; GTI O2 pins 34/62/29/56/57/78/79/73 removed and bank 1/bank 2 sensors re-pinned to 51/61/82/81/60 and 73/83/59/84/62; GTI MAF pins 23/65 removed, 3.6 MAF on 13/22/64/42; throttle pedal all six pins moved (81→58, 82→80, 35→78, 83→79, 11→56, 61→57); fuse-box: terminal 30/15, connection 87, ECM relays 1 and 2, after-run pump relay, ignition-coil and O2-heater 12 V feeds and LDP pin 3 all re-routed, mostly onto the T26 connector. — [ninety4co-swap-wiring-repins.md](/home/user/vr6_jetta/research/sources/ninety4co-swap-wiring-repins.md)
- **REPORTED (transcript)** — Ninety4co, Part 4: "all of your relay triggers on the T94 are going to have to be moved to how they would be on the Passat"; headlights, impact sensors, fog lights, ambient temp sensor stay. — [part4 transcript](/home/user/vr6_jetta/research/transcripts/part4-wiring-final-assembly-first-drive.md)
- **REPORTED** — A partial T94 table exists for the B6 Passat Bosch MED9.1 ECU 3C0 907 115 F (2.0T FSI), not for MED17. — [rusefi wiki, Passat B6](https://wiki.rusefi.com/VolkswagenPassatB6/)
- **VERIFIED (vendor page, from precedents file)** — Stance Dubs requires the donor's body harness (at least the whole engine-bay portion) "because the second ECU connector is one with the harness", i.e., the body-side ECU connector belongs to the body harness, not the engine harness. — [precedents_vendors_salvage.md](/home/user/vr6_jetta/research_notes/Mk6%20Jetta%20CDVC%20VR6%20swap%20parts/precedents_vendors_salvage.md)
- **VERIFIED** — NMS Passat 3.6 was DSG-only in North America. — [Wikipedia, Passat (North America and China)](https://en.wikipedia.org/wiki/Volkswagen_Passat_(North_America_and_China))

### Inferences
- **INFERRED** — Circuits that must be re-mapped from the Jetta GLI harness to CDVC expectations, by function (same list as Ninety4co's, with Gen3-specific additions): power distribution (terminal 30/15, ECM main relay J271, ECM relay 2, connection 87); fuel pump control module J538 PWM/enable and low-pressure sensor G410; brake light/brake test switch F/F47 (Jetta Gen3 uses a single CAN-less switch feeding the ECU); clutch pedal switch F36 (Jetta manual only, no DSG donor equivalent; needed for cruise cancel and start interlock); cruise stalk (via steering-column module over CAN on both cars; Ninety4co's cruise pin stayed unverified); EVAP LDP (the 3.6 FSI uses a leak-detection pump, the EA888 Gen3 uses an NVLD/no pump, so these are new wires); after-run coolant pump V51 and its relay (new circuit; the Gen3 GLI has an electric coolant pump of a different kind); fan control module J293 PWM line and 50 A feed; four O2 sensors on two banks (eight heater/signal pins plus bank-2 heater 12 V); MAF G70 (Gen3 GLI has no MAF; the 3.6 does); accelerator pedal G79/G185 six pins (both drive-by-wire, pinout differs); coolant temp G62. Everything body-side (lighting, airbags, HVAC, BCM) stays.
- **INFERRED** — Because the CDVC never saw a clutch switch or a manual gearbox, the swap tune must disable the TCU-present checks and provide a manual-car cruise/starter logic; Ninety4co's BLV had a manual-equipped B6 sibling (RoW), which the CDVC does not.
- **INFERRED** — Bridge connector: the Mk6 GTI's T14 engine/body bridge is a Golf detail; whether the Jetta GLI and the NMS Passat have an equivalent, and whether their connector counts match, is only answerable from erWin's "fitting locations" documents.

### Gaps
- No published CDVC (03H 906 026 x) body-side pinout; no published Jetta GLI CPLA/CPPA (06K 907 425 x) body-side pinout; no confirmation that both use a 94-pin body connector.
- Whether MED17.1.6x and MED17.5.x share Bosch connector housings (would allow a pin-for-pin re-populate of the Jetta's existing body-side plug).

## Key question 7: Charging and starting

### Takeaway
The CDVC alternator part number and rating could not be found in any catalog this run; the MED9-era 3.6 used a 140 A 06F 903 023 x unit (Ninety4co: 06F 903 023 F). The starter stays with the 02M (Valeo 438152) and needs a manual-car interlock the CDVC software never had. Battery stays in the Jetta's engine bay unless the airbox dictates otherwise.

### Cited Findings
- **REPORTED (local baseline)** — Ninety4co: 3.6 alternator 06F 903 023 F; Mk4 02M starter Valeo 438152; battery relocated to the trunk with a circuit breaker (pre-existing, not swap-required); E-box pole 1 = alternator charge-back 150 or 200 A solid maxi-fuse. — [ninety4co-swap-parts-list.md](/home/user/vr6_jetta/research/sources/ninety4co-swap-parts-list.md)
- **VERIFIED (vendor page)** — FCP Euro Passat alternators: 06F 903 023 P SEG 140 A for "Eos, Passat, A3, TT Quattro, A3 Quattro…" (Valeo and Bosch reman versions list "A3 Quattro, CC, Eos, Passat, R32, TT Quattro", i.e., the PQ35 VR6/2.0T FSI family); 06K 903 023 G Valeo 150 A "Jetta, Beetle, Passat" (EA888 Gen3 family); 06K 903 024 E SEG 140 A "Beetle, Passat, Jetta"; 07K 903 023 C SEG 140 A "Passat, Beetle, Jetta" (2.5L family); 03L 903 023 R Bosch 180 A "Passat" (TDI). None is labelled 3.6/CDVC. — [FCP Euro Passat alternators](https://www.fcpeuro.com/Volkswagen-parts/Passat/Alternator-Unit/)
- **REPORTED (forum, from precedents file)** — G60ING's R36 Corrado thread: "140 A Passat 3.6 alternator" (B6 BLV). — [VWVortex 8028002](https://www.vwvortex.com/threads/3-6-24v-vr6-swap-questions-and-links.8028002/)
- **VERIFIED** — NMS Passat 3.6 was DSG-only; no factory clutch-switch logic exists for the CDVC in NAR. — [Wikipedia, Passat (North America and China)](https://en.wikipedia.org/wiki/Volkswagen_Passat_(North_America_and_China))

### Inferences
- **INFERRED** — The Jetta GLI's charge cable, 150/200 A alternator maxi-fuse and E-box feeds are sized for a 140–150 A EA888 alternator; a 140 A VR6 alternator needs no cable upgrade. If the CDVC alternator turns out to be a different (e.g., 180 A) unit, re-check the maxi-fuse value against the donor's.
- **INFERRED** — Starter: the 02M starter is energised by the ECU-controlled starter relay chain on this generation (terminal 50 via the BCM/ECU); the CDVC ECU expects a DSG "P/N" permission over CAN that a manual car cannot provide, so the swap tune or a hard-wired clutch-switch interlock must replace it. Ninety4co's BLV (MED9) had the same issue solved by Reflect's swap file.

### Gaps
- CDVC (2012–2018 NMS) alternator part number and amperage: searched 06E/03H/03G 903 023 families and FCP's Passat list with no 3.6 result; needs an ETKA/erWin VIN lookup.
- Battery location/cable sizes for the NMS Passat vs Jetta Mk6: not researched this run (both are engine-bay batteries in my recollection, but no source was fetched, so treat as unverified).

## Key question 8: Cooling-fan control, after-run pump and coolant sensors

### Takeaway
Both cars use PWM fan assemblies with the control module built into the fan frame (1K0 959 455 x family on the Jetta); Ninety4co ran the BLV on the stock Mk6 GTI fans after moving one ECU pin and feeding the module 50 A. The NMS 3.6 fan assembly number was not found. The after-run pump (1K0 965 561 B) and its relay are a new circuit on any 4-cylinder Jetta.

### Cited Findings
- **REPORTED (local baseline)** — Ninety4co kept the stock Mk6 fans and A/C condenser; moved the fan-module ECU pin T94/50→T94/28; E-box pole 3 "coolant fan module 50 A"; after-run pump 1K0 965 561 B; coolant temp sensor pin T94/36→26. — [ninety4co-swap-parts-list.md](/home/user/vr6_jetta/research/sources/ninety4co-swap-parts-list.md); [ninety4co-swap-wiring-repins.md](/home/user/vr6_jetta/research/sources/ninety4co-swap-wiring-repins.md)
- **REPORTED (marketplace)** — Jetta Mk6 fan assemblies by aftermarket cross-reference: 1K0959455ES "2014–2015 Jetta 1.8L, 2016 Jetta 1.4L"; 1K0959455P "2011–2013 Jetta SE, 2016–2017 Jetta S"; 1K0959455EA interchange 2005–2017. — [Walmart Cooling Direct listing](https://www.walmart.com/ip/690639336); [Walmart listing](https://www.walmart.com/ip/1995278227)
- **REPORTED (marketplace)** — Fan control module cross-references 1K0959455N / 3C0959455F / 1K0959455DT / 1K0959455FJ / 1K0959455FR for Golf/GTI/Jetta/A3/TT; listing warns to match fan-motor amperage to the module. — [eBay 306298450245](https://www.ebay.de/itm/306298450245); [ManoMano module listing](https://www.manomano.de/p/nouveau-module-de-refroidissement-de-radiateur-unite-de-commande-du-ventilateur-de-refroidissement-pour-audi-a3-tt-cc-golf-r32-qaq-223512803)
- **REPORTED (local baseline)** — Cooling hoses for an OEM-style 3.6 system are "the same as a 2018 Passat GT" (Ninety4co), i.e., the NMS 3.6 cooling layout is the reference. — [ninety4co-swap-parts-list.md](/home/user/vr6_jetta/research/sources/ninety4co-swap-parts-list.md)

### Inferences
- **INFERRED** — The Jetta GLI fan assembly (1K0 959 455 family with integrated J293) is electrically compatible with the CDVC: same PWM-command interface the BLV used on the GTI fans. Verify the fan motor wattage class against the Passat 3.6 (a 2.0T GLI fan may be a lower-power class than a V6's); the module/motor amperage warning above applies.
- **INFERRED** — The EA888 Gen3 GLI has an ECU-controlled electric coolant pump (not an after-run pump in the VR6 sense) and no LDP, so the after-run pump relay/feed and the LDP are added circuits, exactly as on Ninety4co's GTI. Coolant temp sensor G62 is a plain NTC on both ECUs; only the ECU pin changes.

### Gaps
- NMS Passat 3.6 fan assembly and fan-control-module part numbers (search found only CC 3.6 and 2.5 Passat references); whether its motor power class differs from the GLI's.
- Jetta GLI fan assembly part number per catalog (only cross-reference numbers found).

## Key question 9: Factory wiring diagrams: erWin options and the Mitchell/AllData caveat

### Takeaway
North American VW erWin now lives at vw-us.erwin-store.com; it sells timed "Info medium" access (repair manuals, wiring diagrams, TSBs, SSPs, PDF repair guides) and separate ODIS diagnostic time. Current prices are behind the login; the most recent third-party figure is $35 for one day and $1,500 for a year (2023), with downloaded PDFs kept afterwards. Ninety4co used VIN-specific factory diagrams for both cars (~$50 for 24 h at the time) and found Mitchell/AllData/ProDemand had wrong pin numbers, wrong wire colours and missing information.

### Cited Findings
- **VERIFIED** — erwin.vw.com redirects (301) to https://vw-us.erwin-store.com/erwin/; the home page says erWin "contains all published service information from Volkswagen Group of America"; the subscription comparison lists "Info medium" (vehicle identification by make/model/year, repair manuals, maintenance charts, wiring diagrams, body repair, OBD II documents, campaigns/recalls, technical bulletins, vehicle data, self-study programs/videos, model-specific repair guides as PDF; starts with purchase, ends when purchased time expires) and "ODIS" (vehicle diagnostics, GeKo/SVM during an active session; "an interruption of the flat rate is not possible"). Prices are not shown without login. — [erWin VW US home](https://vw-us.erwin-store.com/erwin/showHome.do); [erWin subscription comparison](https://vw-us.erwin-store.com/erwin/showSubscriptionComparison.do)
- **VERIFIED** — Ross-Tech lists the NAR erWin sites (VW, Audi, Bentley, Lamborghini) and says erWin includes repair manuals, wiring diagrams and TSBs, with immobilizer solutions via authorized J2534 pass-thru; it also links a forum thread with videos on reading current-flow diagrams and notes Bentley SSPs "are not a substitute for factory repair manuals." — [Ross-Tech Official Factory Repair Information](https://wiki.ross-tech.com/wiki/index.php/Official_Factory_Repair_Information)
- **REPORTED (2023 blog)** — VW erWin: one day $35, one year $1,500; "once that information is downloaded we can access it in the future as well, without needing to buy a new subscription." — [IDParts blog](https://idpartsblog.com/2023/04/21/find-vw-repair-manual-online/)
- **REPORTED (undated guide)** — Audi erWin: $35/1 day, $60/3 days, $250/month, $2,000/year (Audi, not VW). — [Rick's Free Auto Repair Advice](https://ricksfreeautorepairadvice.com/get-car-wiring-diagram/)
- **REPORTED (local analysis of Ninety4co Part 4)** — "Use factory VW ElsaWeb wiring diagrams (about $50 for 24-hour access), VIN-specific for both cars… Mitchell/AllData/ProDemand had wrong pin numbers, wrong colours and missing info"; transcript: "I did run into several instances where pin numbers were wrong and wire colors were wrong and some info is just flat out missing. The Elsa diagrams are going to have all that." — [ninety4co-vr6-mk6-swap-series.md](/home/user/vr6_jetta/research/ninety4co-vr6-mk6-swap-series.md); [part4 transcript](/home/user/vr6_jetta/research/transcripts/part4-wiring-final-assembly-first-drive.md)

### Inferences
- **INFERRED** — Budget two one-day erWin purchases (recipient VIN and donor VIN), downloading the full wiring-diagram set, "fitting locations" (connector/ground/bridge locations) and the component-location documents for both cars in one session each; that is where the Jetta's E-box connector population, the T-connector between engine and body harness, and the ECU body-side pinouts actually live.

### Gaps
- Current erWin NAR hourly/daily/yearly prices (login required); whether an hourly option exists in the US store.

## Donor-vs-recipient electrical parts list (summary for the report writer)

Labels apply to the reasoning behind each line; part numbers are only those cited above or in the baseline files.

| Item | From donor (NMS Passat 3.6) | Stays Jetta GLI | Label / notes |
|---|---|---|---|
| Engine ECU (Bosch MED17.1.6x, 03H 906 026 x family) with engine harness | Yes | — | VERIFIED family number (Atlas), INFERRED for NMS; needs immo-off or pairing (precedents file) |
| Engine-bay E-box carrier with harness tail and engine-harness connectors | Yes (recommended) | Possibly, if erWin shows the GLI box carries the needed connectors | INFERRED; Ninety4co precedent used the donor-type box (1K0 937 124 K for B6) |
| CAN gateway J533 (7N0 907 530 x) | No | Yes | INFERRED; REPORTED same family on both cars |
| Instrument cluster (GLI 5C6 920 973 B per forum) | No | Yes | REPORTED PN; INFERRED CAN tach/temp; immobilizer handling required |
| BCM, airbag, HVAC, lighting, body harness | No | Yes | VERIFIED same generation (Ross-Tech) |
| ABS/ESC MK60EC1 with XDS | No | Yes | VERIFIED module; INFERRED XDS survives; torque-class mismatch |
| Steering (electromechanical rack, 80 A EPS feed) | No | Yes (GLI) | INFERRED; hydraulic 2.5/2.0 Jettas lose assist |
| Alternator | Yes (CDVC unit; PN not found) | — | REPORTED 140 A on MED9 3.6 (06F 903 023 F); GAP for CDVC |
| Starter | Mk4 02M Valeo 438152 (with the 02M) | — | REPORTED (baseline) |
| Fan assembly with J293 | No | Yes, verify motor class | REPORTED Ninety4co precedent; INFERRED |
| After-run pump 1K0 965 561 B + relay, LDP, bank-2 O2 feed | Yes (new circuits in Jetta harness) | — | REPORTED (baseline) |
| Accelerator pedal | Keep Jetta pedal, re-pin six wires | Yes (hardware) | REPORTED (baseline; both drive-by-wire) |
| Fuel pump control module J538 and 4.0 bar regulator/filter | Passat module 3C0 906 093 A per Ninety4co; verify for NMS | — | REPORTED (baseline) |
| Clutch switch / manual interlock logic | — | Jetta switch; ECU logic must come from swap tune | INFERRED (CDVC DSG-only, VERIFIED) |
| Wiring diagrams | erWin, donor VIN | erWin, recipient VIN | VERIFIED source; REPORTED pricing |

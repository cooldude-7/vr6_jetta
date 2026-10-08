# Manual-transmission path for a 3.6 VR6 (CDVC) in a 2015–2018 Mk6 Jetta GLI: the Mk4 24V 02M, its clutch, hydraulics, differential and the alternatives (VR6-pattern 02M/02Q 4Motion, Passat 02E DSG)

Research date: 2026-10-08. Scope: North American vehicles only. Baseline already documented locally and cross-referenced, not repeated: Ninety4co's BLV + Mk4 24V 02M swap into a 2010 Mk6 GTI (`/home/user/vr6_jetta/research/sources/ninety4co-swap-parts-list.md`, `/home/user/vr6_jetta/research/ninety4co-vr6-mk6-swap-series.md`) and the DSG/vendor/salvage findings in `precedents_vendors_salvage.md` (same folder as this file).

Labels: **VERIFIED** = parts-catalog fitment data, factory document or vendor product page actually opened; **REPORTED** = forum/build thread, or vendor/catalog text seen only in a search snippet (page not opened); **INFERRED** = my reasoning from the cited material. No part number below is invented; where I could not source one it is listed under Gaps.

Access notes: vwvortex.com now redirects automated fetches to a "tollbit" gateway and the curl retry returned an HTTP 202 challenge page, so every VWVortex item is REPORTED from search-engine summaries. bar-tek.com's steel-fork page returned 404 on fetch; its content is REPORTED from snippets. YouTube not used.

---

## Key question 1: Bellhousing patterns, and which North American gearboxes bolt to a 3.6

### Takeaway
No source gives a drawing of the VR6 bellhousing pattern, but the practical evidence is consistent and strong: a Mk4 24V VR6 02M bolts straight to a 3.6 (done, running, Ninety4co), VR6 blocks of all displacements take the same side engine mount, and every VR6 manual box VW/Audi sold here is a 6-cylinder-specific housing. The GLI's own 02Q is a 4-cylinder (EA888, 8-bolt flywheel) box and does not fit. In NA the only front-drive VR6-pattern manual is the 2002.5–2005 Mk4 24V 02M; the Mk4 R32 (2004) and Mk2 TT 3.2 quattro (2008–09) 02Ms are VR6-pattern but 4Motion, and a 4Motion 02M can be converted to FWD with an off-the-shelf adapter kit.

### Cited Findings
- **REPORTED (build, running car)** — Ninety4co: the 24V VR6 02M "will bolt right up" to the 3.6 (BLV) using the Mk4 24V clutch/flywheel application; his car ran and drove on this combination. — [local series notes](/home/user/vr6_jetta/research/ninety4co-vr6-mk6-swap-series.md) (Part 2, 2:02)
- **VERIFIED (vendor article, FCP Euro)** — Flywheel/crank bolt patterns differ by engine family: "VR6 powered cars... have a 10-bolt crank, while 4-cylinder 1.8t models... have a 6-bolt crank"; the 2.0T TSI clutch "uses an 8-bolt flywheel". The 02Q has "some small changes in the bellhousing design and spacing," so an 02M clutch/flywheel kit won't fit an 02Q. — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **VERIFIED (vendor article, FCP Euro)** — North American 02M applications: 2001–2006 Audi Mk1 TT 225 quattro; 2002 GTI 337; 2003 GTI 20th Anniversary; **2004 Golf R32**; **2002.5–2005 Golf GTI 24v VR6**; **2002.5–2004 Jetta GLI 24v VR6**; 2004.5–2005 Jetta GLI 1.8t; 2008–2009 Audi Mk2 TT 2.0t FrontTrak; **2008–2009 Audi Mk2 TT 3.2 VR6 quattro**; 2007–2013 Audi A3 2.0t FrontTrak. 02Q applications include 2006–2009 Mk5 GTI/GLI 2.0t, 2010–2014 Mk6 GTI 2.0t, **2012–2018 Mk6 Jetta GLI 2.0t**, 2015–2020 Mk7/7.5 GTI, 2019–2020 Mk7 GLI, 2007–2010 Eos/Passat 2.0t, 2009–2016 CC 2.0t and the TDIs. No VR6 is listed under 02Q. — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **VERIFIED (vendor fitment list, already in precedents file)** — BFI's Mk5/Mk6 6-cylinder side engine mount fits 1999.5–2005 Golf/Jetta 2.8, 2004 R32, 2008 R32, 2005–2014 Passat 3.2/3.6 and 2003–2006 TT 3.2, i.e. the external block geometry is shared across 24V, 3.2 and 3.6. — [BFI Stage 1](https://blackforestindustries.com/products/bfi-mk5-mk6-engine-mount-6-cylinder-stage-1) (cited in `precedents_vendors_salvage.md`)
- **REPORTED (VWVortex snippets, from precedents file)** — "VR6 engines need VR6-specific bellhousings which themselves vary slightly"; "a 1.8T-pattern 02M will not work" on a 3.6; another thread argues automatic and manual VR6 blocks differ. — VWVortex threads cited in `precedents_vendors_salvage.md` (Key question 1)
- **VERIFIED (vendor page, Epytec)** — Epytec's "6 Speed Manual Gearbox Conversion Kit 02M 4motion VR6 R32" (article 698) converts a 4Motion 02M/02Q to front drive: remove the angle drive and the "toothed ring bearing", fit the adapter plate, press in sealing ring **02M 409 189**, fit drive-shaft flange **02M 409 356 A**, use the shorter **02M 2WD bolt** (4WD bolts are "too long"), medium-strength threadlocker; the plate also "seals the oil line that is normally open for the angle drive"; nothing on the gearbox is modified so it can be reverted. The guide cites VR6 and 1.8T applications generally; it does not name TT 3.2 or A3 3.2. — [Epytec install guide](https://epytec.de/en/blog/einbauanleitung-fuer-artikel-698-02m-umruesten-fuer-einbau-in-frontangetriebene-fahrzeuge-z.b-vr6-umbau-auf-02m-getriebe); [Epytec kit 698](https://epytec.de/en/6-speed-manual-gearbox-conversion-kit-02m-4motion-vr6-r32-golf-mk1-2-3-4-turbo-698)
- **REPORTED (eBay listing title only)** — "Golf R32 VR6 6 speed 02M gearbox conversion for 2WD front-wheel drive AL0090": a second commercial 4Motion-to-FWD adapter exists. — [eBay 172006056770](https://www.ebay.com/itm/172006056770)
- **REPORTED (vendor snippet, Epytec)** — "the 6-speed gearbox can be easily coupled with all current VW VR6 engines" (02M 4Motion R32 kit text). — [Epytec kit 698](https://epytec.de/en/6-speed-manual-gearbox-conversion-kit-02m-4motion-vr6-r32-golf-mk1-2-3-4-turbo-698)
- **REPORTED (factory SSP via search summary; PDF not opened)** — VW Self-Study Programme 205 "6-speed manual gearbox 02M": the 150 kW VR6 column lists pinion-set finals 4.200 and 3.316; FWD box 48.5 kg vs 68 kg with angle drive (4WD). — [SSP 205 PDF](https://www.volkspage.net/technik/ssp/ssp/SSP_205.pdf)

### Inferences
- **INFERRED** — The 12V/24V/3.2/3.6 VR6 family shares one bellhousing pattern: a 24V 02M bolts to a BLV 3.6 (done), the same side mount fits 2.8/3.2/3.6 blocks, and R32 DSGs are reported to bolt to 3.6s (precedents file). The CDVC (NMS 3.6) is the same EA390 block family as the BLV, so the 02M should bolt to it the same way; nobody has documented a CDVC + 02M yet, so verify by trial fit of the box and starter before buying a clutch.
- **INFERRED** — The GLI's 02Q is useless for this swap (4-cylinder housing, 8-bolt TSI flywheel) but its chassis-side parts are not: shift box/cables, pedal, master cylinder and axles are the parts to try to keep (see Key questions 4, 6, 7).
- **INFERRED** — In NA the front-drive VR6 02M exists only in 2002.5–2005 GTI 24V and 2002.5–2004 GLI 24V (roughly a three-model-year, low-volume population, now 20+ years old). The 2004 R32 02M and 2008–09 TT 3.2 02M are the VR6-pattern fallbacks; both are 4Motion and need the Epytec/AL0090-type FWD conversion, both carry shorter (R32-type ~4.2/3.3) finals than the FWD 24V box, and the TT 3.2 box has the PQ35 3-bolt mount pattern (Ninety4co). Euro Mk5 R32 / A3 3.2 / TT 3.2 manual 02Qs were never sold here and are out of scope.
- **INFERRED** — The SSP 205 "150 kW VR6" 4.200/3.316 pair is the Euro Golf 4 V6 4Motion box, not the NA FWD 24V box (whose finals are 3.94/3.09 per Key question 2).

### Gaps
- No factory drawing or dimensioned pattern for the VR6 vs 4-cylinder bellhousing was found; the conclusion rests on precedent and fitment lists.
- Gearbox code letters for the 2004 R32 (NA) and Mk2 TT 3.2 02Ms were not sourced here.
- Whether any 02Q (as opposed to 02M) exists in VR6 pattern could not be verified; FCP Euro's NA list shows none.

---

## Key question 2: The Mk4 24V 02M itself: codes, ratios, torque rating, mount pattern, weaknesses, price, rebuild items, fluid

### Takeaway
The FWD 24V 02M is a dual-final-drive box (3.94 for 1st–4th, 3.09 for 5th–6th per the VW press figures quoted on VWVortex) rated by VW at 258 lb-ft, which is exactly the CDVC's 258 lb-ft / 350 Nm; vendors say it survives 350–400 lb-ft if driven cleanly. Known weak points are the brass-padded multi-piece shift forks (1-2 and 3-4), input-shaft bearing play, 2nd/3rd synchros and the open diff. A used box cost Ninety4co $400 including steel forks; budget forks (if not already fitted), input and axle seals, ~2.5 L of GL4 75W-80/90, and consider the LSD while the case is split.

### Cited Findings
- **VERIFIED (vendor article)** — MQ350 factory rating "258 lb-ft"; the boxes are "easily handling 350-400 lb-ft, provided that the driver is not unnecessarily rough." — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **REPORTED (VWVortex via search summary; thread blocked)** — "Dual final ratios for 6-speed VR6 GLi/GTi": VW press material gives final ratio #1 **3.94:1** and #2 **3.09:1**; ETKA lists the transmission as "71/18/23"; one reply places 3.94 on 1st–4th and 3.09 on 5th–6th; 24V set quoted as 3.36 / 2.09 / 1.47 / 1.15 / 1.19 / 0.98, reverse 3.99. — [VWVortex 1018005](https://www.vwvortex.com/threads/dual-final-ratios-for-6-speed-vr6-gli-gti.1018005/)
- **REPORTED (forum ratio list via search summary)** — vwforum "02m six speed": code **FSR** labelled VR6 with 3.357 / 2.087 / 1.469 / 1.150 / 1.194 / 0.975; code **EDJ** also labelled VR6 (4th–6th match SSP 205's 150 kW column, 1st does not); FML / FZQ / ERR listed as 1.8T boxes (FML said to be from a 2003 20th AE GTI). — [vwforum 73218](https://www.vwforum.com/threads/02m-six-speed.73218/)
- **REPORTED (VWVortex via search summary)** — The R32's 02M uses a 4.2 final for 1st–4th. — [VWVortex 394951](https://www.vwvortex.com/threads/02m-transmission-ratios.394951/)
- **REPORTED (vendor guide, flagged inconsistent by the search summary)** — RWC Motorsport's Mk4 transmission guide gives the 02M final as 3.389 in one table and 3.647 in another; do not rely on it. — [RWC Motorsport](https://www.rwcmotorsport.com/transmissions.php)
- **REPORTED (build)** — Ninety4co's Mk4-sourced FWD 02M has a **2-bolt** transmission-mount pattern and used the PQ35 2.5L 5-speed / 09G mount **1K0 199 555 AP** unmodified; a Mk2 TT 3.2 02M has the **3-bolt** PQ35 pattern and would take a Mk5/6 6-speed mount instead. — [local parts list](/home/user/vr6_jetta/research/sources/ninety4co-swap-parts-list.md) (rows 2, 10)
- **REPORTED (build)** — Price: FWD 24V 02M bought on Facebook Marketplace for **$400 including OEM steel shift forks**; he still did input-shaft and axle seals, and the first seals he bought were the wrong size (he does not say which he ordered, nor the correct numbers). — [local series notes](/home/user/vr6_jetta/research/ninety4co-vr6-mk6-swap-series.md) (Part 2)
- **VERIFIED (vendor article)** — Weak points: "soft brass shift forks bending due to aggressive shifting or a missed shift", 1-2 and 3-4 forks most affected; synchro trouble "most common... with second and third gear", rare on 1/4/5/6; "All variations... can suffer from excessive play on the input shaft"; "the open differential is a weak link for vehicles making substantially more power than stock"; leaks "typically only seen on very high mileage (over 200K) units". 02M uses taper input-shaft bearings, 02Q ball bearings; late 02M and 02Q have an access window so forks can be done without splitting the case; early 02Qs had multi-piece brass/steel forks, later ones "one-piece steel forks from the R32". — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **REPORTED (vendor snippets; page 404 on fetch)** — Bar-Tek "02M & 02Q Upgrade Gear Shift Fork Kit": three forks, welded instead of the OEM riveted assembly; "VW uses shift forks with problematic brass parts. Under enthusiastic use brass forks can and do break", leaving the car stuck in gear; fitment list shows 3.2 VR6 codes BDB, BMJ, BUB, CBRA (no 2.8 codes seen in the snippet). Price not captured. — [Bar-Tek forks](https://bar-tek.com/02m-02q-upgrade-steel-shift-forks)
- **REPORTED (vendor snippet)** — Bar-Tek also sells a "4th gear support" and calls 4th "the biggest weakness of the 02m gearboxes": high torque pushes the gear pair out of mesh. — [Bar-Tek 4th gear support](https://bar-tek.com/transitional-support-4th-gear-transmission-02m-02q)
- **REPORTED (forum anecdote)** — An 02M owner found the main ball bearing had spun in the aluminium case ("a very common problem with 02M gearboxes"); fix was machining the case, shims, Loctite 620 and grub screws. — [SEAT Cupra forum](https://www.seatcupra.net/forums/goto/post?id=4839300)
- **REPORTED (vendor snippet)** — HPA's 02M-to-MQ500 conversion page: the MQ500 has 3 pinions vs 2 in the 02M/02Q, "resulting in higher torque capacity" (sales claim). — [HPA](https://www.hpamotorsports.com/products/02m-to-mq500-conversion)
- **VERIFIED (vendor article)** — Fluid: "VW specifies a GL4-spec oil"; GL5 "generally not recommended for synchronized transmissions"; factory fill "a straight 75W"; 75W-80 and 75W-90 are the popular replacements (Liqui Moly 75W-90 GL4 full synthetic, no. 20012 named); "a refill will typically take around 2.5 liters"; "lifetime" fill but best results changing ~50,000 miles. — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **REPORTED (vendor snippet)** — Pro Race Engineering (UK) sells a "02M R32 VR6 Built Gearbox + 3-6 Carbon Synchro Kit", i.e. built 02Ms with carbon synchros exist as a product category. — [Pro Race Engineering](https://prorace-engineering.co.uk/product/02m-r32-vr6-built-gearbox-with-3-6-kit/)
- **REPORTED (vendor snippet)** — Epytec sells an "02M 6 speed transmission gearbox reinforcing plate" (article 705) for VR6/R32/S3 applications. — [Epytec 705](https://epytec.de/en/vw-audi-02m-6-speed-transmission-gearbox-reinforcing-plate-golf-1-2-3-4-vr6-r32-s3-705)

### Inferences
- **INFERRED** — A stock CDVC (258 lb-ft) sits exactly at VW's 258 lb-ft MQ350 rating and well inside the 350–400 lb-ft "clean driving" envelope quoted by FCP Euro; the 02M is a sensible match for a naturally aspirated 3.6 and would only become marginal with forced induction.
- **INFERRED** — The FWD 24V box's 3.94/3.09 finals are the tallest of the VR6 02Ms (R32-type boxes are ~4.2/3.3); with 350 Nm on tap the taller gearing is a feature, and it is one more reason to prefer the FWD 24V box over a converted R32/TT 4Motion box.
- **INFERRED** — "OEM steel shift forks" in the swap community means the one-piece steel R32-type forks that FCP Euro says VW later fitted; a box advertised "with steel forks" (like Ninety4co's) already has the main weakness addressed. If the case must be split for an LSD, that is the moment for forks (if brass), input-shaft bearings, all seals and the diff bearings.
- **INFERRED** — Expect a used 24V FWD 02M at roughly $400–1,000 depending on condition and whether forks are done; the only hard data point is Ninety4co's $400 (2023). The population is small (2.5 model years in NA), so plan to buy whatever sound box appears rather than waiting for a specific code.

### Gaps
- No authoritative gearbox-code table for the NA 24V FWD 02M was found; FSR and EDJ are forum attributions and the ETKA "71/18/23" note is second-hand. Read the code off the case/data label of any candidate box.
- VW part numbers for the steel shift forks, input-shaft seal, axle-flange seals, differential bearings and the fluid (G 052 xxx) were not sourced; Ninety4co does not list them either. Pull them from ETKA by gearbox code before ordering (his wrong-seal episode shows the Mk4 02M vs later 02M/02Q variants differ).
- Bar-Tek steel-fork kit price and full fitment list (page 404).
- No market survey of used 02M prices beyond the one build.

---

## Key question 3: Clutch, flywheel, release bearing and starter for a 3.6 on an 02M

### Takeaway
The clutch is a Mk4 24V VR6 6-speed application (VR6 10-bolt crank), not a 3.6-specific part. Ninety4co ran a South Bend "K70287-HD-DMF" Stage 2 Daily with a single-mass flywheel and says a stock 24V clutch will not hold the 3.6 even untuned; UroTuning currently lists the South Bend Mk4/TT 6-speed flywheel kit at $683.62 (K70287-HD image/SKU slug), with the K70287 family rated 450–470 lb-ft in retailer listings. The 02M and 02Q share the release bearing; the starter is dictated by the 02M bellhousing (Ninety4co used a junkyard Mk4 02M starter and lists Valeo 438152).

### Cited Findings
- **REPORTED (build)** — Ninety4co: clutch/flywheel **South Bend K70287-HD-DMF** (Mk4 24V 6-speed application), "Stage 2 Daily full kit", bought from UroTuning, described in the video as a lightened **single-mass** flywheel with new hardware; "Do not use a stock 24V clutch/flywheel; it will not hold the 3.6's torque even untuned"; he wanted a DKM but none existed for this application. — [local parts list](/home/user/vr6_jetta/research/sources/ninety4co-swap-parts-list.md) (row 19); [local series notes](/home/user/vr6_jetta/research/ninety4co-vr6-mk6-swap-series.md) (Part 2, 23:00)
- **VERIFIED (vendor search listing, UroTuning)** — "South Bend Clutch (Flywheel Kit) - VW / Mk1 / TT / Mk4 / GTI / GLI / Jetta 6-Speed": **$683.62** (compare at $1,275.27); product image file named K70287-HD-DMF, URL slug `k70287-hd-smf-sbcf0503`; no torque rating on the listing. Same search: "02-05 Volkswagen Golf 1.8T 6sp Stg 2 Drag Clutch Kit" slug `k70287-hd-dxd-b-dmf` $910.19; Audi S3/A3 Stage 2/3 K70287 variants $910–1,237. — [UroTuning search K70287](https://www.urotuning.com/search?type=product&q=K70287)
- **VERIFIED (vendor search listing, UroTuning)** — Sachs OE-type "Clutch Kit - VW/Audi / Mk4 Golf / Jetta / GLI / Beetle / TT Quattro", slug `06A198141C-SCH`, **$547.13** (compare $1,218.69). — [UroTuning search K70287](https://www.urotuning.com/search?type=product&q=K70287)
- **REPORTED (retailer snippets, BMP Tuning)** — **K70287-HD-OCE-SMF** "Stage 2 Endurance" for "6 speed Mk4 1J / Mk1 8N": **450 ft-lb**; **K70287-SS-O-SMF** "Stage 3 Daily": **470 ft-lb**; listings advise checking flywheel type before ordering; none of the K70287 listings name the VR6 (they name the 6-speed Mk4 1J and Mk1 TT 8N chassis). — [BMP Stage 2 Endurance](https://www.bmptuning.com/products/south-bend-stage-2-endurance-clutch-kit-6-speed-mk4-1j-mk1-8n); [BMP Stage 3 Daily](https://www.bmptuning.com/products/south-bend-stage-3-daily-clutch-kit-6-speed-mk4-1j-mk1-8n)
- **VERIFIED (vendor article)** — VR6 cars have a 10-bolt crank (1.8T 6-bolt; 2.0T TSI 8-bolt flywheel); "The same release bearing is used on both" 02M and 02Q; for the 2.0T TSI the clutch is "the most common failure point on any of the 6-speed transmissions from VW". — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **REPORTED (press article)** — Clutch Masters aluminium hydraulic release bearing for VW/Audi 02M/02Q: replaces the spring-loaded release bearing with a piston-driven one, "direct bolt-on, no modifications", **$399** list. — [PASMAG](https://pasmag.com/performance/transmission-drivetrain/clutch-masters-hydraulic-release-bearing-for-02m02q-transmissions)
- **REPORTED (build)** — Starter: "Mk4 02M starter, Valeo 438152"; in the video he fits a junkyard Mk4 02M starter. First-start note: the starter clicked once and the trunk-battery circuit breaker tripped twice before it cranked ("not enough juice"). — [local parts list](/home/user/vr6_jetta/research/sources/ninety4co-swap-parts-list.md) (row 14); [local series notes](/home/user/vr6_jetta/research/ninety4co-vr6-mk6-swap-series.md) (Part 2 28:10, Part 3 27:00)
- **REPORTED (retailer snippets)** — Valeo 438152: 12 V, ~2 kW, 11-tooth pinion, 76 mm flange, PLGR, aluminium housing, two unthreaded mounting holes; one retailer says no application data available, another's marketing text names TT/Golf/R32. On buycarparts the R32 and 2.8 V6 24V applications sit under Valeo **458167**, with 438152 appearing only as a cross-reference. — [partcatalog 438152](https://www.partcatalog.com/products/valeo-438152-starter-motor); [autonationparts 438152](https://aftermarket.autonationparts.com/parts/valeo-valeo-438152-starter-438152); [buycarparts](https://www.buycarparts.co.uk/valeo/1082256)
- **VERIFIED (vendor pages via snippets, IDParts)** — Other 02M-family Valeo starters are engine/box specific: Valeo **438226** = OE **02M 911 024 P** for 2009–2014 Mk6 TDI 6-speed; Valeo **438281** = OE **02M 911 024 M** for 2015 Mk7 6-speed (neither lists a VR6). — [IDParts 438226](https://www.idparts.com/starter-valeo-speed-mk6-cbea-cjaanms-ckra-02m911024p-438226-p-12906.html); [IDParts 438281](https://www.idparts.com/starter-valeo-cvcacrua-02m911024m-438281-p-14896.html)

### Inferences
- **INFERRED** — The "K70287" root is South Bend's Mk4/Mk1-TT 6-speed (02M) application; the HD = Stage 2 "Daily", SS = Stage 3; the OCE/O/DXD codes are disc types; SMF/DMF describe the flywheel situation. Ninety4co's "HD-DMF" kit came with a single-mass flywheel, and UroTuning's listing carries both "DMF" (image) and "smf" (slug), so the most consistent reading is that South Bend's "-DMF" suffix denotes a kit for a car that left the factory with a dual-mass flywheel, supplied with South Bend's single-mass steel flywheel. Confirm with South Bend before ordering; the 24V VR6 10-bolt flywheel pattern is what matters, and the kit must be the VR6 (10-bolt) variant, not the 1.8T (6-bolt) one that shares the K70287 root.
- **INFERRED** — Because the 10-bolt VR6 crank pattern is common to 2.8/3.2/3.6, any 24V VR6 or R32 02M clutch/flywheel bolts to the CDVC; the 3.6's 258 lb-ft puts a stock 24V (2.8, ~195 lb-ft application) clutch over its design torque, which matches Ninety4co's warning. A Stage 2 South Bend (450 lb-ft class) is ample for a stock or Stage 1 3.6.
- **INFERRED** — The CDVC's own flywheel is a DSG drive plate (02E), so the swap must source the flywheel with the clutch kit; a single-mass South Bend flywheel kit sidesteps hunting for a used 24V DMF.
- **INFERRED** — Use the starter that came on the donor 02M (or a Mk4 24V 02M listing) rather than buying by Valeo number: 438152's published application data is thin, and 458167 is the number retailers attach to the R32/24V 02M. Note the starter must also clear the 3.6 block casting; Ninety4co's Mk4 02M starter did.

### Gaps
- No South Bend spec sheet or product page for K70287-HD-DMF itself was reachable (South Bend's exact string returned nothing; UroTuning shows it only as an image name). Torque rating for the HD-DMF kit is not sourced; 450 lb-ft is the figure for the sibling HD-OCE-SMF.
- Clutch Masters, DKM and Sachs Performance 24V-02M kits: no VR6-specific listings were found in this pass (Ninety4co says DKM had none).
- OE VW part number of the 24V 02M starter (02M 911 02x) and confirmation of which Valeo (438152 vs 458167) it is.
- Release bearing / guide sleeve part numbers.

---

## Key question 4: Hydraulics (slave, line, master) and the clutch-pedal switch

### Takeaway
The evidence says the 02M and the GLI's 02Q use the same external-type release mechanism (shared release bearing; a plastic slave cylinder block that aftermarket vendors replace in billet; a Clutch Masters kit that converts both to a hydraulic throw-out bearing), so the brief's premise that the 02Q uses a concentric slave looks wrong and the Jetta's existing master cylinder and line are likely to connect to the 02M slave with little or no adaptation. Electrically, the Mk6 clutch-position switch must be re-fused: in the Passat fuse box it lands on T40 pin 14, which has no fuse because the NA 3.6 was never a manual.

### Cited Findings
- **VERIFIED (vendor article)** — "The same release bearing is used on both" the 02M and 02Q. — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **REPORTED (vendor snippet)** — ACM Technik: the factory **plastic slave block on 02M/02Q transmissions** is "a well-known failure point"; billet aluminium replacement listed for Golf/GTI/Jetta/Passat B6/Tiguan/A3 8P/TT/Leon/Octavia 02M/02Q 6-speed; the listing title says it "replaces 1J0721468C". — [ACM Technik](https://acmtechnik.com/products/vw-golf-gti-jetta-passat-b6-tiguan-audi-a3-8p-tt-seat-leon-skoda-octavia-02m-02q-6-speed-billet-aluminium-clutch-master-cylinder-mod-kit-replaces-1j0721468c)
- **REPORTED (press article)** — Clutch Masters' hydraulic release bearing "for 02M/02Q transmissions" replaces the spring-loaded release bearing, $399, bolt-on. — [PASMAG](https://pasmag.com/performance/transmission-drivetrain/clutch-masters-hydraulic-release-bearing-for-02m02q-transmissions)
- **REPORTED (cross-reference site)** — OE number **02M 141 671** is catalogued as the slave cylinder for VW/Audi/SEAT/Skoda 02M-family boxes; **02M 141 671 A** appears as a kit (slave + release bearing + hose); aftermarket kits distinguish DMF (…671A) and SMF (…671B) applications. No model-year fitment table for the Mk6 GLI was returned. — [spareto 02M141671](https://spareto.com/oe/02m141671); [spareto 02M141671A](https://spareto.com/oe/02m141671a)
- **REPORTED (build, running car)** — Ninety4co kept the Mk6 pedal and master; his parts list has no separate clutch line or slave entry, and the series notes record no hydraulic adaptation; the only clutch-circuit problem was electrical (below). — [local parts list](/home/user/vr6_jetta/research/sources/ninety4co-swap-parts-list.md); [local series notes](/home/user/vr6_jetta/research/ninety4co-vr6-mk6-swap-series.md)
- **REPORTED (build, running car)** — Clutch switch wiring: the ECU would not give a starter signal because "the GTI clutch switch feeds **T40 pin 14**, which is unassigned on the Passat box, so that circuit had no fuse"; **fuse 39 (15 A) added** and it started. Keep "the GTI clutch position sensor on the T40" when re-pinning the Passat fuse box. — [local series notes](/home/user/vr6_jetta/research/ninety4co-vr6-mk6-swap-series.md) (Part 4, 8:02 and 12:03)

### Inferences
- **INFERRED** — Both boxes use an external slave cylinder acting on a release lever and a conventional release bearing (that is what a "hydraulic release bearing" kit replaces, and what a "plastic slave block" is). The GLI's existing clutch line should therefore reach and mate to a 02M slave (02M 141 671-type) with at most a different quick-connect; verify the connector style on the donor 02M slave against the Mk6 line before assembly. If the 02M slave is old, replace it (plastic body, known failure) or fit the ACM billet block.
- **INFERRED** — The Mk6 Jetta GLI clutch-position switch is wired through the Jetta's fuse/relay box exactly like the GTI's; the fuse-39/T40-14 fix transfers as a concept, but the pin and fuse numbers must be re-derived from the Jetta GLI wiring diagram because Mk6 Jetta fuse assignments differ by year (see precedents file, Key question 4).
- **INFERRED** — The CDVC's MED17 ECU also needs the clutch switch and (for a manual) a neutral/clutch strategy; the ECU was never configured for a manual in NA, so the swap calibration must include the manual-transmission coding or the tuner's swap file (precedents file: United Motorsport lists "change/missing/new automatic transmission" in its swap-tune scope).

### Gaps
- A VW fitment table confirming 02M 141 671 (or which suffix) for the 2015–2018 Jetta GLI 02Q and for the 2002–2005 24V 02M was not retrieved (parts.vw.com/ECS fitment pages not opened in this pass).
- Mk6 Jetta GLI clutch master cylinder and line part numbers, and whether the quick-connect at the slave end matches the Mk4 02M slave.
- Whether 1J0 721 468 C (quoted by ACM Technik) is a slave-side or master-side part.

---

## Key question 5: Differential: open as stock, and LSD options for the 02M

### Takeaway
The FWD 02M is open as stock and FCP Euro names the open diff as a weak link above stock power. Peloquin's 02M unit (02M498005A, $1,024 with bearings and ARP bolts) is backordered with no ETA at NGP; Wavetrac's 02M FWD unit (10.309.190WK) is in stock at UroTuning for $1,155.50 (final sale). No Quaife, OS Giken or MFactory 02M listing surfaced in this pass. Any LSD means splitting the case and re-shimming the diff, so it belongs in the same work order as forks and seals.

### Cited Findings
- **VERIFIED (vendor article)** — "the open differential is a weak link for vehicles making substantially more power than stock." — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **VERIFIED (vendor page, NGP Racing)** — "Peloquins Limited Slip Diff VW Mk4 6-Speed 02M", SKU **02M498005A**, **$1,024.00**, "Sold out" / "Special Order"; "all Peloquins differentials are currently on backorder with no ETA... we recommend choosing a Wavetrac differential instead"; fitment (FWD 02M): 2002 GTI 337, 2002–2006 GTI VR6 [sic], 2002 Jetta VR6, 2003 GTI 20th, 2003–2006 GLI; "Does not fit AWD models"; includes differential, ARP hardware kit, new bearings; shim kit optional; lifetime warranty; "we highly recommend having this differential installed by a professional." — [NGP Peloquin 02M](https://store.ngpracing.com/products/peloquins-limited-slip-diff-vw-mk4-6-speed-02m)
- **VERIFIED (vendor listing title)** — NGP sells an "OEM Audi/VW 02M/02Q 6-Speed Transmission Differential Shim Kit" as the companion item. — [NGP shim kit](https://store.ngpracing.com/collections/differentials/volkswagen-jetta-gli-mk5---2005-5-2010-tdi-esi7700376)
- **REPORTED (vendor snippet)** — Kermatdi lists the Peloquin 02M (02M498005a) as special order, "Please Call for Availability", transferable limited lifetime warranty, asks for the VIN to confirm fitment. — [Kermatdi](https://kermatdi.com/i-1031-peloquin-limited-slip-differential-6-speed-02m-transmission-98-08.html)
- **VERIFIED (vendor page, UroTuning)** — "Wavetrac Limited Slip Differential 02M - ALL FWD Mk4 | TT 6-speed", part **10.309.190WK**, $1,295.00 on sale **$1,155.50**, "IN STOCK... ship out within 1 business day", "FITS: 2WD, Golf 4 / Jetta 4 / Beetle S (6-spd)", carbon-fiber bias plates standard, "This clearance item is FINAL SALE! (No returns will be accepted)"; included bearings/bolts not stated. — [UroTuning Wavetrac 02M](https://www.urotuning.com/products/wavetrac-r-limited-slip-differential-02m-all-fwd-mk4-tt-6-speed-10-309-190wk)
- **REPORTED (vendor snippets, Bar-Tek)** — Wavetrac 02M 2WD, Bar-Tek product no. 2102m09.2, **€1,599.95** (shown as US$1,822.66 in another locale), fitment includes Golf III/Corrado 2.8/2.9 VR6 conversions. — [Bar-Tek Wavetrac 02M](https://www.bar-tek.com/02m-differential-wavetrac-2wd)
- **REPORTED (vendor snippet)** — Autotech lists a Wavetrac for the **02Q** at $1,195 (not the 02M). — via [NGP differentials collection](https://store.ngpracing.com/collections/differentials?page=2)
- **REPORTED (vendor snippet)** — Bar-Tek also lists a Peloquin "R32 differential lock" and gives Peloquin's contact as sales@peloquins.com. — [Bar-Tek Peloquin R32](https://bar-tek.com/r32-differential-lock-lock-peloquin)

### Inferences
- **INFERRED** — For a stock-output 3.6 on street tyres the open diff is tolerable (Ninety4co ran open); the LSD is a nice-to-have that is cheapest to do while the case is already apart for forks/seals. With Peloquin supply uncertain, the Wavetrac at UroTuning ($1,155.50, final sale) is the realistic off-the-shelf choice today; add NGP's shim kit and a bearing set if the Wavetrac kit does not include bearings.
- **INFERRED** — The 02M and 02Q diffs are not interchangeable listings (vendors sell separate 02M and 02Q Wavetracs), so a GLI 02Q LSD cannot be carried over.

### Gaps
- Quaife, OS Giken and MFactory 02M FWD part numbers/prices: nothing surfaced (only a Quaife 02A item).
- Wavetrac 10.309.190WK kit contents (bearings, bolts) and fitment-notes tab were not exposed on the page.
- Peloquin production status (NGP says it will update once Peloquin confirms).
- Diff shim selection procedure and preload spec (needs the 02M workshop manual).

---

## Key question 6: Shifter interface: 02M tower vs Mk6 (02Q-style) shift box and cables

### Takeaway
Ninety4co used the stock Mk6 (GTI, 02Q-type) shift box and cables on his Mk4 02M without modification, and both HPA and CTS sell one short-shifter for "02M/02Q", which is consistent with a shared tower/cable-end geometry. The only reported snag was cable routing near the R32-style downpipes.

### Cited Findings
- **REPORTED (build, running car)** — Shift box and cables: "stock Mk6"; "the stock Mk6 dogbone, shift box, cables and manual axles all mate to it"; Part 3: with the USP R32 downpipes "the shifter cables need attention near the pipes". — [local parts list](/home/user/vr6_jetta/research/sources/ninety4co-swap-parts-list.md) (row 6); [local series notes](/home/user/vr6_jetta/research/ninety4co-vr6-mk6-swap-series.md) (Part 3, 21:00)
- **VERIFIED (vendor listing titles)** — HPA "02M - 02Q Short Throw Shifter"; CTS Turbo "VW/Audi 6-speed Manual Short Shift Kit (02M/02Q)". — [HPA](https://www.hpamotorsports.com/products/02m-02q-short-throw-shifter); [CTS Turbo](https://us.ctsturbo.com/?p=2088)
- **REPORTED (vendor snippet)** — Epytec sells a cable-gearbox shift bushing (article 730) for Golf Mk4/Mk3 VR6 and A3 1.8T cable boxes. — [Epytec 730](https://epytec.de/en/golf-mk4-3-vr6-audi-a3-1.8t-cable-gearbox-gear-changing-bush-bushing-730)
- **VERIFIED (vendor article)** — "the 02Q does away with the vehicle speed sensor in the transmission, as used in the 02M." — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)

### Inferences
- **INFERRED** — The 2015–2018 Jetta GLI's 02Q shift box and cables should mate to the 02M tower as the GTI's did (same PQ35 family, same 02Q box); confirm cable lengths on the bench since the Jetta and Golf cables carry different part numbers. Short shifters marketed for 02M/02Q (HPA, CTS) will fit either way.
- **INFERRED** — The 02M's in-box vehicle speed sensor port is unused in a Mk6 (speed comes from ABS over CAN); leave the sensor in place as a plug or cap the bore.

### Gaps
- Mk6 Jetta GLI shift cable part numbers vs Mk6 GTI, and whether lengths differ.
- No Jetta-specific confirmation of cable/downpipe clearance with a 3.6.

---

## Key question 7: Axle flanges and Jetta axles

### Takeaway
Ninety4co ran stock Mk6 manual axles on his 02M, which is the only direct evidence that the 02M's flanges accept PQ35 6-speed axles; the Mk6 Jetta GLI's 02Q axles are the first candidates to test. Flange diameter was not independently verified in this pass.

### Cited Findings
- **REPORTED (build, running car)** — Axles: "stock Mk6 manual axles" on the Mk4 FWD 02M (Mk6 GTI). — [local parts list](/home/user/vr6_jetta/research/sources/ninety4co-swap-parts-list.md) (row 3)
- **VERIFIED (vendor page text via snippet, Epytec)** — Epytec's FWD VR6 driveshafts fit "02M 02Q DQ250 DSG 6 speed" boxes, but "The DQ250 gearboxes, which are installed in conjunction with the 6-cylinder engines, have a star-shaped flange and a tripod joint and are therefore unfortunately not compatible with our drive shafts" — i.e., the 6-cylinder 02E output differs from the 4-cylinder 02E and from the manual boxes' bolt-on flanges. — [Epytec ISP106](https://epytec.de/en/drive-shaft-vw-golf-mk2-mk3-corrado-passat-vr6-axle-conversion-02m-02q-dq250-dsg-6-speed-isp106)
- **VERIFIED (vendor page, Epytec)** — A 4Motion 02M converted to FWD uses drive-shaft flange **02M 409 356 A** on the converted side. — [Epytec install guide](https://epytec.de/en/blog/einbauanleitung-fuer-artikel-698-02m-umruesten-fuer-einbau-in-frontangetriebene-fahrzeuge-z.b-vr6-umbau-auf-02m-getriebe)

### Inferences
- **INFERRED** — The Mk4 FWD 02M and the PQ35 02Q use the same bolt-on inner-CV flange size (the brief's 100 mm), since Mk6 GTI 02Q axles bolted to Ninety4co's 02M unmodified. The 2015–2018 Jetta GLI manual axles should fit the same way; Jetta track/length differences are small within PQ35, but confirm the inner joint plunge on the bench.
- **INFERRED** — For the DSG alternative (Key question 8) the axle situation is worse, not better: the 6-cylinder 02E has a different (star/tripod) output arrangement, so GLI DSG axles are not a given and Passat inner joints may be needed (the precedents file reports longer Passat axles).

### Gaps
- No parts-catalog confirmation of the 100 mm flange on the 24V 02M vs the Mk6 GLI 02Q; no Jetta GLI axle part numbers checked.

---

## Key question 8 (secondary path): the Passat 3.6's 02E DQ250

### Takeaway
The 2012–2018 NMS Passat 3.6 is 6-speed DSG (02E) and front-drive, so a VR6-bellhousing FWD 02E exists and comes with the donor; it is a different housing and output arrangement from the GLI's 4-cylinder 02E, and nothing in this pass yielded its code letters, drive-plate or cooler-line part numbers. The DSG specifics already found (R32-DSG-to-3.6 reports, BFI mount kit, Unitronic TCU file, Passat axle length) are in `precedents_vendors_salvage.md` and are not repeated.

### Cited Findings
- **VERIFIED (Wikipedia/KBB via search summary)** — NMS Passat engine table: 3.6 VR6 FSI with 6-speed DSG, 2012–2018; a 2013 Passat V6 SEL is listed with "6-Spd DSG Tiptronic". — [Wikipedia NMS Passat](https://en.wikipedia.org/wiki/Volkswagen_Passat_(North_America_and_China)); [KBB 2013 V6 SEL](https://www.kbb.com/volkswagen/passat/2013/v6-sel-premium-sedan-4d/options)
- **VERIFIED (Ross-Tech wiki via search summary)** — Ross-Tech labels the car "VW Passat (NMS/A3) MY 2012+" and documents the 02E as "6-Speed Direct Shift Gearbox (DSG/02E)" with label file 02E-300-0xx.LBL; when replacing a mechatronic unit, copy the coding from the original auto-scan into the new unit. — [Ross-Tech NMS](https://wiki.ross-tech.com/wiki/index.php/VW_Passat_(NMS/A3)); [Ross-Tech 02E](https://wiki.ross-tech.com/index.php/6-Speed_Direct_Shift_Gearbox_(DSG/02E))
- **VERIFIED (vendor page text via snippet, Epytec)** — 6-cylinder DQ250s have "a star-shaped flange and a tripod joint" output, unlike 4-cylinder DQ250s. — [Epytec ISP106](https://epytec.de/en/drive-shaft-vw-golf-mk2-mk3-corrado-passat-vr6-axle-conversion-02m-02q-dq250-dsg-6-speed-isp106)
- **REPORTED (aggregator table; partly conflicts)** — A transmission-lookup table puts the DQ250/02E against 2005–2016 Passat 3.2/3.6 "front/all-wheel drive" and lists 09G (FWD) / 09M (AWD) / TF-61SN for 2005–2012 3.6 Passats; this fits the B6 (2006–2010) conventional automatics, not the NMS. — [youcanic](https://www.youcanic.com/volkswagen-transmission-model/)
- **REPORTED (blog, unverified lead)** — A Chinese-language post lists the 02E mechatronic as **02E 325 025** with revisions AD through AM, and AQ/AS/AT for "420 Nm" units. — [zhihu](https://www.zhihu.com/tardis/jm/art/2074298562670761525)
- **REPORTED (already in precedents file)** — HPA found the DQ250 "not reliable past 650 HP" and moved to the DQ500; The Drive quotes a "500 lb-ft limit on the six-speed DQ250" in an HPA context; Unitronic sells a Stage 1 TCU file for the B6 Passat/CC 3.6 DSG. — see `precedents_vendors_salvage.md`, Key questions 1–2

### Inferences
- **INFERRED** — If the car stays DSG, the donor's own FWD 02E is the only sensible gearbox (VR6 housing, already paired with the CDVC's MED17 and its own mechatronics); mixing a GLI 02E or an R32 02E with the CDVC adds bellhousing, drive-plate and TCU-pairing risk for no gain. The NMS unit's code letters, drive plate, cooler lines and mechatronic revision should be read off the donor rather than researched.
- **INFERRED** — The DQ250's nominal rating (350 Nm class, with later uprated variants per the 420 Nm mention) is the same ballpark as the 02M's; neither path has torque headroom to spare for forced induction on paper, though both are routinely run harder.
- **INFERRED** — Axles are the hidden cost of the DSG path: the 6-cylinder 02E's star/tripod output means GLI DSG axles are unlikely to bolt on; expect Passat inner joints or hybrid shafts (precedents file).

### Gaps
- NMS Passat 3.6 02E gearbox code letters (not found; read from donor label or ETKA by donor VIN).
- 02E drive plate, VR6 bellhousing casting, cooler and line part numbers for the 3.6 02E; mechatronic/TCU part number for the CDVC pairing.
- A factory torque rating citation for the DQ250 (not retrieved in this pass).

---

## Consolidated cost picture (manual path, gearbox side only)

| Item | Figure | Label / source |
|---|---|---|
| Used FWD 24V 02M, with steel forks | $400 (2023, Marketplace) | REPORTED, Ninety4co |
| South Bend 6-speed flywheel kit (K70287-HD, Mk4/TT 6-spd) | $683.62 (sale; compare $1,275.27) | VERIFIED, UroTuning search listing |
| South Bend K70287-HD-OCE-SMF Stage 2 Endurance (450 lb-ft) | price not captured | REPORTED, BMP Tuning |
| Sachs OE-type Mk4 6-spd kit 06A198141C (not recommended behind a 3.6) | $547.13 | VERIFIED, UroTuning |
| Clutch Masters hydraulic release bearing 02M/02Q | $399 | REPORTED, PASMAG |
| Peloquin 02M LSD 02M498005A (bearings + ARP) | $1,024, backordered | VERIFIED, NGP |
| Wavetrac 02M FWD 10.309.190WK | $1,155.50 (final sale), in stock | VERIFIED, UroTuning |
| Wavetrac 02M FWD (EU) | €1,599.95 | REPORTED, Bar-Tek |
| Bar-Tek steel shift forks (3) | price not captured | REPORTED |
| Epytec 4Motion-to-FWD kit 698 (only if using an R32/TT box) | price not captured | VERIFIED page exists |
| Gear oil, GL4 75W-80/90, ~2.5 L | — | VERIFIED, FCP Euro |
| Trans mount 1K0 199 555 AP (2-bolt Mk4 02M) | — | REPORTED, Ninety4co |
| Fuse for clutch switch circuit (his: fuse 39, 15 A) | — | REPORTED, Ninety4co |

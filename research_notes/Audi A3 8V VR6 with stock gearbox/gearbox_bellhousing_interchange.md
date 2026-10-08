# Bolting a VW VR6 to the Audi A3/S3/RS3 8V's own transmissions (0D9 DQ250, 0GC DQ381, 0DL DQ500, 0FB/02Q manual) and the TT boxes: bellhousing interchange, adapter plates, flywheels, and matching VR6 gearboxes

Research date: 2026-10-08. Background read first and **not repeated** except where needed for a point: `research_notes/Audi A3 8V VR6 swap parts/transmission_driveline.md` (VR6-pattern gearbox families, HPA VR550T, Haldex 5, Atlas 09P) and `research_notes/Mk6 Jetta CDVC VR6 swap parts/manual_02m_transmission.md` (02M/02Q facts, 10-bolt VR6 crank, Epytec kits). The TuneZilla S3 precedent is summarised from `research_notes/Audi A3 8V VR6 with stock gearbox/tunezilla_vr6t_s3_build.md` (builder's own videos).

Labels: **VERIFIED** = parts catalogue, factory document or index of factory manuals, or vendor product page actually opened; **REPORTED** = forum or build post, press, video, or vendor or listing text seen only in a search-engine summary (page not opened); **INFERRED** = my reasoning from the cited material. No part number below is invented. Numbers I could not source are listed under Gaps.

Access notes: oemwolf.com has no pages for 02E/0D9/0GC/0BH/0DL 301 107 (all returned its generic not-found page; 02G 301 107 does resolve, titled "clutch housing"). racingcustomparts.com, snapring24.com and valvebody.gr sit behind Cloudflare or return 403, so their content is REPORTED from search summaries. VWVortex, r32oc.com and ttforum.co.uk redirect to a "tollbit" gateway, so forum content is REPORTED from search summaries. Transmission Digest returned 403. YouTube was not used (the TuneZilla facts come from the coordinator's transcript notes).

---

## Verdict question: does a VR6 02E DQ250 front case / clutch housing (02E 301 107 xx, from Mk5 R32 / A3 8P 3.2 / TT 8J 3.2 / CC or Passat 3.6) fit the A3/S3 8V's MQB 0D9 gear case and internals?

### Takeaway
**Verdict: LIKELY YES (mechanically), with caveats. Not proven to catalogue level.**

Evidence for:
1. **One direct precedent.** Dewain (@dmods480) ran "an MKV R32 DSG bell housing on the factory MK7 DSG" in a Mk7 Golf R (VRSociety, 2021-05-19). It is a single second-hand report with no follow-up and no list of modifications.
2. **MQB DQ250s carry 02E-numbered parts:**
   - a Golf VII gearbox listed with references 02E 301 103 / 02E 301 107;
   - MQB 0D9 mechatronics sold as 02E 927 770 AT/AN "DQ250 02E 0D9";
   - rebuild kits and the 02E 398 029 C clutch pack listed for both 02E and 0D9/A3 8V quattro.
3. **No source names a 0D9 301 107 / 0D9 301 103 part number.** Searches and ETKA-mirror probes found none, which is consistent with the 0D9 reusing 02E case numbers.

Evidence against or open:
- A Chinese source calls 02E and 0D9 separate part families with incompatible clutch series (02E 398 029 vs 0D9 398 029 A).
- A machine-written catalogue page claims AWD DSG6 cases carry a 0D9 prefix.
- The VR6 02E differs in output (star flange/tripod) and in its R32 4WD differential.

So the bell face and gear-case joint very probably match, as Dewain's build suggests. What remains unproven for an **A3 quattro** is that the VR6 4WD front case's differential, output and angle-drive (PTU) features accept the 0D9's own diff and PTU. Settle it by a bench comparison of the two front cases before buying anything else (checks under Inferences).

### Cited Findings
- **REPORTED (VRSociety post, 2021-05-19, page opened)**: "MKV R32 DSG bell housing on the factory MK7 DSG", "APR tuned TCU", "custom TZ Engineering dual mass flywheel", DDKA 2.5T. Instagram @dmods480. Searches for "dmods480"/"Dewain" found no later update. — [VRSociety](https://vrsociety.tumblr.com/post/651662812635152384/oem-25l-vr6-turbo-in-a-mk7-golf-r-dewain-is)
- **VERIFIED (vendor)**: HPA's DQ381 program needs a 2018–2019 Golf R. A Mk7 Golf R with an R32-compatible DSG is therefore an earlier 6-speed DQ250 car. — [HPA VR550T](https://www.hpamotorsports.com/pages/hpa-vr550t-2-5l-vr6-program-for-golf-r)
- **REPORTED (salvage listing, search summary)**: "Gearbox volkswagen golf vii … 02e301103 02e301107". — [ecooparts Golf VII](https://ecooparts.com/en/used-auto-part/gearbox/volkswagen/golf-vii-lim/17733787_gearbox-volkswagen-golf-vii-lim-sport-bluemotion.html)
- **REPORTED (vendor titles, search summaries)**:
  - "DQ250 02E 0D9 **02E927770AN** Transmission Mechatronic" and "**02E927770AT** DQ250 02E 0D9 Transmission Mechatronic". — [Sheng Hai AN](https://www.shenghaiautoparts.com/shop/tcu/dq250-02e-0d9-02e927770an-transmission-mechatronic/); [Sheng Hai AT](https://www.shenghaiautoparts.com/shop/tcu/02e927770at-dq250-02e-0d9-transmission-mechatronic/)
  - The AT suffix replaces AL "used on immobilized units in MQB cars with UDS diagnostics". — [Tosen guide](https://www.tosenparts.com/dq250-vs-dq200-mechatronic/); [MHH "How to determine DQ250 versions (cxx,exx,fxx,mqb)"](https://mhhauto.com/Thread-How-to-determine-DQ250-versions-cxx-exx-fxx-mqb)
  - Rebuild kit "02E, DQ250, 0D9 (DSG) (6-Speed, FWD) Automatic Transmission Overhaul Repair Kit". — [Cobra Transmission](https://cobratransmission.com/dsg-02e-overhaul-kit-w-o-pistons-3023001-1)
- **VERIFIED (vendor fitment)**: clutch pack 02E 398 029 C lists "Audi A3 8V, Quattro: 2.0T" and Golf VII. — [vagparts](https://vagparts.com.au/products/02e398029c-clutch-service-kit)
- **REPORTED (VCDS wiki table, search summary)**: 02E and 0D9 are both listed as Borg-Warner 6-speed wet-clutch units, 350 Nm. 02E from 2003 (A3 8P, TT, Golf, Passat); 0D9 from 2013 (Golf 7, A3 8V, Passat from 2015). — [VCDS wiki "Getriebe"](https://wiki-online.vcds.de/de/Dokumentation/Getriebe)
- **Conflict (REPORTED, Chinese article via search summary)**: 02E and 0D9 are successive generations whose base numbers differ. "Most parts don't carry over"; clutch series 02E398029 vs **0D9398029A** "not compatible". The search summary adds that the MQB mounting interface, flywheel and clutch housing "were all new". It is unclear whether the article says this or the summariser inferred it; treat it as unverified. — [zhihu](https://www.zhihu.com/tardis/jm/art/2074298562670761525)
- **Conflict (REPORTED, machine-written catalogue text)**: "The 4motion, 4x4, and Quattro all-wheel-drive (AWD) DSG6 installations … use a distinct housing assembly carrying the 0D9 parts-code prefix". This contradicts Maktrans's "Front case 4WD 02E DQ250 … 02E301107 / 02E301107R" (VERIFIED). — [Autoparts-24](https://www.autoparts-24.com/oem/02E-301-107/); [maktrans](https://maktrans.net/02E4WD107)
- **REPORTED (search summary of Super-Parts)**: 02E301107 front case listed for transmission codes "SYJ, SFT, SFU, RLN" (code family not identified). — [Super-Parts](https://www.super-parts.eu/02e301107-gearbox-housing-dq250-02e-dsg-6/)
- **VERIFIED (Ross-Tech)**: replacing the 0D9 "transmission or mechatronics unit will result in P1701". Keeping the A3's own 0D9 mechatronic and moving it onto the VR6 front case avoids a new-module pairing (INFERRED). — [Ross-Tech 0D9](https://wiki.ross-tech.com/wiki/index.php/6-Speed_Direct_Shift_Gearbox_(DSG/0D9))
- **Searched, nothing found**: "0D9301107", "0D9 301 107", "0D9301103", "0D9 301 103". zzap.ru, emex.ru and partsouq returned bot challenges. exist.ru and autodoc.ru returned no data without JavaScript. The scribd 0D9 manual did not load. No 0D9 rebuild using 02E case parts was documented.

### Inferences
- **INFERRED, verdict logic:** the R32 bell on a Mk7 DSG (Dewain) is the decisive data point for the bell face and the gear-case joint. Shared 02E case, mechatronic and clutch numbering on MQB units explains why it worked. The A3 quattro case adds the 4WD angle-drive interface, which Dewain's 4Motion Golf R also had, but the post does not say whether he kept the Golf R PTU unchanged.
- **INFERRED, physical checks that settle it (in order):**
  1. **Read the cast or stamped numbers** on the A3's 0D9 front case and gear housing. If they read 02E 301 107 xx / 02E 301 103 xx, the case family is shared. Compare the suffix with the VR6 donor's front case.
  2. **Joint face:** lay the VR6 front case on the 0D9 gear housing (or compare photos and measurements). Check bolt-hole count and positions, dowel positions, and the oil-gallery ports to the mechatronic and clutch-oil feed.
  3. **Bearing bores:** compare bore diameters and positions for input-shaft/clutch support, output shafts 1 and 2, reverse shaft, differential bearings, and selector/parking-lock shafts. The front case carries bearing bores (Maktrans "spun bearing bore" remanufacturing).
  4. **4WD features:** compare the angle-drive (PTU) mounting face, spigot and bolt pattern, and the right-hand output bore and seal, between the VR6 4WD case and the 0D9 4WD case. Confirm the 0D9 differential (with its MQB flanges) fits the VR6 case's diff bores and seals. That is where the 6-cylinder star-flange/tripod output and the R32-only diff (Quaife exclusion) could bite.
  5. **Flywheel:** try-fit the VR6 02E DMF (022 105 266 AH/AK) on the 0D9 clutch input hub. Check spline engagement and axial depth. Dewain needed a custom DMF, but with a DDKA crank.
  6. **Clutch cover and oil-pump drive:** confirm the 0D9 clutch cover (renewed at every repair) and oil-pump drive seat in the VR6 front case.
  7. **Starter:** the starter boss is on the VR6 front case, so use the donor's VR6 DSG starter and check ring-gear mesh with the DMF.
  8. **Re-shim and re-adapt:** re-shim with 02E 398 321 rings and set K1/K2 end play per the 0D9 manual. Run clutch adaptation (Ross-Tech 0D9 basic settings).
- **INFERRED, best donor:** a 4WD VR6 DSG front case from a Mk5 R32 DSG or A3 8P 3.2 quattro S tronic, the same family Dewain used (MKV R32). TT 8J 3.2 S tronic is the third choice. CC/Passat 3.6 only if confirmed 4Motion DSG. Not the NMS Passat 3.6 (FWD).

### Gaps
- No catalogue (ETKA) confirmation of the 0D9 front-case number, or of which 02E 301 107 suffixes are VR6 and which are 0D9.
- No detail of what Dewain modified, and no later update.
- No documented 0D9 rebuild that used 02E case parts.

---

## Headline question: the exact parts for a stock 3.2/3.6 VR6 on the A3/S3 8V quattro's own 6-speed DQ250 (0D9), via a VR6 02E bellhousing (front case) plus a VR6 DSG dual-mass flywheel

### Takeaway
**Feasible, with one precedent, but it is a gearbox-rebuild job, not a bolt-on.** In May 2021, VRSociety reported Dewain (@dmods480) running "an MKV R32 DSG bell housing on the factory MK7 DSG with an APR tuned TCU and a custom TZ Engineering dual mass flywheel" in a Mk7 Golf R, behind a Chinese 2.5T DDKA VR6. The Mk7 Golf R's factory DSG before the DQ381 change is the 6-speed DQ250, and an R32 bell only fits the DQ250 family.

On the DQ250 the "bellhousing" is the front half of the gearbox case, **02E 301 107** ("front housing / bell housing / clutch housing"). It carries bearing bores and comes in a separate **4WD** version. So the job is:
- split the A3's 0D9;
- move its gearsets, differential, clutch pack, mechatronic, rear housing (02E 301 103 family) and angle drive onto a **4WD VR6 02E front case**;
- re-shim (end-play rings 02E 398 321);
- fit the **VR6 DSG DMF 022 105 266 AH** (Audi A3/TT 3.2) **/ 022 105 266 AK** (VW R32 / CC / Eos / Passat 3.2 and 3.6), LuK **415 0755 09**.

For stock power the torque is fine on paper: DQ250 "Maximum 350 Nm (depending on engine)" (SSP 308), against about 320 Nm for the 3.2 and about 350 Nm for the 3.6.

The open risks, none resolved by any source:
1. The VR6 front-case part-number suffix, and whether 3.2 and 3.6 cases differ.
2. Whether the VR6 4WD front case's output, differential and angle-drive faces match the 0D9 4WD internals, so that the 0D9 PTU and A3 axles really carry over. The VR6 02E uses star-flange/tripod outputs and an R32-specific diff.
3. Whether the OEM VR6 DMF spline engages the 0D9 hub. Dewain used a *custom* DMF, but for a DDKA crank, so this is not proof either way.
4. The starter number.

**Donor rule (INFERRED):** use a **4WD** VR6 DSG front case: Mk5 R32 DSG, A3 8P 3.2 quattro S tronic, TT 8J 3.2 S tronic, or a CC/Passat 3.6 4Motion *if* it is a DSG. The NMS Passat 3.6 is FWD only, so its front case is the FWD casting and will not take the A3's angle drive.

### Cited Findings
**The precedent and the 0D9**
- **REPORTED (VRSociety post, 2021-05-19, page opened)**: Dewain's Mk7 Golf R with a Chinese-market 2.5L VR6 Turbo (DDKA) from a Teramont, using "an MKV R32 DSG bell housing on the factory MK7 DSG", an APR-tuned TCU, and "a custom TZ Engineering dual mass flywheel" "for now". The Teramont ECU is to be tuned for the MK7 chassis. He plans to run the Teramont's DQ500 later. Instagram @dmods480. No later status found. — [VRSociety](https://vrsociety.tumblr.com/post/651662812635152384/oem-25l-vr6-turbo-in-a-mk7-golf-r-dewain-is)
- **VERIFIED (vendor page, background)**: HPA's DQ381 VR6 program requires a "2018-2019 Golf R" with DSG. The DQ381 arrived on the Golf R with the 2018 model year, so a Mk7 Golf R *before* that has the 6-speed DQ250. — [HPA VR550T Golf R](https://www.hpamotorsports.com/pages/hpa-vr550t-2-5l-vr6-program-for-golf-r)
- **VERIFIED (Ross-Tech)**: the 0D9 is documented for the "Mk7/MQB chassis". "Replacement of the transmission or mechatronics unit will result in P1701." So keep the A3's own 0D9 mechatronic, already paired to the car. — [Ross-Tech 0D9](https://wiki.ross-tech.com/wiki/index.php/6-Speed_Direct_Shift_Gearbox_(DSG/0D9))

**Bellhousing (front case)**
- **VERIFIED (vendor pages)**:
  - Maktrans lists "Front case **4WD** 02E DQ250 DSG 6 02E301107" ($210) and "Case front part 4WD … **02E301107R**" (€207.90). — [maktrans](https://maktrans.net/02E4WD107)
  - Super-Parts lists "02E301107 Gearbox housing" and "**02E301103M** Gearbox housing" (€196.48 each). Its search summary gives 02E301107 transmission codes "SYJ, SFT, SFU, RLN" (REPORTED). — [Super-Parts](https://www.super-parts.eu/02e301107-gearbox-housing-dq250-02e-dsg-6/)
- **Conflict (REPORTED, machine-written text)**: Autoparts-24 says 02E 301 107 is catalogued for FWD 02E variants and that AWD DSG6 cases carry a 0D9 prefix. This contradicts Maktrans's 4WD 02E 301 107 listings. — [Autoparts-24](https://www.autoparts-24.com/oem/02E-301-107/)
- **REPORTED (listing title)**: "08 Audi TT Mk2 Auto Automatic Transmission Trans Assembly 02E301107" (engine not stated). — [eBay 2112956159](https://www.ebay.com/p/2112956159)
- **Not found**: any 02E 301 107 suffix tied to the R32, A3 3.2, TT 3.2 or 3.6.

**Flywheel (drive plate / DMF)**
- **VERIFIED (vendor page)**: DMF "415075509 / 022105266AH / 022105266AK", mapping "Audi TT, A3: 022105266AH" and "VW CC, Eos, Passat, Golf: 022105266AK". Fitment covers A3 8P 3.2 (BDB/BMJ/BUB), TT 8J/8N 3.2 (BUB/BHE/BPF/CBR), R32 Mk4/Mk5, **CC 3.6**, **Passat B6/B7 3.2/3.6**, Eos 3.2/3.6 and Superb 3.6. US $349.99. The page does not say DSG. — [FridayParts](https://www.fridayparts.com/dual-mass-flywheel-415075509-022105266ah-for-vw-cc-golf-r32-audi-a3-tt-3-2-3-6-vr6)
- **REPORTED (titles and prices, search summaries)**:
  - "OEM VW **DSG** Flywheel Mk5 R32 Audi A3 2.8L 3.2L Dual Mass 022105266AK". — [eBay 290689210280](https://www.ebay.com/itm/290689210280)
  - FCP Euro "Dual Clutch Flywheel – LuK 022105266AK", $857.99. — [FCP Euro](https://www.fcpeuro.com/filters/Volkswagen-parts/Flywheel/)
  - The manual R32 DMF is a different part (LuK DMF057). — [PartsHawk](https://partshawk.com/volkswagen-r32-clutch-flywheel-luk-dmf057.html)
- **VERIFIED (vendor page)**: RTMG "Performance Dual Mass Flywheel for 3.2 V6 R32 Engines DQ250 02E", SKU 901-0680, €1,351.60, 8.2 kg, chromoly, "770Nm to 1200Nm"; "Only genuine OEM flywheel bolts must be used". 0D9 and 3.6 fitment not stated. — [RTMG](https://rtmgperformance.com/products/dsg-dq250-dual-mass-flywheel-for-3-2-v6-r32-engines)
- **REPORTED (title)**: Carlicious "R32 DSG Lightweight Flywheel 3kg", "MK4 or MK5 DSG Gearbox". — [Carlicious](https://www.carlicious-parts.com/R32-DSG-Lightweight-Flywheel-3kg)
- **VERIFIED (SSP 308 / 851403)**: the DMF's internal splines drive the input hub of the double clutch. The DMF is the only engine-specific rotating part. — [SSP 308](https://www.volkspage.net/technik/ssp/ssp/SSP_308.pdf)

**Clutch pack and input shafts**
- **VERIFIED (vendor fitment)**: the DQ250 clutch pack **02E 398 029 C** lists the A3 8V (incl. "Quattro: 2.0T"), Golf 7, TT 8S and 4-cylinder PQ cars, and **no VR6**. — [vagparts](https://vagparts.com.au/products/02e398029c-clutch-service-kit)
- **Conflict (REPORTED)**: 02E 398 029 vs 0D9 398 029 A are claimed "not interchangeable". — [zhihu](https://www.zhihu.com/tardis/jm/art/2074298562670761525)
- **No source** compares input shafts or K1/K2 packs between 4-cylinder and VR6 02E.

**Torque**
- **VERIFIED**: "Maximum 350 Nm (depending on engine)". — [SSP 308](https://www.volkspage.net/technik/ssp/ssp/SSP_308.pdf)
- **VERIFIED**: TVS gives "Stock rated up to +/- 350 Nm", "engine torque up to 350-380 Nm". — [TVS DQ250](https://tvsengineering.com/en/dsg-gearbox/dq250/)

**Starter**
- **REPORTED (listing summaries)**: DSG starters 02E 911 023 J (6-speed automatic), 02E 911 023 S (Tiguan 2.0 TSI DQ500) and 02E 911 024 A (2.0 TDI). **No R32/3.2/3.6 DSG starter number was found.** — [eBay 275087204380](https://www.ebay.com/itm/275087204380)

**Confirming the A3 has the 6-speed 0D9**
- **VERIFIED (factory index)**: 0D9 code letters MTF, PPN, PUL, QSJ, MTE, PPM, PUH, QSE, PDZ, PPR, PUJ, QSF, NUT, PPP, PUP, QSM, PUN, QSL. The 2.0 TFSI 162 kW combinations are PUL, PZQ, QML, QMQ, QSJ, QSQ, RHN, RVS, RVW. The 7-speed alternatives in the same index are **0CW** (DQ200; e.g. PNA, PNB, MSP, NAR, PMZ …), **0GC** (DQ381) and **0DL** (DQ500, RS3). — [vwts.ru A3 8V](https://vwts.ru/audi_a3_8v.html)
- **REPORTED (press/spec pages, search summaries)**:
  - The 2016 US A3/S3 media kit lists six-speed S tronic across the line. — [Audi 2016 media kit](https://www.audiworld.com/wp-content/uploads/2018/12/2016-audi-a3-s3-media-kit.pdf)
  - For 2017, FWD 2.0T A3s gained a seven-speed while the **2017 A3 2.0T quattro "continues with … a six-speed dual-clutch S tronic"**. — [Autotrader.ca 2017 A3/S3](https://www.autotrader.ca/editorial/expert-reviews/audi/a3/first-drive-2017-audi-a3-s3/); [JD Power 2017 A3](https://www.jdpower.com/cars/2017/audi/a3)
  - **Conflict:** an Australian MY17 A3 quattro listing shows a 7-speed. — [carsales](https://www.carsales.com.au/cars/details/2017-audi-a3-s-line-auto-quattro-my17/SSE-AD-20641863/)

### Inferences
- **INFERRED, parts list (stock 3.2/3.6, A3/S3 8V quattro 0D9 kept):**

  | # | Part | Number / source | Status |
  |---|---|---|---|
  | 1 | A3/S3 8V quattro 6-speed DQ250 **0D9** (DQ250-6A) with its own mechatronic, angle drive (PTU), axles, mount, selector | Code letters from the data sticker must be in the 0D9 list above | Keep (avoids P1701 pairing) |
  | 2 | **4WD VR6 02E front case / bellhousing** | 02E 301 107 + unknown VR6/4WD suffix (4WD 02E301107R exists, engine unknown). Donor: Mk5 R32 DSG, A3 8P 3.2 quattro S tronic, TT 8J 3.2 S tronic, or CC/Passat 3.6 4Motion DSG. Not the NMS Passat 3.6 (FWD). | Read the cast number on the donor |
  | 3 | Gearbox rebuild consumables | End-play ring set 02E 398 321; clutch cover (the clutch-pack listing says it must be renewed at every repair); seals; G052 182 DSG oil (7.2 L) | Per factory manual |
  | 4 | **VR6 DSG DMF** | 022 105 266 AH (Audi 3.2) / 022 105 266 AK (VW 3.2/3.6), LuK 415 0755 09. Alternatives: RTMG 901-0680 (€1,351.60) or a custom DMF (TZ Engineering, as Dewain) if the OEM spline does not match the 0D9 hub | Bench-check the spline engagement |
  | 5 | VR6 flywheel bolts | "genuine OEM flywheel bolts" (RTMG); number not sourced | Gap |
  | 6 | Starter | Use the starter from the same VR6 DSG donor (it locates in the VR6 bell) | Number not sourced |
  | 7 | TCU calibration | Dewain used an "APR tuned TCU". Stock power may need only coding for the new engine/torque messages | Unverified |
  | 8 | Engine-side mount | Atlas 3.6 mount (TuneZilla on S3 8V; VWVortex poster on Mk7: "The Atlas VR mount bolts straight into the same location as my 2.0t") | REPORTED |

- **INFERRED, why a 4WD donor matters:** the 4WD front case is a separate casting (Maktrans) and the angle drive (PTU) bolts to the gearbox. To keep the A3's PTU, prop shaft and Haldex 5, the VR6 front case must be the 4WD type, and its angle-drive interface must match the 0D9 4WD's. Dewain's car is a 4Motion Golf R, so the R32 4Motion front case appears to have accepted Mk7 internals with the Golf R's AWD hardware. That is not explicitly stated, so verify it on the bench.
- **INFERRED, 3.2 vs 3.6 front case:** the vendors' common flywheel fitment (one DMF family for 3.2 and 3.6) and the shared VR6 bell for 24V/3.2/3.6 (Key question 6) suggest one VR6 02E bell pattern for 3.2 and 3.6. Suffixes may still differ by drivetrain (FWD/4WD) and build date. The R32/A3 3.2/TT 3.2 4WD cases are the only proven-donor type (Dewain).
- **INFERRED, the DMF spline question:** the 02E 398 029 C clutch pack fits both 4-cylinder 02E and MQB 0D9 cars, so the 0D9's input hub is very likely the 02E spline. In that case the OEM VR6 02E DMF (022 105 266 AH/AK) should engage it. Dewain's custom DMF was needed for the DDKA crank (a DQ500-native engine), not necessarily for the 0D9 hub.
- **INFERRED, how to confirm the A3 is a 0D9:** read the 3-letter gearbox code on the vehicle data sticker (spare-wheel well or service booklet) or on the gearbox case, and match it to the 0D9 code list. In VCDS module 02 the part number should begin 0D9 (the 0D9 vs 0GC/0CW prefix is the giveaway). The selector or cluster showing a 7th gear means it is 0GC or 0CW. US 2015–2017 A3 2.0T quattro and S3 are reported 6-speed.

### Gaps
- VR6 02E front-case part numbers (R32, A3 3.2, TT 3.2, CC/Passat 3.6 4Motion, NMS Passat 3.6 FWD) and whether 3.2 and 3.6 cases differ. Not in any source reached (no ETKA access; oemwolf has no 02E 301 107 page).
- Whether Dewain's car kept the Golf R PTU and axles unchanged, and what TZ Engineering changed on the DMF. No details beyond the 2021 post.
- VR6 DSG starter part number; VR6 DMF bolt part number and torque.
- Whether K1/K2 packs or input shafts differ between 4-cylinder and VR6 DQ250 (no source; the clutch-pack fitment omits VR6).
- The exact model year the US A3 2.0T quattro and S3 switched to the 7-speed DQ381 (0GC). Check each car's code.

---

## Key question 1: DQ250. Can a VR6 02E clutch housing, clutch pack and drive plate be fitted to the A3/S3 8V's MQB 0D9?

### Takeaway
It is not a bolt-on job. One precedent exists: Dewain's Mk7 Golf R ran an MKV R32 DSG bell housing on the factory Mk7 DSG (2021). See the Verdict question and Headline question above. The DQ250 case is two halves: a front case / clutch housing (bellhousing) **02E 301 107** and a rear gearbox housing **02E 301 103**. The front case carries shaft and differential bearing bores, so swapping it means fully splitting and re-shimming the gearbox. It is not like changing a bolt-on adapter. Evidence suggests the MQB 0D9 reuses 02E-numbered cases and the 02E clutch pack. The VR6 02E differs in more than the bell, though: its bolt pattern or angle, its star-flange/tripod outputs, and (in 4WD form) its differential. The MQB 0D9 has its own mechatronic generation. Torque is also against it: the DQ250 is rated at 350 Nm "depending on engine", which a naturally aspirated 3.6 already reaches.

### Cited Findings
- **VERIFIED (factory manual index, A3 8V)**: "Gearbox 0D9 – DSG Workshop Manual" for A3 8V1/8VA/8VS/8V7, gearbox code letters **MTF, PPN, PUL, QSJ, MTE, PPM, PUH, QSE, PDZ, PPR, PUJ, QSF, NUT, PPP, PUP, QSM, PUN, QSL**. A second "Direct Shift Gearbox 0D9" manual (ed. 09.2015) gives engine combinations: **PUL, PZQ, QML, QMQ, QSJ, QSQ, RHN, RVS, RVW** with 2.0 L 162 kW TFSI; RVS with 169 kW; PUL, PZQ, QMQ, QSJ, RVS with 155 kW; PZN, PUG, QMM, QSD with 110 kW TDI. It covers A3 8V1/8VA/8VS/8V7 (2013–) and 8VK/8VF/8VE/8VM (2017–). Both manuals' contents read "00 Technical data, 30 Clutch, 34 Controls, housing, 35 Gears, shafts, 39 Final drive". — [vwts.ru A3 8V index](https://vwts.ru/audi_a3_8v.html)
- **VERIFIED (factory manual index, A3 8P)**: the "6-Speed Dual Clutch Transmission 02E" repair manual (ed. 09.2015) lists only 4-cylinder and TDI pairings: 1.4 TSI (JBT, JPS, KDC, KNF, KPY, KVV, LRC), 1.9 TDI, 2.0 TDI, and **2.0 TFSI 147 kW (HBQ, HRW, HUS, HUT, HXW, JPP, KCZ, KNC, KPV, LQZ, LTL, MMA, MSX, MSY, NJL, NJM, NLQ, NVW, PBG, PPZ, PQL)**. There is no 3.2 VR6 row. The same index carries the 02E SSP (Russian), which covers the A3 8P, TT 8J and TT 8N, the J743 mechatronic and the angle drive. — [vwts.ru A3 8P index](https://vwts.ru/audi_a3_8p.html); [vwts.ru TT 8J index](https://vwts.ru/audi_tt_8j.html)
- **VERIFIED (SSP 308, "Direct Shift Gearbox 02E")**:
  - Torque path: "The torque is transmitted from the crankshaft to the dual mass flywheel. The splines of the dual mass flywheel on the input hub of the double clutch transmit the torque to the drive plate of the multi-plate clutch". So the engine-specific part is the DMF, and the gearbox-side interface is a splined input hub.
  - Technical data: weight "Approx. 94 kg front-wheel drive, 109 kg 4motion"; torque "**Maximum 350 Nm (depending on engine)**"; oil "7.2 ltr. DSG oil G052 182".
  - The oil cooler "is incorporated in the cooling circuit of the engine".
  - "The direct shift gearbox is already available for Golf R32 and Touran models."
  — [SSP 308 PDF](https://www.volkspage.net/technik/ssp/ssp/SSP_308.pdf)
- **VERIFIED (SSP 851403, US version)**: "The dual-mass flywheel transfers the torque to the input hub via splines". — [SSP 851403 PDF](https://at-manuals.com/wp-content/uploads/2016/manuals/DSG-02E%20DQ250%20DQ200%20manual.pdf)
- **REPORTED (vendor listings, search summaries), the 02E 301 107 housing:**
  - "Volkswagen 02E DQ250 Front Housing – Bell Housing (02E301107)", €140, out of stock. — [valvebody.gr](https://valvebody.gr/product/volkswagen-02e-dq250-front-housing-02e301107/)
  - "VAG Skoda VW DSG 6 PQJ DQ250 Getriebe Gehäuse Kupplungsgehäuse 02E301107", €200 used. — [eBay 126109557104](https://www.ebay.com/itm/126109557104)
  - "08 Audi TT Mk2 Auto Automatic Transmission Trans Assembly 02E301107" (sold out; engine not stated; page opened, **VERIFIED** that the listing exists). — [eBay 2112956159](https://www.ebay.com/p/2112956159)
- **VERIFIED (vendor pages, curl)**:
  - Maktrans: "Front case 4WD 02E DQ250 DSG 6 02E301107", "Case front part 4WD DQ250 02E DSG **02E301107R** €207.90", and "Remanufactured 02E DQ250 4WD Front Case 02E301107 – Spun Bearing Bore Restored [Exchange Basis] … €189". The front case therefore carries bearing bores. — [maktrans](https://maktrans.net/02E4WD107)
  - Super-Parts: "02E301107 Gearbox housing DQ250 02E DSG 6" and "**02E301103M** Gearbox housing DQ250 02E DSG 6", both €196.48. — [Super-Parts](https://www.super-parts.eu/02e301107-gearbox-housing-dq250-02e-dsg-6/)
- **REPORTED (salvage listing title, search summary)**: a used Golf VII (MQB) gearbox is listed with references "02e301103 02e301107". MQB DQ250s appear to use 02E-numbered case castings. — [ecooparts Golf VII](https://ecooparts.com/en/used-auto-part/gearbox/volkswagen/golf-vii-lim/17733787_gearbox-volkswagen-golf-vii-lim-sport-bluemotion.html)
- **REPORTED (Brazilian torque sheet, search summary)**: "DQ250-6F tipo 0D9 e DQ250-6A tipo 0D9", i.e. the 0D9 exists in FWD (6F) and AWD (6A) forms. — [cambioautomaticodobrasil PDF](https://cambioautomaticodobrasil.com.br/app/uploads/2021/12/httpscambioautomaticodobrasil.com_.brpainelpublicpdf15880957475ea86b0306237-1.pdf)
- **VERIFIED (vendor fitment, clutch pack)**: "02E398029C – DSG Clutch Service Kit – Audi 8P/8V/8J & Volkswagen MK5/MK6/MK7", AUD $2,058.50, "stock replacement clutch pack for the DQ250 DSG gearbox". Its fitment includes A3 8V (2013–16, 2017–) and "**Audi A3 8V, Quattro: 2.0T**", Golf 5G, Tiguan AD1, TT/TTS 8S and TT 8J (FWD 2.0T only). It lists **no VR6/3.2/3.6** application. — [vagparts.com.au 02E398029C](https://vagparts.com.au/products/02e398029c-clutch-service-kit)
  - **Conflict (REPORTED, Chinese blog via search summary)**: 02E and 0D9 are two generations with clutch series **02E398029** vs **0D9398029A** and are "not interchangeable". — [zhihu](https://www.zhihu.com/tardis/jm/art/2074298562670761525)
- **REPORTED (vendor snippet)**: clutch end-play ring set **02E 398 321** ("chosen to shim the clutch on the input shaft"). Its fitment includes VR6 and 3.2 cars (VW CC VR6, Eos 3.2). — [ECS 02E398321](https://www.ecstuning.com/b-genuine-volkswagen-audi-parts/ring-set/02e398321/)
- **REPORTED (VWVortex 1.8T + DQ250 build, search summary)**: "DO NOT buy the DSG6 transmission from the VR6 equipped cars. It has a different bellhousing bolt pattern and WILL NOT FIT to your 4 cylinders engine." The same poster advises avoiding DSG6 units from MQB cars; no reason was given in the snippet. — [VWVortex 9353965](https://www.vwvortex.com/threads/1-8t-20v-dsg-dq250-complete-project-with-photos-videos-and-racelogic-data.9353965/)
- **REPORTED (r32oc, search summary)**: "You can't put a complete GTI box into a VR6 powered car. The bellhousing is the same pattern, but at a different angle. The GTI engine leans backwards and the VR6 leans forwards." Also: "Mk5 R32 plus Mk2 Audi A3/TT 3.2 V6 all use the same gearboxes with same codes". **Conflict:** this "same pattern, different angle" claim contradicts the VWVortex "different bolt pattern" claim. Both agree the bell casting differs. — [r32oc 274130](https://www.r32oc.com/threads/mk5-r32-dsg-compatibility.274130/)
- **REPORTED (vendor title)**: Quaife "ATB helical LSD differential for 4WD VAG DQ250 DSG 02E transmission **excluding Golf 5 R32**" (QDF25R). The VR6 02E 4WD differential differs from the 4-cylinder one. — [AwesomeGTI QDF25R](https://www.awesomegti.com/shop-by-car/volkswagen/golf-mk6/differentials/quaife-atb-helical-lsd-differential-for-4wd-vag-dq250-dsg-02e-transmission-excluding-golf-5-r32-qdf25r/)
- **VERIFIED (vendor, background file)**: 6-cylinder DQ250s "have a star-shaped flange and a tripod joint". — [Epytec ISP106](https://epytec.de/en/drive-shaft-vw-golf-mk2-mk3-corrado-passat-vr6-axle-conversion-02m-02q-dq250-dsg-6-speed-isp106)
- **REPORTED (vendor blog title/snippet)**: DQ250 mechatronic **02E 325 025 AD** is "suitable for the Golf 5 GTI, R32, Passat 3C, Audi A3". The PQ-generation J743 is shared between 4-cylinder and VR6 02E boxes. — [Langwieser](https://www.langwieser-performance.com/blogs/news/rescue-for-golf-5-gti-r32-co-dsg-mechatronics-dq250-available-again)
- **REPORTED (forum snippet; thread not identified precisely)**: DSG boxes from MQB cars "have an immobiliser, so you'll need to get it de-immobilised". — [SEAT Cupra forum "DQ200 upgrade?"](https://seatcupra.net/forums/goto/post?id=5044049)

### Inferences
- **INFERRED, what a "VR6 bell on a 0D9" would really involve:**
  - Split the 0D9 and transplant its gearsets, differential, mechatronic and rear housing into a **VR6 02E front case (02E 301 107, VR6 4WD suffix unknown)**.
  - Re-shim the input shafts and differential, then reset K1/K2 end play with the 02E 398 321 rings and the T10303/T10466-type tools.
  - Fit the VR6 DSG DMF (Key question 6).
  - Because the VR6 front case carries the 6-cylinder star-flange/tripod output geometry, the A3's MQB axles and the MQB angle drive would probably no longer match on the right-hand side. That would defeat the point of keeping the A3 gearbox.
  - No source shows the 0D9 front case is dimensionally identical to the 02E's at the bearing bores, mechatronic bores or angle-drive face. The shared "02E 301 1xx" casting numbers make it plausible, not proven.
- **INFERRED**: the reverse trick, putting the 0D9's internals behind a VR6 02E front case, is the same job seen from the other side. Its only gain over using a whole TT 3.2 / R32 4WD 02E is that it keeps the MQB mechatronic, which matters for CAN. That gain is uncertain anyway (component protection and immobiliser on MQB DSGs).
- **INFERRED, torque:** 350 Nm (SSP 308) is about the stock 3.6's output (≈350–360 Nm). Any turbo VR6 is far outside it. The DQ250 is the wrong gearbox for this swap regardless of the bell.
- **INFERRED, cooler:** the 02E/0D9 cooler runs on engine coolant, so the VR6's coolant plumbing must feed the A3's gearbox cooler. This is minor.

### Gaps
- No ETKA listing of the 02E 301 107 suffixes by engine (VR6 vs 4-cylinder, FWD vs 4WD), and no 0D9 301 107 number found. oemwolf has none of them.
- No dimensional comparison of the 02E vs 0D9 front case, and no confirmation that the 0D9 input-hub spline equals the 02E's (the clutch-pack evidence conflicts).
- 02E VR6 gearbox code letters for the R32 / A3 3.2 / TT 3.2 (not in the opened manual index).
- Beyond Dewain's one-line 2021 report (R32 DSG bell on a Mk7 Golf R DSG), no VR6-02E-bell-on-0D9 build with parts and modifications was found.
- No 0D9 code letters for the 213 kW US S3 were captured from the index (the snippet showed 155/162/169 kW rows only).

---

## Key question 2: DQ381 (0GC). Is there any VR6 clutch housing, and what is HPA's "CNC adaptation"?

### Takeaway
No VR6 DQ381 exists in any source, and no commercial VR6-to-DQ381 adapter was found. The DQ381 also uses a two-piece case with a **0GC 301 107** front housing. HPA's VR550T "CNC adaptation of DQ381 Gearbox" is only available inside the $49,000+ (Golf R) or $64,300+ (Alltrack) labour-inclusive program. No standalone part or price was found.

### Cited Findings
- **VERIFIED (factory manual index)**: "7-speed dual clutch gearbox 0GC (eng.) Workshop Manual" is listed for the A3 8V. — [vwts.ru A3 8V index](https://vwts.ru/audi_a3_8v.html)
- **REPORTED (salvage listing and eBay title via search summaries)**: **0GC301107** appears as the reference on complete used 0GC gearboxes. One eBay title reads "Front housing CASE COVER AUDI VW SKODA [4WD] DQ381 0GC **0GC301107K**" (exact eBay listing not identified). — [ecooparts Tiguan 0GC](https://ecooparts.com/en/used-auto-part/gearbox/volkswagen/tiguan/19941912_gearbox-uay-volkswagen-tiguan-advance-bmt.html)
- **VERIFIED (vendor pages, background file)**: HPA VR550T Golf R includes "CNC adaptation of DQ381 Gearbox", "Upgraded DQ381 DSG with upgraded Clutch Packs" and "Full UDS canbus integration", from $49,000. The Alltrack program adds a "DQ381 compatible drive shaft", from $64,300 labour-inclusive. — [HPA VR550T Golf R](https://www.hpamotorsports.com/pages/hpa-vr550t-2-5l-vr6-program-for-golf-r); [HPA VR550T Alltrack](https://www.hpamotorsports.com/pages/hpa-vr550t-2-5l-vr6-program-for-sportwagen-alltrack)
- **REPORTED (The Drive, search summary)**: HPA uses Chinese 2.5 VR6 **DDKA** engines (551 hp / 748 Nm). The DSG "gets tougher clutch packs". The conversion is "$40,000, not counting the donor Golf R". — [The Drive](https://www.thedrive.com/news/vw-tuner-is-building-turbo-vr6-swapped-mk7-5-golf-rs-with-550-hp)
- **VERIFIED (vendor news page)**: TVS Engineering sells DQ500 conversion kits "for all VAG DQ250, DQ380 and DQ381 equipped vehicles". In other words, the commercial answer to DQ381 limits is to replace the DQ381, not adapt it. — [TVS news](https://tvsengineering.com/en/news/tvs-dq500-conversion-kits-now-available-for-all-dq250-dq380-and-dq381-vehicles/)
- **Searched, nothing found**: "VR6 DQ381 adapter", "DQ381 VR6 bellhousing", HPA DQ381 part listing. The adapter makers found (Key question 5) list DQ500/MQ500 only.

### Inferences
- **INFERRED**: by analogy with the documented DQ500 method (machine the 4/5-cylinder bell, add a VR6 plate or spacer, fit a VR6 10-bolt flywheel with the gearbox-side spline), HPA's "CNC adaptation" most likely machines the 0GC bell to take a VR6 pattern plate, plus a custom DDKA-to-DQ381 flywheel. HPA has not published this.
- **INFERRED**: for an A3/S3 8V, the DQ381 route is strictly a pro-shop job. The DQ500 route (Key question 3) has off-the-shelf adapters and two MQB A1 precedents, so it dominates.

### Gaps
- What HPA physically machines, whether it fabricates a flywheel, and whether HPA would sell the adapted 0GC on its own.
- DQ381 rated torque in VW's own documents (secondary sources: 420–430 Nm, per the background file).

---

## Key question 3: DQ500 (RS3 8V 0DL / TT RS 8S). VR6 versions, what "machined bellhousing" means, which VR6 flywheel fits, and the precedents

### Takeaway
This is the proven route. The RS3/TT RS DQ500 (**0DL**, 600 Nm) is a 4/5-cylinder-bell gearbox. VR6 conversions machine (mill) the DQ500 bellhousing and bolt on a VR6-pattern adapter plate or spacer. They then add a VR6 10-bolt dual-mass flywheel made for the DQ500 input, and a custom transfer-case (PTU) support bracket, because the VR6 block lacks the 4/5-cylinder engine's PTU bracket points.

At least five European vendors sell the adapter and machining (€284 for a plate alone; €550–€760 or £950 with machining). HPA sells a complete kit at US $11,699. Two MQB A1 cars run it:
- **TuneZilla's 2017 S3 8V**: turbo BWS 3.6, RS3/TT RS DQ500 "bell housing machined to mate up to the VR6", VR6 flywheel, AWD retained.
- **HGP's Golf 7 R**: twin-turbo 3.6 with the RS3/TT RS DQ500, 4Motion retained.

"Machined bellhousing" is therefore a re-machined 4/5-cylinder DQ500 bell plus a plate. No source shows a factory VR6 DQ500 bell (Teramont/Talagon) being used.

### Cited Findings
**The RS3/TT RS gearbox**
- **VERIFIED (factory manual index)**: "7-speed dual clutch gearbox **0DL**" repair manual (ed. 11.2019) for "Audi A3 from 2013" and "Audi TT from 2015". The 0DL SSP (Russian, Skoda SSP 115) calls the "7-ступенчатая КПП DSG **0DL (DQ500)**" a wet dual clutch with one shared oil circuit for clutch and Mechatronik, and oil "cooled by a heat exchanger in the engine cooling circuit". The design is rated for "**до 600 Нм**" (up to 600 Nm). Listed for TT Mk3 FV3/FV9 2015–. — [vwts.ru A3 8V index](https://vwts.ru/audi_a3_8v.html); [vwts.ru TT FV index](https://vwts.ru/audi_tt3_fv.html)
- **REPORTED (vendor title, background file)**: "DQ500 7-speed DSG complete service kit Audi 8V/8Y RS3, 8S TT RS". — [NGP](https://store.ngpracing.com/products/dq500-7-speed-dsg-transmission-complete-service-kit-audi-8v-8y-rs3-8s-ttrs)
- **REPORTED (NHTSA bulletin title, background)**: 2019–2020 TTS/TT RS with 0DL or 0GC. — [NHTSA MC-10171334](https://static.nhtsa.gov/odi/tsbs/2020/MC-10171334-0001.pdf)

**Precedent 1: TuneZilla S3 8V** (REPORTED, builder's own videos, from the coordinator's transcript notes)
- 2017 S3 8V quattro with a new European **BWS** 3.6 long block, turbocharged.
- "RS3/TT RS DQ500 7-speed DSG, imported used from Europe. 'We had the bell housing machined to mate up to the VR6, cuz typically they don't mate to the VR6, they're made for the 2.5 L.'"
- A **VR6 flywheel** was ordered (one-month lead time) and clearanced for the main-cap girdle. Stock DQ500 clutches were kept at first.
- Mounts: **RS3 transmission mount** ("the RS3 mount works with the DQ500"), **Atlas 3.6 VR6 engine mount**, **RS3-style dogbone** (the 2.0 one "didn't reach far enough").
- AWD retained through the DQ500 bevel box, prop shaft and Haldex rear.
- ECU: Atlas MED17 ECU with TuneZilla patches.
- Sources: [TuneZilla Road To 1000 Ep 2](https://youtu.be/40MiKU9WxwE); [Shop Vehicle Tour](https://youtu.be/pIoSMRWVuOg); [Drag-strip prep](https://youtu.be/mSBLWcTih2k); local notes `research_notes/Audi A3 8V VR6 with stock gearbox/tunezilla_vr6t_s3_build.md`

**Precedent 2: HGP Golf 7 R** (REPORTED, press via search summaries)
- 3.6 VR6 twin-turbo "coupled to the dual-clutch gearbox from the Audi RS3". — [auto motor und sport](https://www.auto-motor-und-sport.de/tuning/hgp-tuning-vw-golf-7-r-vr6/)
- "seven-speed Audi RS3 DSG", "amended DSG software and a reinforced eight-disc clutch". — [CarThrottle](https://www.carthrottle.com/post/the-735bhp-hgp-vw-golf-r-is-a-v6-bi-turbo-supercar-slayer)
- **Conflict on the donor:** The Drive calls it the "European Audi TTRS's 7-speed DSG DQ500". Both are 0DL-family DQ500s, so this is a naming difference. — [The Drive video page](https://www.thedrive.com/video/3085/transforming-a-volkswagen-into-a-740-horsepower-guided-missile)
- Factory 4Motion retained, with clutches reinforced for close to 1,000 Nm. — [ifanr](https://www.ifanr.com/884085)
- Claimed >550 kW / 925 Nm. — [CarMag](https://www.carmag.co.za/news/this-bi-turbo-vr6-powered-golf-7-r-makes-550-kw/)

**What the conversion vendors machine and supply**
- **VERIFIED (HPA "VR6 7-Speed DSG Conversion (DQ500)")**, $11,699:
  - Pitched at "3.2 VR6 owners"; the DQ500 is "Originally engineered for high-output platforms such as the Audi TT RS and RS3".
  - Includes "**DQ500 bell housing machining and CNC transmission adapters**", a "**DQ500 to VR6 conversion flywheel** w/installation hardware", a "DQ500 transmission assembly w/transfer case", a "**Transfercase bracket** w/installation hardware", a "DQ500 mechatronic", "Full conversion DSG software", a "DQ500 performance clutch assembly w/ OEM clutch basket core", plus mounts, heat shields, cooler hardware, a "shifter cable adapter" and "DQ500 shift cables".
  - Claims "applications exceeding 1000 Nm when properly configured and calibrated".
  — [HPA DQ500 conversion](https://www.hpamotorsports.com/products/dq500-conversion)
- **VERIFIED (Krabifab, €550)**:
  - "Sadly, the DQ500 gearbox didn't come with the VR6 engines and does not fit bolt-on to the engine."
  - Kit = "adapter plates, custom housing machining, and all necessary bolts". "All you have to do is send us your gearbox's bellhousing and we will provide you the spacer since the body needs some machining."
  - Also needs "a 10-bolt flywheel" (their "VR6 DQ500 Dual Mass Flywheel", €550) "and a custom transfer case bracket". The OE wiring harness works.
  — [Krabifab DQ500 adapter](https://www.krabifab.ee/product/dq500-adapter/)
- **VERIFIED (HST Turbotuning, €760 incl. VAT plus shipping, 3–4 weeks)**: "DQ500 conversion suitable for R32/R36/VR6 … we need your gearbox/gearbox bell housing to mill it around in our house and attach an adapter plate". "Gearbox/gearbox bell housing not included in the price." — [HST DQ500 milling and adapter plate](https://eu.hst-tuning.com/en/gearbox/dq500/dq500-milling-and-adapterplate/hstg-dq500-f-ap)
- **REPORTED (Racing Custom Parts, Poland; page behind Cloudflare, search summary)**:
  - "VR6 / R32 / R36 to DSG DQ500 NZS adapter": a one-piece adapter that locates on three gearbox base points, **€600 net / €738 incl. VAT**.
  - "bellhousing machining needed … if you can do it by yourself ask for gearbox shape file; if you can't just send bellhousing to us … price of machining bellhousing 200euro". A centering-sleeve dimension is marked mandatory (text garbled).
  - A Transporter T6 "SDE" variant is listed at the same price.
  - eBay sells "DQ500 Adapter +machining for R32 R36 3.2 3.6" (brand Racing Custom Parts) at US $1,140.62.
  — [RCP NZS adapter](https://racingcustomparts.com/produkt/vr6-r32-r36-to-dsg-dq500-nzs-adapter/); [RCP SDE adapter](https://racingcustomparts.com/produkt/vr6-r32-r36-to-dsg-dq500-sde-adapter-transporter-t4/); [eBay 225780185250](https://www.ebay.com/itm/225780185250)
- **VERIFIED (Boost-Parts, €284 incl. tax)**: "Adapter plate DQ500 MQ500 4-shaft gearbox to VR6 R30 R32", ref. **DQ-VR6-500-ADP01**, "Compatible with VR6 R30, R32, R33, R36 engines", "Ideal for 4-Motion turbo conversions". Racing use only. Machining is not stated. — [Boost-Parts](https://boost-parts.de/en/accesories/1683-adapter-plate-dq500-mq500-4-shaft-gearbox-to-vr6-r30-r32.html)
- **VERIFIED (Deutsche Automotive UK, £950)**:
  - "DQ500-MQ500 R32 R36 VR6 Turbo Machining Service": custom bell-housing modifications plus CNC adapter plates "Complete with a full bolt set".
  - "The price listed requires you to send us your bell housing". Gearbox strip and assembly costs extra.
  - The same page sells a "DQ500 & MQ500 transfer case support bracket for 24v VR6 engines", **£190**, and TVS DQ500 software in "RS3/TTRS" and "Tiguan/Q3/Transporter" variants from £339.
  — [Deutsche Automotive](https://deutsche-automotive.co.uk/product/dq500-mq500-r32-r36-vr6-turbo-machining-service/)
- **REPORTED (title)**: 9T Performance resells the "Krabifab DQ500 VR6 Transmission Adapter Plate". — [9T Performance](https://www.9tperformance.com/products/krabifab-dq500-transmission-mount)

**VR6-to-DQ500 flywheels**
- **VERIFIED (Motorsport Calibrations / Don Octane)**: "VW AUDI R32 3.2 24v VR6 Billet Reinforced Dual Mass Flywheel – 1300nm", SKU **DORFW-R32**, "designed for VW Audi 3.2 24v VR6 Engines when fitted with a 7 speed DQ500 gearbox", "10 Bolt Centre", **£1,300**, on backorder. — [Motorsport Calibrations](https://www.motorsportcalibrations.co.uk/products/r32-billet-flywheel-1300nm)
- **VERIFIED (Krabifab, via its adapter page)**: "VR6 DQ500 Dual Mass Flywheel", €550. — [Krabifab](https://www.krabifab.ee/product/dq500-adapter/)
- **REPORTED (Racing Custom Parts, search summary)**: "VR6/R32/R36 to DQ500 dual mass sport flywheel stage 4", 6.5 kg, **€1,300 net / €1,599 incl. VAT**. — [RCP flywheel](https://racingcustomparts.com/produkt/vr6-r32-r36-to-dq500-dual-mass-sport-flyweel/)

**A factory VR6 DQ500 (China)**
- **REPORTED (Chinese press, background file)**: Teramont 2.5T EA390 V6 (500 Nm) "配以DQ500 DSG七速湿式双离合变速器" (paired with the DQ500 7-speed wet DSG). — [Autohome 2018](https://www.autohome.com.cn/info/201803/913726.html)
  - **Conflict:** Krabifab says "the DQ500 gearbox didn't come with the VR6 engines". It is probably unaware of the China-only Teramont/Talagon. No gearbox code, bell part number or Western availability for a VR6 DQ500 was found.

### Inferences
- **INFERRED, what "machined bellhousing" means:** every vendor that describes the method (HST "mill it around … attach an adapter plate"; Krabifab "housing machining" plus "spacer"; RCP adapter plus "machining bellhousing"; HPA "bell housing machining and CNC transmission adapters"; Deutsche Automotive "bell housing modifications" plus "CNC-machined custom adapter plates") does the same thing. The DQ500's 4/5-cylinder bell flange is milled for clearance and re-faced, and a VR6-pattern plate or spacer is bolted to it. TuneZilla's "bell housing machined to mate up to the VR6" almost certainly means one of these services, not a re-drilled bell or a Teramont bell. The video does not say whether a plate was used.
- **INFERRED, parts set for an A3/S3 8V, following TuneZilla:**
  - **Engine and gearbox:** VR6 (BWS/CDVC/BLV 3.6 or BUB 3.2) and an RS3 8V / TT RS 8S **0DL** DQ500 with its PTU.
  - **Adapter:** bell machining plus VR6 adapter plate (Krabifab, HST, RCP, Deutsche Automotive, or HPA's kit).
  - **Flywheel and PTU support:** VR6 10-bolt DQ500 DMF (Krabifab €550 / Don Octane £1,300 / RCP €1,599); VR6 transfer-case bracket (Deutsche Automotive £190, or included by HPA).
  - **Mounts:** RS3 8V transmission mount, RS3 dogbone, Atlas 3.6 engine-side mount.
  - **Driveline:** RS3 axles and prop-shaft interface (the RS3 is an 8V, so these should be RS3 bolt-ins; unverified).
  - **Software:** DQ500 TCU software for the VR6 torque map (TVS/HPA).
  The adapter and machining are about €550–€950. The flywheel and bracket add about €550–€1,600 and £190. The used RS3 DQ500 itself is unpriced here.
- **INFERRED, why DQ500 beats 0D9 and 0GC:** it is 600 Nm against 350 or 420 Nm. Adapters are commercial. The RS3 is the same 8V body, so its mounts, axles, PTU and prop shaft fit the A3 chassis, and TuneZilla confirms the mounts. Two MQB A1 precedents exist (TuneZilla, HGP).
- **INFERRED, CAN:** the 0DL is an MQB-generation mechatronic, so it should sit on the A3's gateway more naturally than a PQ 02E. TuneZilla still reported "lots of communication errors" before everything talked.

### Gaps
- Whether the adapter plates cover all three DQ500 generations (0BH/0BT Tiguan/T5/T6 vs MQB 0DL). RCP's "NZS"/"SDE" may be gearbox code letters (unverified).
- Starter position with the adapter plate (no vendor states which starter is used).
- Plate thickness, and whether the input-shaft/DMF engagement depth is corrected in the flywheel or the plate.
- Exact HPA, Krabifab or RCP flywheel spline type, and whether they fit the 0DL as well as the 0BH.
- Teramont/Talagon VR6 DQ500 code letters, its bell part number, and whether it is the same bolt pattern as the 3.6. Nothing found.
- Used RS3/TT RS DQ500 price in Canada/US (TuneZilla had to import theirs from Europe).

---

## Key question 4: Manual. Can a VR6 02M/02Q bellhousing go on the MQB 0FB/02Q (Golf R Mk7, Euro S3 8V manual)?

### Takeaway
There is no source for a VR6 bell on an 0FB, and no adapter for it. The 02M/02Q "clutch housing" (part 301 107) is one structural half of the gearbox case, like the DSGs'. FCP Euro says VW "refined the bellhousing spacing and design" on the 0FB. A VR6 02M/02Q bell is therefore not a documented swap onto an 0FB.

The A3 8V manual options are 02Q codes or **0FB (code PDT)**, rated 380 Nm. For a manual VR6 A3, the practical routes are a whole VR6 02M/02Q 4Motion (background file) or an MQ500 with one of the VR6 DQ500/MQ500 adapters above.

### Cited Findings
- **VERIFIED (factory manual index)**: "Gearbox 02Q and 0FB, Workshop Manual" (ed. 06.2014) for A3 8V1/8V7/8VA/8VS.
  - "Механическая коробка передач 0FB имеет меры усиления вблизи выходного вала с 1-й по 4-ю передачу и предназначена для передачи момента до 380 Нм" (the 0FB is reinforced near the output shaft for 1st–4th and rated up to 380 Nm).
  - 0FB code letters: **PDT**.
  - 02Q code letters (shared index): GRF, HDV, GVT, JLU, JLW, JMA, KDN, KDQ, KDS, KNS, KNU, KNY, KXX, KXZ, KZS, LHD, NFP, NFN, FWZ, JLS, JLR, KDX, KDL, KNP, KNQ, KSC, KXU, KXV, LHC, LNN, LNM, NFR, NFQ, PFL, PFN, NBK, PNN, MRV, PFM, PGS, NFU, NGD, KNW, KXY, NFM, NFV, NGC, KRN.
  The same manual is listed for TT Mk3 FV3/FV9. — [vwts.ru A3 8V index](https://vwts.ru/audi_a3_8v.html); [vwts.ru TT FV index](https://vwts.ru/audi_tt3_fv.html)
- **VERIFIED (FCP Euro, background)**: the 0FB is the MQB 02Q; VW "once again refined the bellhousing spacing and design". The 02Q itself had "small changes in the bellhousing design and spacing" vs the 02M. VR6 = 10-bolt crank; 2.0 TSI = 8-bolt flywheel. — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **VERIFIED (catalogue page title)**: oemwolf titles **02G 301 107** "clutch housing". **REPORTED (search summary)**: oemwolf **02Q 301 107** is a "clutch housing" fitting 27 VW Group vehicles 2003–2010. VAG's 301 107 base number is the clutch housing across manual families. — [oemwolf 02G301107](https://oemwolf.com/oem-parts/02g301107.html); [oemwolf 02Q301107](https://oemwolf.com/oem-parts/02q301107.html)
- **VERIFIED (vendor pages)**: Boost-Parts and Deutsche Automotive VR6 adapters are explicitly for "DQ500 **MQ500**" (the manual sibling of the DQ500). HPA sells an "02M to MQ500 conversion" (background: MQ500 has 3 pinions vs 2 in the 02M/02Q). — [Boost-Parts](https://boost-parts.de/en/accesories/1683-adapter-plate-dq500-mq500-4-shaft-gearbox-to-vr6-r30-r32.html); [Deutsche Automotive](https://deutsche-automotive.co.uk/product/dq500-mq500-r32-r36-vr6-turbo-machining-service/); [HPA 02M to MQ500](https://www.hpamotorsports.com/products/02m-to-mq500-conversion)
- **VERIFIED (HPA)**: VR550T "Available in DSG & 6-Speed Manual"; the manual gearbox is not named. — [HPA VR550T Golf R](https://www.hpamotorsports.com/pages/hpa-vr550t-2-5l-vr6-program-for-golf-r)

### Inferences
- **INFERRED**: a VR6 02M/02Q clutch housing on an 0FB would be the same full-split transplant as the DSG case (Key question 1), with the added uncertainty of the 0FB's revised bell spacing and reinforcements. It is not worth attempting when whole VR6 4Motion 02M/02Q boxes exist.
- **INFERRED**: at 380 Nm, an 0FB adapted to a VR6 would cope with a stock 3.6 on paper but not a turbo VR6. MQ500 plus a VR6 adapter is the higher-torque manual route. It is not an A3 8V factory gearbox, so its fit with the A3's mounts, axles and Haldex prop shaft is unknown.

### Gaps
- No source on a VR6-pattern 02Q (EU Mk5 R32 / A3 3.2 / TT 3.2 manual) clutch-housing part number or code letters.
- No MQ500 application list (which vehicles carry it) or MQ500 4Motion PTU interface data.

---

## Key question 5: Commercial VR6 adapters (VR6-to-EA888 / VR6-to-MQB-DSG) and prices

### Takeaway
Every commercial adapter found is VR6-to-**DQ500/MQ500**. None is VR6-to-DQ250 (0D9), VR6-to-DQ381 (0GC) or VR6-to-0FB. The A3's RS3 gearbox is a DQ500, so these adapters are the "A3-family gearbox" solution.

### Cited Findings
| Vendor (country) | Product | Price | What you send / get | Label |
|---|---|---|---|---|
| HPA Motorsports (Canada) | VR6 7-Speed DSG Conversion (DQ500) | US $11,699 | Complete: DQ500 + transfer case, bell machining + CNC adapters, VR6 flywheel, transfer-case bracket, mechatronic, software, clutch, mounts, cables | VERIFIED [HPA](https://www.hpamotorsports.com/products/dq500-conversion) |
| Krabifab (Estonia) | DQ500 Adapter for VR6 | €550 (+ VR6 DQ500 DMF €550) | Send bellhousing; plates + machining + bolts + spacer; needs 10-bolt flywheel and custom transfer-case bracket | VERIFIED [Krabifab](https://www.krabifab.ee/product/dq500-adapter/) |
| HST Turbotuning (Germany) | DQ500 milling and adapterplate (hstg-dq500/f/ap) | €760 incl. VAT + shipping, 3–4 wk | Send gearbox/bell; milled + plate | VERIFIED [HST](https://eu.hst-tuning.com/en/gearbox/dq500/dq500-milling-and-adapterplate/hstg-dq500-f-ap) |
| Racing Custom Parts (Poland) | VR6/R32/R36 to DSG DQ500 NZS (and T6 SDE) adapter | €600 net / €738 incl. VAT + €200 bell machining; eBay "adapter + machining" US $1,140.62 | One-piece plate on 3 base points; DIY machining with their shape file, or send the bell | REPORTED [RCP](https://racingcustomparts.com/produkt/vr6-r32-r36-to-dsg-dq500-nzs-adapter/); [eBay](https://www.ebay.com/itm/225780185250) |
| Deutsche Automotive (UK) | DQ500-MQ500 R32 R36 VR6 Turbo Machining Service | £950 (+ VR6 transfer-case bracket £190) | Send bell; modified bell + CNC plate + bolts | VERIFIED [Deutsche Automotive](https://deutsche-automotive.co.uk/product/dq500-mq500-r32-r36-vr6-turbo-machining-service/) |
| Boost-Parts (Germany) | Adapter plate DQ/MQ500 to VR6 R30/R32/R33/R36, DQ-VR6-500-ADP01 | €284 incl. tax | Plate only; machining not stated | VERIFIED [Boost-Parts](https://boost-parts.de/en/accesories/1683-adapter-plate-dq500-mq500-4-shaft-gearbox-to-vr6-r30-r32.html) |
| TVS Engineering (Netherlands) | DQ500 conversion kits, incl. "3.2 & 3.6L VR6 EA390" Golf Mk5 / TT 8J / A3 8P, and "EA888 Gen3" Golf Mk7 / TT 8S / A3 8V | Price on request | New DQ500, new clutch, new mechatronic, TVS software, "all additional parts needed … (varies by model)"; mating method not stated | VERIFIED [TVS news](https://tvsengineering.com/en/news/tvs-dq500-conversion-kits-now-available-for-all-dq250-dq380-and-dq381-vehicles/); [TVS product page](https://tvsengineering.com/en/product/dsg-conversion-kit/) |

- **VERIFIED (vendor page)**: Don Octane VR6 DQ500 DMF DORFW-R32, £1,300. — [Motorsport Calibrations](https://www.motorsportcalibrations.co.uk/products/r32-billet-flywheel-1300nm)
- **Not relevant (VERIFIED titles via search)**: 9T Performance's VR6 adapter is for longitudinal Audi manuals (01E/02X/0A3). Domi-Works' VR6 3.2/3.6 adapter goes to BMW 8HP. — [9T longitudinal plate](https://www.9tperformance.com/products/audi-transmission-adapter-plate-longitudinal-vr6-swap); [Domi-Works](https://www.domi-works.com/products/vw-vr6-3-2-3-6-bmw-8hp-45-50-51-70-75-76-n47-n57-b57-b58-s58-adapter-kit)
- **Searched, nothing found**: Kennedy Engineering, Collins Adapters, KEP, Epytec (Epytec sells DQ250 *mounts* and axles for VR6 conversions, not bell adapters), DSG Tech and Polish/Russian VR6-to-DQ250/DQ381 adapters.

### Inferences
- **INFERRED**: the TVS listing of a "3.2 & 3.6L VR6 EA390" DQ500 kit for PQ35 cars (Golf Mk5/TT 8J/A3 8P) implies TVS also has a VR6-to-DQ500 mating solution (adapter or machined bell). Ask TVS whether that kit carries over to an A3 8V body.
- **INFERRED, cheapest credible DIY bundle:** Krabifab adapter €550 + Krabifab DMF €550 + Deutsche Automotive transfer-case bracket £190 ≈ €1,320 before shipping and VAT. That is about one-ninth of HPA's complete $11,699 kit, which includes the gearbox, mechatronic and software.

### Gaps
- No North American adapter maker other than HPA, which sells complete kits only.
- Adapter compatibility with the MQB 0DL specifically (vs 0BH/0BT) is not stated by any vendor.

---

## Key question 6: Which VR6 engines share the VR6 bell pattern and crank flange, and which drive plates/flywheels fit the DSG applications?

### Takeaway
The 24V 2.8, 3.2 (BUB/CBRA/BDB/BMJ) and 3.6 (BLV/BWS/CDVB/CDVC) are treated by every vendor as one bell and crank family: 10-bolt crank, the same 02E DSG DMF across 3.2 and 3.6, and the same DQ500 adapters for "VR6/R32/R36". The VR6 02E DSG DMF is **022 105 266 AH** (Audi A3/TT 3.2) / **022 105 266 AK** (VW R32/CC/Eos/Passat 3.2/3.6), LuK **415 0755 09**. It fits 02E, not DQ500 (DQ500 needs the DORFW-R32 / Krabifab / RCP units). No source confirms that the 12V VR6 or the Chinese 2.5T DDKA uses the same bell pattern.

### Cited Findings
- **VERIFIED (FCP Euro, background)**: "VR6 powered cars … have a 10-bolt crank"; 1.8T has a 6-bolt crank; 2.0T TSI an 8-bolt flywheel. — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **REPORTED (build, background)**: a Mk4 24V 02M bolted straight to a BLV 3.6 (Ninety4co, running car). — `research_notes/Mk6 Jetta CDVC VR6 swap parts/manual_02m_transmission.md`
- **VERIFIED (vendor page)**: DMF "415075509 022105266AH" fitment covers A3 8P 3.2 (BDB, BMJ, BUB), TT 8J/8N 3.2 (BUB, BHE, BPF, CBR), Golf R32 Mk4/Mk5, **VW CC 3.6**, Eos 3.2/3.6, **Passat/R36 B6/B7 3.2 and 3.6**, Skoda Superb 3.6. Cross-references 022 105 266 AK. Mapping: "Audi TT, A3: 022105266AH", "VW CC, Eos, Passat, Golf: 022105266AK". US $349.99. DSG vs manual not stated on the page. — [FridayParts](https://www.fridayparts.com/dual-mass-flywheel-415075509-022105266ah-for-vw-cc-golf-r32-audi-a3-tt-3-2-3-6-vr6)
- **REPORTED (listing title and price, search summaries)**: "OEM VW DSG Flywheel Mk5 R32 Audi A3 2.8L 3.2L Dual Mass **022105266AK**". FCP Euro lists "Audi VW Dual Clutch Flywheel – LuK 022105266AK" at $857.99. The manual R32 DMF is LuK DMF057, a different part. — [eBay 290689210280](https://www.ebay.com/itm/290689210280); [FCP Euro flywheels](https://www.fcpeuro.com/filters/Volkswagen-parts/Flywheel/); [PartsHawk DMF057](https://partshawk.com/volkswagen-r32-clutch-flywheel-luk-dmf057.html)
- **VERIFIED (vendor pages)**:
  - DQ500 adapters are sold as one item for "VR6 R30, R32, R33, R36" (Boost-Parts), "R32/R36/VR6" (HST) and "VR6/R32/R36" (RCP).
  - TVS groups "3.2 & 3.6L VR6 EA390".
  - The DQ500 DMF is a "10 Bolt Centre" for "3.2 24v VR6" (Don Octane).
  — [Boost-Parts](https://boost-parts.de/en/accesories/1683-adapter-plate-dq500-mq500-4-shaft-gearbox-to-vr6-r30-r32.html); [HST](https://eu.hst-tuning.com/en/gearbox/dq500/dq500-milling-and-adapterplate/hstg-dq500-f-ap); [TVS](https://tvsengineering.com/en/news/tvs-dq500-conversion-kits-now-available-for-all-dq250-dq380-and-dq381-vehicles/); [Motorsport Calibrations](https://www.motorsportcalibrations.co.uk/products/r32-billet-flywheel-1300nm)
- **REPORTED (TuneZilla)**: a BWS 3.6 took the VR6 DQ500 adapter and flywheel route. — [TuneZilla Ep 2](https://youtu.be/40MiKU9WxwE)

### Inferences
- **INFERRED**: any 24V 2.8/3.2/3.6 (including the NA CDVC/CDVB/BLV and EU BWS) will take the same DQ500 adapter and 10-bolt DQ500 flywheel. That is the only DSG-adapter interface the vendors offer.
- **INFERRED**: the 022 105 266 AH/AK DMF is the part to use only when running a VR6 02E (whole R32/TT 3.2/A3 3.2/Passat box, or the theoretical VR6-02E-front-case-on-0D9 hybrid). It does not fit a DQ500, because each vendor sells a separate "VR6-to-DQ500" DMF.
- **INFERRED**: the 2.5T DDKA ran with a CNC-adapted DQ381 (HPA) and, in China, a DQ500. Its bell pattern relative to the 3.6 is unknown.

### Gaps
- 12V VR6 (AAA/ABV) crank flange bolt count and bell pattern vs 24V. Not sourced.
- DDKA/DPK (2.5T) bell pattern and crank flange. Not sourced.
- The NMS Passat CDVB 02E drive-plate part number (likely within the 022 105 266 AK family per FridayParts' 3.6 fitment; not catalogue-confirmed).

---

## Key question 7: Audi TT gearboxes. TT 8J 3.2 quattro (02E S tronic and manual), and TT 8S / TT RS 8S

### Takeaway
1. **TT 8J 3.2 quattro (NA 2008–2009):** offered with a 6-speed S tronic (VR6 **02E** DQ250-6A, PQ35 J743 mechatronic) or a 6-speed manual. FCP Euro says the NA manual is a VR6 **02M** 4Motion; a factory index lists **02Q** codes for the TT 8J. Neither box is a good whole-gearbox choice for an A3 8V:
   - PQ35 mechatronic and CAN;
   - a 6-cylinder star-flange output;
   - a PQ35 angle drive and an early-generation Haldex prop shaft, with no Haldex 5 match.
   The TT 3.2 S tronic is a logical **donor of a VR6 4WD 02E front case (02E 301 107, suffix unknown)** for the VR6-bell-on-0D9 hybrid. The only documented hybrid (Dewain, Mk7 Golf R, 2021) used an MKV R32 DSG bell instead.
2. **TT 8S (2015/16–2023) and TT RS 8S:** the same families as the A3/S3/RS3: 0D9 DQ250 / 0GC DQ381 (TT/TTS), **0DL DQ500** (TT RS), and the 02Q/0FB manual. All have 4/5-cylinder bells and no VR6 bell. The TT RS 8S DQ500 is the gearbox TuneZilla and HGP adapted.

### Cited Findings
**TT 8J 3.2**
- **VERIFIED (factory manual index, TT 8J)**: the TT 8J page lists the 02E (DSG) oil change. It lists the 02E S tronic SSP covering A3 8P / TT 8J / TT 8N, J743, "Распределение момента на полноприводных автомобилях, Угловой редуктор" (torque distribution in AWD cars, angle drive). It lists "Audi TT 2007 → 6-speed manual gearbox 02Q" with code letters **JLV, JYV, KDP, KNT, KZN** "for VW Golf 5 / Jetta 5 (1K), VW Eos (1F), Audi A3 (8P), Audi TT (8J)". Which engines these codes go with is not stated. — [vwts.ru TT 8J index](https://vwts.ru/audi_tt_8j.html)
- **VERIFIED (FCP Euro, background)**: NA 02M applications include "2008–2009 Audi Mk2 TT 3.2 VR6 quattro". **Conflict** with the 02Q listing above (possibly market- or engine-specific). — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **REPORTED (TT Forum, search summary)**: the TT 3.2 VR6 carries the 02E "DQ250-6F/6Q", not the 0D9. The poster was correcting an AI answer and cited Ross-Tech's transmission category. — [TT Forum 2040942](https://www.ttforum.co.uk/threads/which-dq250-does-the-3-2-vr6-carry.2040942/)
- **REPORTED (press, search summary)**: "the TT 3.2 models equipped with S tronic gearboxes have a base price $1,400 higher than manual transmission cars" (2008 US pricing). — [Autoblog](https://www.autoblog.com/2007/01/29/audi-prices-2008-tt/)
- **REPORTED (retail listings, search summary; dates uncertain)**: US 2008–2009 TT 3.2 automatics were listed at about **$7,529–$12,190** (97k–135k mi); manuals at **$15,699–$17,856**. KBB fair purchase price for a 2008 TT 3.2 quattro roadster was $8,300. UK 2008 3.2 S tronic £6,995. No Canadian listings or used-gearbox-only prices were found. — [KBB TT 3.2 listings](https://www.kbb.com/cars-for-sale/used/audi/tt/3-2); [TrueCar TT 3.2L](https://www.truecar.com/used-cars-for-sale/listings/audi/tt/?trim=3-2l); [Parkers](https://parkers.co.uk/audi/tt/for-sale/engine-32)
- **REPORTED (eBay listing page opened, engine not stated)**: "08 Audi TT Mk2 Auto … Trans Assembly 02E301107". — [eBay 2112956159](https://www.ebay.com/p/2112956159)
- **VERIFIED (FridayParts)**: TT 8J 3.2 engine codes BUB/CBR (CBRA) with DMF 022 105 266 AH. — [FridayParts](https://www.fridayparts.com/dual-mass-flywheel-415075509-022105266ah-for-vw-cc-golf-r32-audi-a3-tt-3-2-3-6-vr6)
- **REPORTED/VERIFIED (background file)**:
  - Haldex Gen 2 service kit lists the "Audi 8J TT … 3.2L" (conflicting Gen 4 attribution elsewhere).
  - The HPA Gen 5 controller excludes the TT.
  - 6-cylinder 02E has star-flange/tripod outputs.
  — [NGP Gen2 kit](https://store.ngpracing.com/products/haldex-gen2-service-kit-vw-mk5-r32-b6-passat-audi-8j-tt-8p-a3-3-2l); [HPA Gen 5](https://www.hpamotorsports.com/products/gen-5-performance-haldex-controller); [Epytec ISP106](https://epytec.de/en/drive-shaft-vw-golf-mk2-mk3-corrado-passat-vr6-axle-conversion-02m-02q-dq250-dsg-6-speed-isp106)
- **VERIFIED (vendor page)**: TVS's DQ500 kit list includes "3.2 & 3.6L VR6 EA390 … Audi TT MK2 (8J)". A TT 3.2 owner can buy a VR6-to-DQ500 kit from TVS. — [TVS](https://tvsengineering.com/en/news/tvs-dq500-conversion-kits-now-available-for-all-dq250-dq380-and-dq381-vehicles/)

**TT 8S / TT RS 8S**
- **VERIFIED (factory manual index, TT FV)**: "7-speed dual clutch gearbox 0DL … Audi TT from 2015"; the 0DL (DQ500) SSP lists "Audi TT Mk3 (FV3, FV9) 2015–". "Gearbox 02Q and 0FB" (0FB code **PDT**) is listed for "Audi TT Mk3 (FV3, FV9)". — [vwts.ru TT FV index](https://vwts.ru/audi_tt3_fv.html)
- **VERIFIED (vendor fitment)**: the DQ250 clutch pack 02E398029C fits "TT/TTS Coupe/Roadster (8S), 2015 onward". The TT/TTS 8S DSG is a DQ250 (0D9). — [vagparts 02E398029C](https://vagparts.com.au/products/02e398029c-clutch-service-kit)
- **REPORTED (bulletin title, background)**: 2019–2020 TTS/TT RS with 0DL or 0GC. — [NHTSA MC-10171334](https://static.nhtsa.gov/odi/tsbs/2020/MC-10171334-0001.pdf)
- **REPORTED (vendor title, background)**: DQ500 service kit "8V/8Y RS3, 8S TT RS". — [NGP DQ500 kit](https://store.ngpracing.com/products/dq500-7-speed-dsg-transmission-complete-service-kit-audi-8v-8y-rs3-8s-ttrs)

### Inferences
- **INFERRED, using a TT 8J 3.2 gearbox whole in an A3/S3 8V:**
  - Bell: fits a VR6.
  - Electrics: the PQ35 J743 needs a CAN bridge into MQB.
  - Driveline: the 02E angle-drive output needs a custom prop-shaft front section to reach the A3's Haldex 5. The VR6 02E's star-flange/tripod outputs need custom or hybrid axles.
  - Torque: 350 Nm, at the stock-3.6 limit.
  - Mounts: unknown vs the 8V.
  It ranks below the RS3 DQ500 route on every count except bell fit.
- **INFERRED, the TT 3.2 as a bell donor:** it is the only North American source of a **4WD VR6 02E front case** (the US R32 Mk5 is the other). It is a suitable donor for the VR6-02E-front-case-on-0D9 hybrid, with all the Key question 1 caveats. Dewain's Mk7 Golf R used an MKV R32 DSG bell on the factory Mk7 DSG, so the R32 is a proven donor type. A whole TT 3.2 S tronic plus a used 0D9 would both have to be bought.
- **INFERRED, TT 8J 3.2 manual:** whichever code it is (02M per FCP, or a 4Motion 02Q), it is a VR6-bell 4Motion manual and the same "whole VR6 manual" option described in the background file. The 2008–09 TT 3.2 is the newest NA source of one.
- **INFERRED, TT 8S:** no VR6 path of its own. Its TT RS 0DL is interchangeable in purpose with the RS3 8V 0DL as the adapter base.

### Gaps
- TT 8J 3.2 S tronic gearbox code letters and its 02E 301 107 front-case suffix.
- Resolution of 02M vs 02Q for the NA TT 3.2 manual (read the gearbox code on any candidate).
- Used gearbox-only prices (US/Canada) for a TT 3.2 S tronic or manual. Not found; only whole-car asking prices.

---

## Key question 8: Do the A3/S3/RS3/TT RS gearboxes share one 4/5-cylinder bell pattern, and can the VW 2.5 inline-5 (07K) use them?

### Takeaway
1. **Shared 4/5-cylinder bell pattern: strongly suggested, not catalogue-proven.**
   - The DQ500 family sits behind both 2.0 TSI/TDI four-cylinders (Tiguan, Q3, Transporter, Arteon) and the 2.5 TFSI five (RS3/TT RS).
   - Tuners sell one software family for "RS3/TTRS" and "Tiguan/Q3/Transporter" DQ500s.
   - TVS sells "plug & play" DQ500 kits for EA888 Gen3 A3 8V/Golf 7 cars.
   - TuneZilla describes the DQ500 as "made for the 2.5 L" while the S3's own boxes are 2.0 boxes.
   I found no document that states the pattern outright.
2. **NA 2.5 07K (BGP/BGQ/CBTA/CBUA/CCCA): no MQB DSG precedent.** Forum sources say:
   - the NA 07K has a **6-bolt** crank flange like the 1.8T;
   - the TT RS/RS3 2.5 TFSI crank is **8-bolt**, like the 2.0 TSI flywheel.
   Any 8-bolt EA888 or 2.5 TFSI DSG flywheel will therefore not bolt to a 6-bolt 07K crank without an 8-bolt TT RS/RS3 crank (reported at about $1,300–1,500) or a custom flywheel.
3. **No 07K-into-MQB (Golf 7 / A3 8V) build was found.**

### Cited Findings
- **REPORTED (Honest John, background file)**: the DQ500 (0BH/0BT) is used with "2.0 litre four-cylinder petrol and diesel engines and 2.5 litre five-cylinder petrol engines", mainly the Tiguan and Audi Q3. — [Honest John](https://good-garage-guide.honestjohn.co.uk/askhj/answer/112154/are-there-any-reliable-dsg-transmissions-used-by-volkswagen-)
- **VERIFIED (vendor page)**: TVS DQ500 software is sold in "RS3/TTRS" and "Tiguan/Q3/Transporter" variants (same gearbox family across 5-cylinder and 4-cylinder). — [Deutsche Automotive](https://deutsche-automotive.co.uk/product/dq500-mq500-r32-r36-vr6-turbo-machining-service/)
- **VERIFIED (vendor page)**: TVS DQ500 conversion kits list "2.0 T(F)SI EA888 Gen3: Golf MK7 (5G), Audi TT MK3 (FV/8S), Audi A3 MK3 (8V)". Contents: "New DQ500 gearbox, New clutch, New mechatronic, TVS conversion software". No adapter is mentioned for the EA888 rows, while VR6 rows sit in their own group. — [TVS](https://tvsengineering.com/en/news/tvs-dq500-conversion-kits-now-available-for-all-dq250-dq380-and-dq381-vehicles/)
- **VERIFIED (factory manual index, background)**: "Transmission 0GC 7 speed (DQ381-7A)" is listed with EA888 engines DKFA, DTFA, DCGA. The 0D9 is listed with 2.0 TFSI/TDI (Key question 1). — [vwts.ru Teramont index](https://vwts.ru/vw_teramont_0a.html); [vwts.ru A3 8V](https://vwts.ru/audi_a3_8v.html)
- **REPORTED (TuneZilla)**: RS3/TT RS DQ500s "typically … don't mate to the VR6, they're made for the 2.5 L". — [TuneZilla Ep 2](https://youtu.be/40MiKU9WxwE)
- **REPORTED (press, search summary)**: MTR Performance's Golf R took the RS3's 2.5 TFSI (DAZA) with the DQ500 and an RS3 rear subframe. The 5-cylinder and DQ500 went in together as a package. — [The Drive](https://www.thedrive.com/news/21908/a-volkswagen-golf-r-with-a-591-hp-audi-rs3-engine-is-nearly-perfect)
- **REPORTED (GRM forum, search summary)**: "If you get one without the forged crank (**6 bolt flange** for flywheel) you can buy a **TTRS/RS3 one (8 bolt flange)** for about $1300." — [GRM 2.5 five thread](https://grassrootsmotorsports.com/forum/grm/audis-seemingly-indestructible-25l-tsfi-five/194963/page1)
- **REPORTED (Audizine 07K swap thread, search summary)**: "1.8T flywheels are the same bolt pattern as the 07K"; "Only 07K105101E cranks are forged, only exception … is the $1500 TTRS crank". In a longitudinal (Vanagon-type) swap, an "01E transmission can be used but bell housing needs to be cut/trimmed because of the hump for the vacuum pump". The 07K bell face matches an Audi longitudinal 4/5-cylinder gearbox pattern apart from clearance. — [Audizine 07K turbo swap](https://audizine.com/forum/showthread.php/904241-07K-Turbo-swap-any-takers)
- **VERIFIED (FCP Euro, background)**: 1.8T = 6-bolt crank; 2.0 TSI = 8-bolt flywheel. — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **REPORTED (vendor snippets)**: NA Mk5 2.5 manual cars have a ~23 lb factory DMF; ECS sells a 16.4 lb single-mass flywheel for 07K Mk5s. BFI's 2.5L 228 mm clutch/flywheel kit "Does not fit 02Q 6-speed transmission equipped vehicles". The NA 2.5 clutch kits are 5-speed (0A4-type) applications. — [ECS 07K flywheel](https://www.ecstuning.com/b-ecs-parts/mk5-25l-flywheel/054650la01~a/); [BFI 2.5L kit](https://blackforestindustries.com/products/bfi-2-5l-228mm-clutch-kit-and-lightweight-flywheel-stage-3)
- **REPORTED (forum snippet)**: in an MQB DQ200 swap a poster found "the R flywheel has 8 bolts rather than 6". Flywheel bolt counts vary even within MQB engines. — [SEAT Cupra forum thread](https://seatcupra.net/forums/goto/post?id=5044049)
- **Searched, nothing found**: a 07K + 02Q 6-speed swap write-up with parts; any 07K (or CBTA/CBUA) swap into a Golf 7 / A3 8V; any DSG flywheel listed for a 6-bolt 07K crank; 07K starter compatibility with MQB DSGs.

### Inferences
- **INFERRED**: the A3/S3 (0D9, 0GC), RS3/TT RS (0DL) and MQB manual (02Q/0FB) almost certainly share the VW/Audi transverse 4/5-cylinder bell family. Without that, TVS could not list a "new DQ500 gearbox" kit without an adapter for EA888 A3 8V/Golf 7 cars, and DQ500 software could not span RS3 and Tiguan. Small casting variations (dowels, starter boss, PTU bracket points) may still differ. TuneZilla's "made for the 2.5 L" is consistent with this.
- **INFERRED, 07K on an MQB DSG:** the bell face probably matches (same family; an Audi longitudinal 01E bell fits with trimming). The blockers are the **crank-to-flywheel interface**: 6-bolt NA 07K vs 8-bolt DSG flywheels. One fix is an 8-bolt TT RS/RS3 crank (~$1,300–1,500 reported) so an RS3/TT RS DQ500 DMF can be used; the other is a custom 6-bolt DSG flywheel. No vendor lists such a flywheel. Starter fit and PTU bracket points are unverified.
- **INFERRED, relevance to this project:** the 07K is not a VR6, so its value here is only as evidence that the A3's gearboxes are 4/5-cylinder pattern. That pattern is why every VR6 route onto an A3-family gearbox needs machining and an adapter.

### Gaps
- No catalogue or drawing that states the EA888 vs EA855 vs 07K bell bolt pattern, dowels or starter location.
- NA 07K (BGP/BGQ/CBTA/CBUA/CCCA) crank flange bolt count from a catalogue (only forum claims), and whether all NA 07Ks are 6-bolt or only the forged-crank ones.
- Which gearboxes the NA 07K shipped with (0A4 5-speed / 09G 6-speed auto are commonly cited, but no source was opened in this pass).
- No 07K-to-MQB or 07K-to-DSG precedent of any kind.

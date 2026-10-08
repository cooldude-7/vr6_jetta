# Transmission and AWD driveline behind a transverse 3.6 VR6 (EA390) in a 2015–2020 Audi A3 8V quattro (MQB A1, Haldex 5): VR6-pattern gearboxes, controllers, Haldex 5, manual + AWD, and the most realistic combination

Research date: 2026-10-08. Scope: North American vehicles where possible; EU/China parts noted only where they are the only VR6-pattern option. Background read first and **not repeated**: `research_notes/Mk6 Jetta CDVC VR6 swap parts/manual_02m_transmission.md` (02M/02Q bellhousing facts, FCP Euro MQ350 guide, Epytec 4Motion-to-FWD kit 698, clutch/flywheel, LSD, slave cylinder) and `precedents_vendors_salvage.md` / `engine_ecu_immobilizer.md` in the same folder (R32-DSG-to-3.6 reports, HPA/AW Racing DQ500 turbo builds, engine code CDVB (NMS Passat) vs CDVC (Atlas), Atlas ECU 03H 906 026 E MED17.1.62).

Labels: **VERIFIED** = parts catalog, factory document (or an index of factory manuals), or vendor product page actually opened; **REPORTED** = forum/build thread, press, encyclopedia, or vendor/catalog text seen only in a search-engine summary (page not opened); **INFERRED** = my reasoning. No part number below is invented; numbers I could not source are listed under Gaps.

Access notes: audiworld.com returned 403 to WebFetch and "error code 1005" to curl, so the only A3 2-pedal-to-3-pedal build is REPORTED from search snippets. oemwolf.com search works only with `?search=<exact number>` and returned nothing for 09P/0CQ/0D9/0BH numbers; parts.vw.com returned a Cloudflare challenge. YouTube not used.

---

## Key question 1: Which transverse gearboxes have the VR6 bellhousing, and what are their codes, torque ratings, AWD/PTU availability, controller generation, flanges and prices?

### Takeaway
Five families come with a VR6 bellhousing from the factory: (a) the **Atlas Aisin 8-speed 09P (AQ450)**, in FWD and AWD 3.6 versions with their own code letters (FWD QVJ/TYT, AWD QVK/TYF); (b) the **02E DQ250** 6-speed wet DSG in 6-cylinder form (Mk4/Mk5 R32, A3 8P 3.2, TT 3.2, Passat 3.2/3.6), which has a 6-cylinder-specific star-flange/tripod output; (c) a **DQ500** 7-speed wet DSG behind the Chinese **Teramont/Talagon 2.5T VR6** (China-only; code not found); (d) the **02M/02Q 6-speed manuals** in VR6 form (Mk4 R32 02M 4Motion and Mk2 TT 3.2 02M quattro in NA; Mk5 R32 manual in EU); (e) the **Aisin 09G/09M** 6-speed automatics (B6 Passat 3.6 FWD/4Motion). Only two of these have controllers built for MQB CAN: the Atlas 09P and, by inference, the Teramont DQ500. The manuals have no TCU at all. A third route exists only as a pro-shop job: HPA's "CNC adaptation" of the MQB DQ381 to a VR6.

### Cited Findings
**(a) Atlas 8-speed Aisin, 09P / AQ450**
- **VERIFIED (index of VW factory repair manuals)**: "8-Speed Automatic Transmission 09P (AQ450)". Code letters: **FWD, 3.6 L 206 kW: QVJ, TYT**. **AWD, 3.6 L 206 kW: QVK, TYF**. FWD 2.0 L 175 kW: QVL, TYG. AWD 2.0 L 162 kW: RGZ. Separate entries: "Diagnostics engine CDVC and 8 speed Transmission 09P (AQ450-8F)" and "Diagnostics engine CDVC and 8 speed transmission AQ-450-8A/F 09P (2022 MY)". There is a separate "Rear Final Drive" manual whose contents list "All Wheel Drive Clutch Oil". — [vwts.ru Atlas/Teramont manual index](https://vwts.ru/vw_teramont_0a.html)
- **VERIFIED (vendor page, NGP Racing)**: "VW Audi 09P/AQ450 8 Speed Automatic Transmission Service Kit", SKU 09P-SRV-KIT, **$279.99** (now NLA, superseded by an "MQB Tiguan, Arteon, Atlas" kit). Fits 2018+ Tiguan 2.0T, **2018+ Atlas 2.0T and 3.6L**, 2019–2021 Arteon and 2019–2023 Q3 F3. Contents: **7 × 1 L Liqui Moly Top Tec ATF 1800**, OE filter, pan gasket, drain plug and washer. — [NGP 09P kit](https://store.ngpracing.com/collections/dsg-system/products/vw-audi-09p-aq450-8-speed-automatic-transmission-service-kit)
- **REPORTED (eBay listing, search summary)**: used "2018–2023 Volkswagen Atlas 3.6L 4Motion automatic transmission assembly", Grade B, about 67K miles, "FITS ONLY FOR 4MOTION, 3.6L", 8 speeds. The part-number fields read **09P300036A, 09P323571L, 09P321107**. These are seller-entered and not catalog-checked. Price was not captured. — [eBay 198230786141](https://www.ebay.com/itm/198230786141)
- **REPORTED (press)**: both the VR6 and the 2.0T Atlas use an Aisin 8-speed automatic with a manual mode. — [doubleclutch.ca](https://doubleclutch.ca/?p=42942); [uscar-trader](https://www.uscar-trader.com/en/magazine/vw-atlas-buying-prices-and-more/)
- **REPORTED (NHTSA-hosted VW bulletins, search snippets only)**: a 2017 bulletin for the 2018 Atlas gives an AQ450 software update for "smoothing the shift operation, driveshaft protection and transmission emergency mode". A 2025 Atlas bulletin names the TCM as **J217** ("Transmission Control Module -J217-, DTC P0613 S/W Update"). I did not confirm which of the two 2017 PDFs in the results carries the AQ450 text. — [NHTSA MC-10128427](https://static.nhtsa.gov/odi/tsbs/2017/MC-10128427-9999.pdf); [NHTSA MC-11021375](https://static.nhtsa.gov/odi/tsbs/2025/MC-11021375-0001.pdf)
- **REPORTED (vendor news title)**: "VAG 8-speed Aisin AQ450 now live via OBD on the tool", meaning the 09P TCU can be flashed over OBD with a commercial tool. — [Autotuner](https://us.autotuner.com/blogs/news/vag-8-speed-aisin-aq450-now-live-via-obd-on-the-tool)
- **VERIFIED (vendor page, HPA)**: HPA's Gen 5 Haldex controller is sold for "all VAG MQB vehicles with Haldex AWD", and its fitment list includes **Atlas 2018–2022**. The Atlas 4Motion is therefore an MQB car with the same Gen 5 Haldex controller family as the A3 8V (part numbers in Key question 3). — [HPA Gen 5 controller](https://www.hpamotorsports.com/products/gen-5-performance-haldex-controller)

**(b) 02E DQ250 in VR6 form**
- **REPORTED (Wikipedia)**: "It has been paired to engines with up to 350 N⋅m (260 lb⋅ft)". The page's own variant table says 400 N·m, so it contradicts itself. "The DQ250 comes in a 6F variant for FWD and a -6A variant for AWD". The first DSG went into the German-market Golf Mk4 R32 and the original Audi TT 3.2. — [Wikipedia DSG](https://en.wikipedia.org/wiki/Direct-shift_gearbox)
- **VERIFIED (Epytec vendor page, cited in background file)**: "The DQ250 gearboxes, which are installed in conjunction with the 6-cylinder engines, have a **star-shaped flange and a tripod joint**", which is incompatible with the bolt-on (4-cylinder 02E/02M/02Q) driveshafts. — [Epytec ISP106](https://epytec.de/en/drive-shaft-vw-golf-mk2-mk3-corrado-passat-vr6-axle-conversion-02m-02q-dq250-dsg-6-speed-isp106)
- **REPORTED (vendor snippets)**: Quaife's ATB covers "VAG models fitted with the 02E DSG gearboxes in both two and four wheel drive formats". Another LSD listing "fits 02E 4wd DSG Golf 5 R32 Transmission Only" and tells buyers to check the gearbox code first. — [Quaife 02E](https://www.quaife.co.uk/new-quaife-atb-differentials-for-vag-02e-dsg-models/); [AwesomeGTI Mk5 differentials](https://www.awesomegti.com/shop-by-car/volkswagen/golf-mk5/differentials)
- **REPORTED (vendor title)**: "Haldex Gen2 service kit VW Mk5 R32, B6 Passat, Audi 8J TT, 8P A3 3.2L". The PQ35/PQ46 VR6 4Motion cars use an earlier Haldex generation, not Gen 5. **Conflict:** another retailer is summarised as listing the 2008 Mk5 R32 under a **Gen 4** kit. — [NGP Gen2 kit](https://store.ngpracing.com/products/haldex-gen2-service-kit-vw-mk5-r32-b6-passat-audi-8j-tt-8p-a3-3-2l); conflicting summary via [AwesomeGTI](https://www.awesomegti.com/shop-by-car/volkswagen/golf-mk5/differentials)
- **REPORTED (background file, VWVortex snippets)**: a Mk5 R32 DSG "should bolt up to the 3.6". The DSG mechatronic **J743** and selector J587 sit on the PQ drivetrain CAN and are wired differently from an 09G/09M TCM. The NMS Passat 3.6 02E is FWD only. — `precedents_vendors_salvage.md` (VWVortex 8929969, 7143344)
- **REPORTED (press)**: the Mk5 R32 was sold with "either a six-speed manual or double clutch transmission". — [australiancar.reviews Mk5 R32](https://australiancar.reviews/review-volkswagen-mk-5-golf-r32-2006-10/)

**(c) DQ500 with a VR6 bellhousing (China)**
- **REPORTED (Chinese press via search summary)**: launch material says the Teramont carries the world-first **EA390 2.5T V6** (500 N·m, 220 kW) "配以**DQ500** DSG七速湿式双离合变速器", that is, paired with the DQ500 7-speed wet DSG. The 2019 "530 V6 四驱旗舰版" (530 V6 AWD flagship) is front-engined AWD with a 7-speed DSG. — [Autohome 2018](https://www.autohome.com.cn/info/201803/913726.html); [Autohome 2021](https://www.autohome.com.cn/news/202106/1165913.html)
- **REPORTED (encyclopedia/press)**: Talagon 530 V6 is EA390 **DPK**, 220 kW, 7-speed DSG. The Teramont/Talagon 2.5 V6 makes 299 PS / 500 Nm through a "seven-speed DSG and 4Motion all-wheel drive". **Conflict:** HPA/The Drive call the Chinese 2.5 VR6 **DDKA**. — [Wikipedia Talagon](https://en.wikipedia.org/wiki/Volkswagen_Talagon); [paultan](https://paultan.org/2021/04/22/volkswagen-talagon-suv-debuts-in-china); [The Drive](https://www.thedrive.com/news/vw-tuner-is-building-turbo-vr6-swapped-mk7-5-golf-rs-with-550-hp)
- **REPORTED**: the DQ500 is rated **600 Nm**, with codes **0BH/0BT**. Its listed applications are 4-cylinder petrol/diesel and the 2.5 **five**-cylinder (TT RS, RS3); the T5 Transporter DQ500 is a 2.0 TDI. No Western source lists a VR6 DQ500. — [Honest John](https://good-garage-guide.honestjohn.co.uk/askhj/answer/112154/are-there-any-reliable-dsg-transmissions-used-by-volkswagen-); [Wikipedia DSG](https://en.wikipedia.org/wiki/Direct-shift_gearbox)

**(d) 02M/02Q manuals in VR6 form**
- **VERIFIED (FCP Euro, also in background file)**: NA VR6-pattern 4Motion manuals are the **2004 Golf R32 02M** and the **2008–2009 Audi Mk2 TT 3.2 VR6 quattro 02M**. "The 02M is available in both front-wheel drive and all-wheel drive variants", the AWD models "utilizing an outboard transfer case" (the angle drive bolts to the gearbox). Factory rating is "258 lb-ft", and the box is "easily handling 350-400 lb-ft" if not abused. The **0FB** is the MQB revision of the 02Q found in the "2015 and up Golf R in the USA"; VW "once again refined the bellhousing spacing and design", and it is "more or less mechanically identical to the 02Q" (same diff, same clutch/flywheel packages, plus a bonded plastic shim on the release bearing). — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **REPORTED (vendor titles)**: Epytec sells front driveshafts for "VR6 axle conversion 4 Motion 02M 02Q 6 speed 4WD" (ISP105) and a rear driveshaft set for "02M 02Q 4motion Haldex conversion" (ISP113). VR6 4Motion 02M/02Q boxes are an established conversion part. — [Epytec ISP105](https://epytec.de/en/drive-shaft-vw-golf-mk2-mk3-corrado-passat-vr6-axle-conversion-4-motion-02m-02q-6-speed-4wd-isp105); [Epytec ISP113](https://epytec.de/en/driveshaft-set-vw-golf-2-3-g60-vr6-conversion-rear-wheel-drive-02m-02q-4motion-haldex-conversion-isp113)
- **VERIFIED (Epytec, background file)**: a 4Motion 02M uses its own diff-side flange arrangement; converting it to FWD takes flange **02M 409 356 A** and seal **02M 409 189**, and VR6 FWD 02M/02Q boxes use bolt-on CV flanges. — [Epytec 698 install guide](https://epytec.de/en/blog/einbauanleitung-fuer-artikel-698-02m-umruesten-fuer-einbau-in-frontangetriebene-fahrzeuge-z.b-vr6-umbau-auf-02m-getriebe)
- **REPORTED (background file)**: the only used-price data point is a FWD 24V 02M bought for $400 with steel forks (Ninety4co, 2023).

**(e) Aisin 09G/09M/09K**
- **VERIFIED (Ross-Tech wiki)**: 09G, 09K and 09M are "built on the same version of the 6-speed automatic transmission manufactured by ... AISIN Co., LTD." When replacing the TCM, use the coding from the original module. — [Ross-Tech 09G/09M/09K](https://wiki.ross-tech.com/wiki/index.php/6-Speed_Automatic_Transmission_(09G/09M/09K))
- **REPORTED (aggregator, background file)**: 09G (FWD) and 09M (AWD) for 2005–2012 3.6 Passats, i.e. B6 Passat 3.6 FWD and 4Motion; VWVortex has a "VR6 4Motion 09M automatic to DSG swap" thread. — [youcanic](https://www.youcanic.com/volkswagen-transmission-model/); [VWVortex 7143344](https://www.vwvortex.com/threads/vr6-4motion-09m-automatic-to-dsg-swap.7143344/)

### Inferences
- **INFERRED, controller generation per box:**
  - 09P (Atlas): native MQB. J217 TCM, the Atlas is listed by HPA as an MQB Haldex 5 car, and it pairs with the Atlas MQB-generation MED17.1.62 ECU.
  - DQ500 (Teramont VR6): very likely MQB, because the Teramont is the Chinese Atlas and shares the 09P/CDVC diagnostics in the same index. Unverified.
  - 02E (R32, A3 8P 3.2, TT 3.2, NMS/B6 Passat, R36/CC EU): PQ-generation J743 that expects PQ35/PQ46 drivetrain-CAN messages, so it is not native to an MQB gateway.
  - 09G/09M: PQ-generation TCM, also not native.
  - 02M/02Q: no TCU; the gearbox's only electrics are reverse-light and (02M) VSS.
- **INFERRED, flanges:** the 6-cylinder 02E has a star flange with tripod inner joint; VR6 02M/02Q (FWD side) and 4-cylinder boxes have bolt-on CV flanges. I found no flange data for the 09P, the DQ500 VR6 or the MQB 0D9/0GC. Expect custom or hybrid axles on any non-A3 box.
- **INFERRED, torque:** the 3.6 (258 lb-ft / 350–361 Nm) sits at the 02M/02Q factory rating, at the DQ250's 350 Nm nominal rating, inside DQ381 (≈420 Nm) and DQ500 (600 Nm), and probably inside the AQ450. Only DQ500 and AQ450 leave forced-induction headroom on paper.
- **INFERRED, NA availability:** in NA, the VR6 boxes you can buy in quantity are the Atlas 09P (2018–2023, FWD and 4Motion), the 02E from the Mk5 R32, A3 8P 3.2 and TT 3.2 (low volume) and NMS Passat 3.6 (FWD only), the 09G/09M from the B6 Passat and probably the CC VR6 4Motion, and the rare 02M 4Motion from the 2004 R32 and 2008–09 TT 3.2. The Teramont VR6 DQ500 would have to be imported from China, as HPA does with the DDKA engine.

### Gaps
- No torque rating for the AQ450/09P was found. The "450" may denote ~450 Nm, but VW naming is not a rating (the DQ250 is a 350 Nm box), so this is unconfirmed.
- No overall dimensions or weights for the 09P, and no confirmation whether the Atlas uses a cable or shift-by-wire selector, or where the J217 sits (in the valve body or separate).
- No gearbox code letters for the Mk5 R32 / A3 8P 3.2 / TT 3.2 02E or 02Q, nor for the Teramont VR6 DQ500.
- Whether the US CC 3.6 4Motion used the 02E (as the brief assumed) or the 09M Tiptronic was not confirmed. My recollection is the 09M, which is unverified.
- No used-price survey for the 09P, 02E VR6 4Motion, 02M R32/TT or DQ500.
- Factory torque ratings for the 02E VR6 4Motion variant were not found (only the generic 350/400 Nm figures).

---

## Key question 2: Do any of the A3 8V's own gearboxes have a VR6 bellhousing, and does a VR6-to-EA888 adapter exist?

### Takeaway
None of them. The A3 8V's boxes are 4-cylinder (EA888/EA211) or 5-cylinder (RS3) bellhousings: 0CW DQ200, 0D9 DQ250, 0GC DQ381, the MQB manuals (0FB/02Q family), and the RS3's DQ500 (most likely 0DL). No commercial VR6-to-EA888 adapter plate was found. The only VR6-on-MQB-gearbox precedent is HPA's in-house "CNC adaptation of DQ381 gearbox" for its VR550T Golf R and Alltrack programs, which are sold as $49k+ labour-inclusive conversions.

### Cited Findings
- **REPORTED (vendor/catalog snippets)**: the original 8V S3 and A3 1.8T quattro used the DQ250 6-speed, and the 8V facelift moved to the DQ381. Codes: **0D9** = 6-speed DSG (DQ250, MQB), **0GC** = DQ381 7-speed, **0DL** = DQ500 in the RS3 8V. **Conflict:** a Polish repair shop lists 0DL under DQ381 together with 0GC and 0DE. — [vagparts.com.au 8V DSG](https://www.vagparts.com.au/collections/audi-8v-a3-s3-rs3-dsg-service-parts); [Ross-Tech 0D9 (title)](https://wiki.ross-tech.com/wiki/index.php/6-Speed_Direct_Shift_Gearbox_(DSG/0D9)); [NGP DQ500 kit 8V/8Y RS3, 8S TT RS](https://store.ngpracing.com/products/dq500-7-speed-dsg-transmission-complete-service-kit-audi-8v-8y-rs3-8s-ttrs); [naprawczesc](https://en.naprawczesc.pl/artykul-Repair_of_DSG_gearbox_controller_DQ380_DQ381_and_DQ500_(P1735_10666_and_P1736_10668)); [SSP 556 "7 Speed Dual Clutch Gearbox 0GC"](https://www.t6forum.com/threads/ssp-556-the-7-speed-dual-clutch-gearbox-0gc.25584/latest)
- **REPORTED (NHTSA-hosted Audi bulletin, title/snippet)**: a 2019–2020 TTS/TT RS bulletin covers cars with either 0DL or 0GC gearboxes. — [NHTSA MC-10171334](https://static.nhtsa.gov/odi/tsbs/2020/MC-10171334-0001.pdf)
- **VERIFIED (factory manual index)**: "Transmission 0GC 7 speed (DQ381-7A)" is listed with 4-cylinder engines DKFA, DTFA and DCGA. — [vwts.ru](https://vwts.ru/vw_teramont_0a.html)
- **REPORTED (Wikipedia; Chinese press)**: DQ381 is rated at 420–430 Nm (Wikipedia table); one Chinese source says 380 Nm. DQ200 (0AM/0CW) is "paired to engines with up to 250 N⋅m". — [Wikipedia DSG](https://en.wikipedia.org/wiki/Direct-shift_gearbox); [Autohome](https://www.autohome.com.cn/info/201803/913726.html)
- **VERIFIED (FCP Euro)**: the MQB 0FB has "refined ... bellhousing spacing and design" relative to the 02Q, which is itself a 4-cylinder housing (8-bolt TSI flywheel; VR6 has a 10-bolt crank). — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **VERIFIED (catalog page, oemwolf)**: 02S 300 048 "6-Speed Manual Transmission" is listed for "Audi A3, S3, Sportback, quattro" ranges 2013–2015 (incl. USA 2015) at $4,409.96, and 02S 300 047 is listed for 2007–2013 VAG cars (superseded by 02S 300 047 F). — [oemwolf 02S300048](https://oemwolf.com/oem-parts/02s300048.html); [oemwolf 02S300047](https://oemwolf.com/oem-parts/02s300047.html)
- **VERIFIED (vendor page, HPA)**: VR550T Golf R spec list: "**CNC adaptation of DQ381 Gearbox**", "Upgraded DQ381 DSG with upgraded Clutch Packs", "Full UDS canbus integration", "Available in DSG & 6-Speed Manual". Base car is a 2018–2019 Golf R with DQ381. Packages "begin at $49,000 USD" covering labour. — [HPA VR550T Golf R](https://www.hpamotorsports.com/pages/hpa-vr550t-2-5l-vr6-program-for-golf-r)
- **VERIFIED (vendor page, HPA)**: VR550T Sportwagen/Alltrack: "DQ381 7-Spd DSG transmission conversion with upgraded Clutch Packs and **DQ381 compatible drive shaft**". The base car must be a 2016–2019 Sportwagen/Alltrack with the DQ250. "Starting at $64,300 USD, labour inclusive". — [HPA VR550T Alltrack](https://www.hpamotorsports.com/pages/hpa-vr550t-2-5l-vr6-program-for-sportwagen-alltrack)
- **REPORTED (The Drive, via search summary)**: on the Alltrack, HPA judged the DQ250 unable to take more than 500 lb-ft and fitted the Mk7.5 Golf R's DQ381. This "required hunting for a trouble code thrown when the transmission tried to connect to an electronic parking brake that wasn't there". — [The Drive Alltrack](https://www.thedrive.com/news/swapping-a-537-hp-vr6-turbo-into-a-vw-golf-alltrack-is-the-right-choice)
- **Searched, nothing found**: no listing for a VR6-to-EA888 (or VR6-to-02Q/0FB/DQ381) bellhousing adapter plate turned up. A 2020 Classic Motorsports forum post claims "VR5/6 have the same bolt pattern as the 1.8/2.0/2.5 and 4cyl TDI". That is **REPORTED**, unverified, and contradicted by FCP Euro's 10-bolt vs 6/8-bolt crank facts and by the swap community's VR6-specific-bellhousing consensus (background file). — [Classic Motorsports VR6 RWD thread](https://classicmotorsports.com/forum/grm/vr6-rwd/53192/page1/)

### Inferences
- **INFERRED**: "CNC adaptation" plus the absence of any VR6-pattern DQ381 in VW's catalogue implies HPA machines the DQ381 bellhousing, or a plate/housing, to accept the VR6 block and flywheel/drive plate. It is a one-shop solution, not a buyable part.
- **INFERRED**: HPA needing a "DQ381 compatible drive shaft" when going from DQ250 to DQ381 in an MQB Alltrack shows that **the PTU-to-prop-shaft interface differs between MQB 4Motion gearboxes**. Do not assume an Atlas, R32 or A3 PTU will mate to the A3 prop shaft without a custom or hybrid shaft.
- **INFERRED**: the 02S 300 048 catalog line is very likely a front-drive MQ250-family 6-speed (02S is not the 02Q/0FB code), and oemwolf's "quattro" text is the model-range name, not proof of AWD. Do not treat it as an A3 quattro manual.
- **INFERRED**: the A3 8V's own DSGs (0D9/0GC) are the ideal mechanical/electrical fit for the chassis (axles, mounts, PTU, prop shaft, shifter, CAN), but using one with a VR6 means replicating HPA's machining.

### Gaps
- What HPA's "CNC adaptation" physically is (machined bellhousing, adapter plate, custom input shaft or drive plate) and whether HPA sells it outside the VR550T program.
- The manual gearbox HPA uses for "6-Speed Manual" VR550T cars (02Q/0FB adapted, or a VR6 02M/02Q).
- Code letters for the US A3 8V 0D9/0GC/0CW boxes, and confirmation of 0DL vs 0GC for the RS3.

---

## Key question 3: How is MQB Haldex 5 controlled, will it run with a non-MQB gearbox or ECU, and do PTUs and prop shafts interchange?

### Takeaway
On the A3 8V, Golf R and Atlas the Haldex 5 coupling sits at the rear diff with its controller **J492** on the unit, part numbers **0CQ 907 554 D/H/J** (HPA). It runs from CAN data: wheel speeds, ESP and steering data, engine torque, pedal and rpm. It works with a manual gearbox from the factory (Mk7 Golf R manual, Euro S3 manual), so a DSG TCU is not required. No source shows the OEM J492 running happily without MQB engine and ABS messages. The documented workaround is a standalone controller: Syvecs, "works with any engine management system", about NZ$3,890. No source gives PTU or prop-shaft flange data allowing interchange between PQ35 R32/A3 3.2, Atlas and A3 8V parts. Plan on a custom or hybrid prop shaft.

### Cited Findings
- **VERIFIED (vendor page, HPA)**: compatible OEM Haldex controllers are **0CQ 907 554 D (SW 7076, 7082)**, **0CQ 907 554 H (SW 7083)** and **0CQ 907 554 J (SW 7084)**. The HPA controller fits "all VAG MQB vehicles with Haldex AWD except Audi RS3, TT, TTRS, TTS". Fitment includes **Audi A3 Quattro (8V) 2015–2020** and **S3 (8V) 2015–2020** (both marked "Default Coding"), Golf VII R 2015–2019, Tiguan 2016–2022, **Atlas 2018–2022**, Passat B8, Arteon and others. Non-default cars must be "individually coded for your car's make, year, and model". **$1,099.00**. — [HPA Gen 5 controller](https://www.hpamotorsports.com/products/gen-5-performance-haldex-controller)
- **REPORTED (vendor listing)**: Neuspeed's "Haldex Performance Controller Gen 5 MQB" appears to be the same unit (part no. HALDEX.2022060). — [Black Forest Industries](https://blackforestindustries.com/products/haldex-performance-controller-gen-5-mqb)
- **VERIFIED (vendor page, Syvecs)**, SYV-4WD-HALP-VAG:
  - It is "a standalone AWD/4WD/Centre Diff controller designed to control the haldex system". It "replicates all the OEM CAN information" (steering angle, brake pressure, RPM, throttle position, lateral and longitudinal G, yaw, speeds, temperatures, mode switches).
  - It "Works with any Engine management system".
  - It has 4 magnetoresistive ABS sensor inputs, 2 configurable CAN buses, outputs up to 30 A, and is tuned in Scal (40+ maps).
  - Listed fitment: S3, Leon Cupra, Golf R 7/7.5 "and more". The RS3/TT RS need the Iroz Motorsport controller.
  - "Designed for Off-Road use only".
  — [Syvecs](https://www.syvecs.com/?p=6664)
- **REPORTED (retailer, search summary)**: Syvecs MQB Gen 5 controller about **NZ$3,890**, ~2-week lead time. — [Harry's Euro NZ](https://www.harryseuro.co.nz/products/syvecs-haldex-controller-vag-mqb-gen5)
- **REPORTED (trade article)**: Gen 5 is "smaller, lighter and less complex". It drops the Gen 4 pressure accumulator and control valve. The controller uses ABS wheel speeds, longitudinal/lateral dynamics, accelerator position and engine torque received over CAN, and works proactively. — [TPS trade article](https://tps.trade/blog/all-systems-go-as-haldex-put-under-the-spotlight)
- **REPORTED (repair vendor)**: if J492 stops communicating, the AWD system goes to failsafe and disengages the clutch pack. DTC 01324 = "control module for all-wheel-drive (J492): no signal/communication". — [ECU Testing](https://ecutesting.com/common-faults/volkswagen/haldex-gen-5-ecu-failure)
- **REPORTED (VW newsroom via search summary)**: on the Golf R, the 4Motion coupling engages before slip; a control unit sets clutch pressure "to match the torque the rear axle should receive"; activation "depends mainly on the engine torque the driver requests"; the rear axle is decoupled at light load. The manual Golf R had "a reinforced clutch and short-travel shifting". — [VW newsroom Golf R 4Motion](https://www.volkswagen-newsroom.com/en/the-new-golf-r-2432/4motion-all-wheel-drive-in-the-golf-r-2451)
- **REPORTED (vendor title)**: "Haldex Gen5 service kit, VW Mk7/Mk7.5 Golf R, Sportwagen, Alltrack, Tiguan, **Atlas**, Audi **8V A3 S3 RS3**, 8S TT TTS TTRS", i.e. the Atlas and A3 share the Gen 5 pump/filter service parts. Also "Tunezilla Gen 5 Haldex tune VW Mk7/Mk7.5, Audi 8V" (controller flash). — [NGP Gen5 service kit](https://store.ngpracing.com/products/haldex-gen5-service-kit-vw-mk7-mk7-5-golf-r-sportwagen-alltrack-tiguan-atlas-audi-8v-a3-s3-rs3-8s-tt-tts-ttrs); [NGP Tunezilla](https://store.ngpracing.com/products/tunezilla-gen-5-haldex-tune-vw-mk7-mk7-5-audi-8v)
- **REPORTED (marketplace and febi snippets)**: A3/S3 quattro 2013–2020 rear differential assembly **0CQ 525 010 S** (listed as limited-slip); febi's Haldex pump-seal kit cross-references 0CQ 525 010 S. — [eBay.de 317176026245](https://www.ebay.de/itm/317176026245); [febi partsfinder](https://partsfinder.bilsteingroup.com/de/article/febi/1000000)
- **REPORTED (press)**: on the Mk7.5 the Haldex coupling sits "in front of the rear axle differential (at the end of the prop shaft)". — [australiancar.reviews Mk7.5 R](https://australiancar.reviews/review-volkswagen-mk7-5-golf-r-2017-20/)
- **REPORTED (background, VWVortex snippet)**: a 4Motion donor adds ABS and yaw/pitch sensor work to a MED17 3.6 swap. — `precedents_vendors_salvage.md` (VWVortex 6957680/7166366)

### Inferences
- **INFERRED**: the A3 8V's J492 already knows how to run without a DSG, because the same 0CQ 907 554 controller family runs manual Golf Rs and Euro manual S3s. What it needs is valid MQB engine-torque/pedal/rpm messages from an ECU, ABS/ESP messages, and correct coding.
  - If the VR6 runs an **Atlas MQB-generation ECU (MED17.1.62, 03H 906 026 x)**, those engine messages are the right protocol generation. The remaining question is whether the A3 gateway will accept it. That gateway acceptance is unverified.
  - If the swap uses the **NMS Passat PQ-generation ECU** (CDVB, MED17.1.6), the J492 will almost certainly see "no engine torque" or implausible data, set faults and default towards FWD. That case needs a CAN translator or the Syvecs standalone controller.
- **INFERRED**: because the HPA/Neuspeed controller replaces the OEM J492 and depends on OEM CAN, it does not solve a non-MQB ECU problem. The Syvecs unit is the only documented controller that claims engine-management independence, and it reads wheel speeds directly.
- **INFERRED, prop shaft/PTU:** the A3 8V prop shaft, rear diff and Haldex 5 are one MQB system; the Atlas uses the same Gen 5 family on a longer wheelbase. PQ35 VR6 4Motion cars (Mk5 R32, A3 8P 3.2, TT 3.2) use Gen 2 (or Gen 4) Haldex and a PQ35 prop shaft. Even within MQB, HPA needed a different prop shaft for DQ250 → DQ381. So the realistic plan for any non-A3 gearbox is the gearbox's own PTU plus a **custom two-piece prop shaft** with a front flange matched to that PTU and a rear flange matched to the A3's 0CQ Haldex/rear diff. The A3's rear subframe, diff, J492 and fuel tank stay.

### Gaps
- Prop-shaft part numbers for the A3 8V quattro, Atlas 4Motion, Mk5 R32/A3 8P 3.2 (02E) and 02M R32/TT 3.2, and their PTU output-flange types (bolt circle, number of bolts, CV vs Hardy disc). Not found in any opened source.
- PTU/angle-drive part numbers for the A3 8V 0D9/0GC quattro, Atlas 09P 4Motion and 02E/02M 4Motion. Not found. Read them off the donor or ETKA by VIN.
- No official Gen 5 SSP or signal list for J492 was retrieved (only a French SSP 206 on earlier Haldex and a Gen IV PDF: [Gen IV PDF](https://automotivetechinfo.com/wp-content/uploads/2019/08/VW-Haldex-4Motion-Generation-IV.pdf)).
- No source documents a Haldex 5 car running a non-MQB ECU with the OEM J492.

---

## Key question 4: Is a VR6-pattern 02M/02Q 4Motion manual feasible in an A3 8V quattro?

### Takeaway
It is feasible in principle and has partial precedents, but it is a fabrication project. In its favour: MQB built manual + Haldex 5 cars from the factory (US Mk7 Golf R 6-speed, Euro S3 8V manual quattro), so the A3's Haldex 5 does not need a DSG TCU. A manual has no TCU to integrate. A 2-pedal A3 quattro has been converted to 3 pedals by a VW/Audi technician. HPA sells a VR6 Golf R "in DSG & 6-Speed Manual". Against it: the VR6 4Motion manuals (2004 R32 02M, 2008–09 TT 3.2 02M; EU Mk5 R32 02Q) are 20 years old and PQ-generation. Their angle drive, axle flanges and mounts will not match MQB parts, so the prop shaft, axles and probably the shift-cable ends need custom work. A US A3 8V has no clutch-pedal hardware, so the pedal box, master cylinder, line and shifter must come from a manual MQB donor (Golf R/GTI or Euro A3/S3). No source gave those part numbers.

### Cited Findings
- **REPORTED (FCP Euro Golf R buyer's guide, search summary)**: the Mk7 Golf R manual is an MQ350 (02Q-family) H-pattern with 1st 3.36, 6th 0.91, and final drives **4.24 (1st–4th) / 3.27 (5th–6th)**. **VERIFIED (FCP Euro MQ350 guide)**: the US 2015+ Golf R box is the **0FB**. — [FCP Euro Golf R guide](https://blog.fcpeuro.com/the-definitive-volkswagen-mk7-golf-r-buyers-guide); [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)
- **REPORTED (VW newsroom; evo)**: Mk7 Golf R offered "both manual and DSG" with Haldex 5 4Motion. The manual was dropped around the WLTP changeover (2018/19). — [VW newsroom](https://www.volkswagen-newsroom.com/en/the-new-golf-r-2432/4motion-all-wheel-drive-in-the-golf-r-2451); [evo Golf R Mk7](https://www.evo.co.uk/volkswagen/golf-r/15277/volkswagen-golf-r-mk7-2014-2020-review-one-of-the-best-modern-hot-hatches)
- **REPORTED (Wikipedia, search summary)**: on the 8V S3, "A six-speed manual transmission and quattro all-wheel drive come as standard. The 6-speed S tronic dual clutch transmission is available for an additional charge" (European market). — [Wikipedia Audi S3](https://en.wikipedia.org/wiki/Audi_S3)
- **REPORTED (Audiworld feature, snippet only; page blocked)**: "If you can't buy it – Build it! Turning a 2 pedal A3 quattro into a 3 pedal A3 quattro". The builder, Carson, is "a VW and Audi trained technician"; the car "came from the factory with a DSG". The swap "may not be for the faint of heart" but was done cleanly. The snippets do not confirm the generation (8V vs 8P), gearbox or parts. — [Audiworld](https://audiworld.com/?p=47081)
- **VERIFIED (vendor page, HPA)**: the VR550T (VR6) MQB Golf R is "Available in DSG & 6-Speed Manual". No gearbox detail is given. — [HPA VR550T Golf R](https://www.hpamotorsports.com/pages/hpa-vr550t-2-5l-vr6-program-for-golf-r)
- **REPORTED (Speedhunters, via search summary)**: a Mk5 Golf with a naturally aspirated VR6 and DSG was converted to Haldex AWD (PQ35, not MQB). — [Speedhunters](https://www.speedhunters.com/?p=335347)
- **REPORTED (Audizine/forum summaries, generic)**: in Audi auto-to-manual swaps "coding is the real obstacle". ECU and ABS must accept manual coding, and on quattro cars the manual prop shaft and front driveshafts can differ in length from the automatic's. — [Audizine transmission swap](https://audizine.com/threads/transmission-swap.634779/); [Audizine TipTronic to manual](https://www.audizine.com/forum/showthread.php/460049-TipTronic-to-Manual-Transmission-Swap/page4)
- **REPORTED (background file, Ninety4co, running car)**: a PQ35 Mk6 GTI's stock 02Q shift box and cables mated to a Mk4 02M unmodified; HPA and CTS sell one short-shifter for "02M/02Q". The clutch-switch circuit needed a fuse added because the donor engine's car never had a manual. — `manual_02m_transmission.md` (Key questions 4 and 6)
- **VERIFIED (FCP Euro)**: same release bearing on 02M and 02Q. The 0FB uses "generally the same clutch and flywheel packages" as the 02Q, plus a bonded shim. — [FCP Euro MQ350 guide](https://www.fcpeuro.com/blog/definitive-guide-vw-audi-6-speed-manual-transmissions-mq350-02m-02q-0fb)

### Inferences
- **INFERRED, Haldex without a DSG:** not a problem in principle; the J492 runs manual Golf Rs and S3s. Code the A3's J492/ABS/ECU installation list as manual, or borrow a manual Golf R/S3 J492 software version (the HPA list shows several software versions under one part number). If the engine ECU is not MQB-generation, see Key question 3: use the Syvecs controller.
- **INFERRED, shift mechanism:** the MQB manual shift box and cables (Golf R/GTI/Euro A3) are the descendants of the PQ35 02Q cable system. The 0FB is a refined 02Q, and Ninety4co proved PQ35 02Q cables work on an 02M tower, so MQB cables will probably mate to an 02M/02Q tower. Lengths and the routing around a VR6 are unknown; verify on the bench.
- **INFERRED, pedal box and hydraulics:** a US A3 8V was never sold with a manual. Source the complete pedal cluster (with clutch pedal and switch), clutch master, line and slave mount from a manual MQB Golf/GTI/Golf R or a Euro A3, plus the console shifter, boot and cables. The ECU, ABS, gateway and cluster all need manual coding. The CDVC/CDVB ECU was never calibrated for a manual, so a swap tune is required (background file).
- **INFERRED, angle drive:** the 2004 R32 or TT 3.2 02M angle drive is a PQ-era unit. Its output flange will not match the A3 prop shaft, and its height/offset relative to the A3 tunnel is unknown. A custom front prop-shaft section is mandatory.
- **INFERRED, axles:** VR6 02M 4Motion boxes use bolt-on flanges (100 mm class); the A3 8V quattro axles are MQB DQ250/DQ381 items. Expect custom or hybrid axles (Epytec-type or a driveshaft shop).
- **INFERRED, torque:** a manual Golf R puts its EA888 torque through the MQ350/0FB from the factory, so a stock 3.6 is within what this gearbox family survives in practice. The 258 lb-ft factory rating applies on paper.

### Gaps
- Part numbers for the MQB manual pedal box, clutch master, clutch line, shift box (5Q0 711 xxx) and cables. Not found in any opened source.
- Code letters and availability of the Euro Mk5 R32 02Q 4Motion and any Euro A3 8P 3.2 manual.
- Whether HPA's manual VR550T uses an adapted 0FB or a VR6 02M/02Q.
- A documented A3 8V (not 8P) manual conversion with a parts list. The Audiworld feature could not be read.

---

## Key question 5: Could an A3 8V use the Atlas Aisin 8-speed?

### Takeaway
Electrically, the Atlas 4Motion VR6 + 09P (QVK/TYF) is the most natural fit of any VR6 drivetrain. It is the only factory combination of VR6 + MQB-generation ECU and TCU + Haldex 5 (same 0CQ 907 554 controller family, same Gen 5 service kit as the A3). Mechanically it is unproven: no source gives its dimensions, selector type, J217 location or PTU/prop-shaft interface, and no one has documented a 09P in a Golf or A3. The same 09P family does sit behind EA888 in MQB Tiguans, Arteons and Q3s, so it exists in compact MQB bays, but with a 4-cylinder.

### Cited Findings
- **VERIFIED**: 09P AWD 3.6 codes are QVK and TYF, and FWD 3.6 codes are QVJ and TYT; the CDVC is diagnosed with "09P (AQ450-8F)". — [vwts.ru](https://vwts.ru/vw_teramont_0a.html)
- **VERIFIED**: the same 09P service kit covers 2018+ Tiguan 2.0T, Atlas 2.0T/3.6L, Arteon and Q3 F3. The 09P is an MQB-family gearbox used with EA888 as well as VR6. — [NGP 09P kit](https://store.ngpracing.com/collections/dsg-system/products/vw-audi-09p-aq450-8-speed-automatic-transmission-service-kit)
- **VERIFIED**: Atlas 2018–2022 is in the MQB Gen 5 Haldex controller fitment list alongside the A3 8V. — [HPA Gen 5 controller](https://www.hpamotorsports.com/products/gen-5-performance-haldex-controller)
- **REPORTED**: Atlas TCM is J217 (2025 bulletin); AQ450 software includes "driveshaft protection" logic (2017 bulletin); AQ450 TCU flashable via OBD (Autotuner). — [NHTSA MC-11021375](https://static.nhtsa.gov/odi/tsbs/2025/MC-11021375-0001.pdf); [NHTSA MC-10128427](https://static.nhtsa.gov/odi/tsbs/2017/MC-10128427-9999.pdf); [Autotuner](https://us.autotuner.com/blogs/news/vag-8-speed-aisin-aq450-now-live-via-obd-on-the-tool)
- **VERIFIED (background file)**: Atlas CDVC ECU = Bosch MED17.1.62, hardware 03H 906 026 E. — `precedents_vendors_salvage.md` (c4ip.ru)
- **Searched, nothing found**: no build of an Atlas 09P in a Golf, GTI, Golf R or A3, and no Atlas selector or TCM-location document.

### Inferences
- **INFERRED, why it is attractive:** the engine ECU, TCU and Haldex controller all speak MQB CAN. The A3's J492 gets engine torque and gear data in the format it expects, the TCU and ECU are a factory-matched pair, and there is no PQ-to-MQB translation layer. This assumes the Atlas engine/ECU is used, not the NMS Passat one. The integration work moves to the gateway installation list, component protection (if any applies to these modules), cluster coding and the selector.
- **INFERRED, why it is risky:** an 8-speed planetary automatic is usually longer across the car than a DSG. The A3 8V is MQB A1 (narrower engine bay than the Atlas's long MQB). The VR6 plus 09P length against the A3's frame rails, battery tray and left-hand mount is the deciding measurement, and no source gives it. HPA built its MQB A1 VR6 Golf R around an adapted DQ381 rather than the readily available Atlas 09P. That suggests the 09P either does not package in a Golf/A3 or offered no advantage to HPA. It is a hint, not proof.
- **INFERRED, selector:** if the Atlas uses a cable selector, an A3 8V would need the Atlas lever and cable in the tunnel, because the A3's DSG selector and its gearbox-end interface are DSG-specific. Whether the Atlas or the A3 8V DSG uses a cable or shift-by-wire was not sourced, and no such conversion is documented.
- **INFERRED, a parallel option:** the Teramont 2.5T VR6 DQ500 4Motion is the other VR6 + MQB-CAN + Haldex 5 drivetrain. The RS3 8V proves a DQ500 + quattro physically fits an A3 8V body. It is China-only, so sourcing, the gearbox code and the PTU interface are unknown.

### Gaps
- 09P case length, weight, bellhousing-to-end-cover dimension, and the Atlas PTU/prop-shaft flange.
- Atlas selector type (cable vs by-wire) and J217 location.
- Atlas 09P used price (eBay listing seen without price).
- Any precedent of an Atlas drivetrain in an MQB A1 car.

---

## Key question 6: Which gearbox and AWD combination is most realistic for the A3 8V swap, with costs and rebuild items?

### Takeaway
No combination has a documented A3 8V precedent, so this ranking is a judgement (INFERRED) built on the findings above.
1. **For AWD with an automatic: the Atlas 4Motion VR6 drivetrain**, i.e. Atlas CDVC with its MQB ECU, the **09P QVK/TYF** with its PTU, and the A3's own Gen 5 Haldex/rear diff (0CQ family) behind a custom prop shaft. It is the only all-MQB-CAN VR6 AWD drivetrain, it is plentiful and cheap in North America, and the Haldex 5 side needs no translation. It must first pass a physical trial fit in an A3 bay.
2. **For a manual with AWD: a VR6 02M 4Motion** (2004 R32 or 2008–09 TT 3.2 quattro). It needs MQB manual pedal box, shifter and cables from a Golf R/GTI or Euro A3 donor, plus a custom prop shaft and axles, J492 coded as manual (or a Syvecs standalone controller if the ECU is not MQB-generation), and a manual swap tune. It is the most mechanically transparent route but the most fabrication-heavy, and it runs at the 02M's torque rating.
3. **The professional route: HPA-style CNC-adapted DQ381 (0GC)**. It is proven on MQB Golf R and Alltrack, keeps the MQB PTU, axles and selector, and runs about $49k–$64k labour-inclusive at HPA. It is not a DIY part.
4. **Least attractive: a PQ35 02E 4Motion DSG** (R32, A3 8P 3.2, TT 3.2). The bellhousing and size are right, but it brings a PQ-generation J743 plus Gen 2/Gen 4 Haldex expectations into an MQB car. That means two CAN generations, star-flange/tripod axles and a custom prop shaft; the PTU-flange part is shared with options 1 and 2.

### Cited Findings (cost and rebuild data points)
- **VERIFIED**: HPA Gen 5 Haldex controller $1,099.00. Syvecs MQB Gen 5 standalone about NZ$3,890 (REPORTED retailer). — [HPA](https://www.hpamotorsports.com/products/gen-5-performance-haldex-controller); [Harry's Euro](https://www.harryseuro.co.nz/products/syvecs-haldex-controller-vag-mqb-gen5)
- **VERIFIED**: 09P service kit $279.99 (7 L Top Tec ATF 1800, filter, gasket, plug). — [NGP](https://store.ngpracing.com/collections/dsg-system/products/vw-audi-09p-aq450-8-speed-automatic-transmission-service-kit)
- **VERIFIED**: HPA VR550T Golf R from $49,000 labour; Alltrack from $64,300 labour-inclusive (includes the DQ381 conversion and a DQ381-compatible drive shaft). — [HPA Golf R](https://www.hpamotorsports.com/pages/hpa-vr550t-2-5l-vr6-program-for-golf-r); [HPA Alltrack](https://www.hpamotorsports.com/pages/hpa-vr550t-2-5l-vr6-program-for-sportwagen-alltrack)
- **REPORTED (vendor title)**: a Haldex Gen 5 service kit is sold for the Atlas and A3 8V (pump and filter service item). — [NGP Gen5 kit](https://store.ngpracing.com/products/haldex-gen5-service-kit-vw-mk7-mk7-5-golf-r-sportwagen-alltrack-tiguan-atlas-audi-8v-a3-s3-rs3-8s-tt-tts-ttrs)
- **REPORTED/VERIFIED (background file)**, items for the 02M route:
  - used FWD 02M $400 (no 4Motion price found);
  - South Bend Mk4/TT 6-speed flywheel kit $683.62 (VR6 10-bolt variant required);
  - Clutch Masters hydraulic release bearing $399;
  - slave cylinder 02M 141 671 family (plastic slave block a known failure);
  - steel shift forks (Bar-Tek), 4th-gear support, input-shaft bearing play and 2nd/3rd synchros as known weaknesses.
  Note: the Peloquin 02M LSD "Does not fit AWD models", and the Wavetrac 10.309.190WK is FWD only. — `manual_02m_transmission.md`; [NGP Peloquin 02M](https://store.ngpracing.com/products/peloquins-limited-slip-diff-vw-mk4-6-speed-02m)
- **VERIFIED (Epytec, background)**: Epytec's 4Motion-to-FWD kit 698 exists. It is relevant only if a 4Motion 02M were run FWD, which is not the case here. — [Epytec 698](https://epytec.de/en/6-speed-manual-gearbox-conversion-kit-02m-4motion-vr6-r32-golf-mk1-2-3-4-turbo-698)

### Inferences
- **INFERRED, why the Atlas drivetrain ranks first:** the A3 8V quattro's hardest problem is not the bellhousing (every VR6 box has one) but making the Haldex 5, gateway, ABS and cluster accept the swapped powertrain. Only the Atlas set (CDVC + MED17.1.62 + 09P/J217) was engineered on the same MQB electrical architecture as the A3's J492 (same 0CQ 907 554 controller family, same Gen 5 service parts). A FWD Atlas 09P (QVJ/TYT) is a fallback if the 4Motion PTU will not package. The A3 would then need a custom PTU solution or would have to go FWD, which defeats the purpose.
- **INFERRED, Atlas build list, minimum:**
  - donor Atlas 3.6 4Motion (2018–2019 preferred: 11.4:1 CDVC, closest to the Passat engine per the background file), with engine, ECU, 09P + PTU, J217/harness and selector;
  - A3 8V quattro rear driveline retained (0CQ 525 010-type rear diff/Haldex with J492 0CQ 907 554 D/H/J);
  - custom 2-piece prop shaft (Atlas PTU flange to A3 Haldex flange);
  - custom axles (09P flange to A3 hubs);
  - custom left mount and dogbone;
  - gateway, ABS and cluster coding plus J492 re-coding (possibly HPA's controller, which is individually coded per car);
  - rebuild/service items: 09P fluid and filter (7 L Top Tec 1800), PTU and Haldex service, Gen 5 Haldex pump/filter, mounts.
- **INFERRED, 02M build list, minimum:**
  - 02M 4Motion with angle drive (2004 R32 / 2008–09 TT 3.2; inspect forks, input bearing, angle-drive seals);
  - VR6 10-bolt clutch/flywheel (South Bend K70287 VR6 variant) and 02M slave;
  - MQB manual pedal cluster, master, line, shift box and cables from a manual Golf/GTI/Golf R;
  - custom prop shaft and axles;
  - J492/ABS/ECU manual coding or the Syvecs controller;
  - a swap tune with manual strategy.
- **INFERRED, budget:** no complete-route cost is sourced. The sourced pieces (controller $1,099–NZ$3,890, clutch about $684, service kits about $280, HPA labour $49k+) show the DIY routes are dominated by custom prop shaft/axle fabrication and coding labour, neither of which was priced in any source.

### Gaps
- No one has published an A3 8V (or Golf R Mk7) built with any VR6 gearbox other than HPA's adapted DQ381. All four routes rest on inference for the A3 specifically.
- Custom prop shaft and axle fabrication costs, 09P/02M 4Motion/02E 4Motion used prices, and the dimensional data that would settle whether the Atlas 09P fits an MQB A1 bay.
- Whether the A3 8V gateway accepts an Atlas ECU/TCU in its installation list, and whether component protection applies. This belongs to the electrical-integration research.

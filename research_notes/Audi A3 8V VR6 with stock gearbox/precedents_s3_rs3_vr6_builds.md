# VR6 swaps into Audi A3/S3/RS3 8V (MQB A1), and MQB Golf/TT VR6 builds that kept an MQB gearbox

Research date: 2026-10-08. This follows `../Audi A3 8V VR6 swap parts/precedents_recipient_market.md` (whose section 1 said "no documented VR6 swap into any A3/S3/RS3 8V"). That conclusion was wrong. The builds were on YouTube, Facebook, Instagram, Audizine and drive2, which the earlier search could not see. The TuneZilla S3 is documented in detail in the companion note `tunezilla_vr6t_s3_build.md` in this folder, which is built from the video transcripts. Its facts are only summarised here.

**Labels.** **VERIFIED** means a build page, vendor page or article I opened and read. **REPORTED** means a search-engine snippet, a social-post caption, or a forum post I could not open. **INFERRED** means my own reasoning.

**Access.** Audizine (Cloudflare block), VWVortex, drive2.ru (HTTP 403 to both WebFetch and curl), TikTok (empty shell) and the Wayback availability API (HTTP 429) could not be read. Every quote from those sites below is a search snippet. YouTube was not fetched, as instructed; video titles and URLs are listed so the builder can watch them.

## 1. Which VR6-swapped A3/S3/RS3 8V cars exist, and how was each one done?

### Takeaway
At least four 8V-body VR6 cars exist:
- **One S3:** TuneZilla's 2017 S3, Canada. It runs.
- **One true RS3:** Malaka Motorsports' 2018 US RS3, California. It runs, at 1,138 hp.
- **One A3 rebodied as an "RS3 LMS TCR":** Steve Gregorius / L8-Night, Germany. It runs, 199.87 mph over the half mile. Its 8V base is likely but not confirmed.
- **One A3 8V:** a Russian drive2 car with a Teramont 2.5T DDKA and DQ500. It has reportedly made its first start.

A second US S3 project (a 2016 S3 with a 3.6 and a DQ500) is at the planning stage on Audizine. Every running build uses a DQ500, not the S3/A3's own DQ250. Every one is a turbo race or drag car.

### Summary table

| # | Car | Owner/shop, country | VR6 | Gearbox and how it was mated | AWD | ECU | Status | Main source |
|---|---|---|---|---|---|---|---|---|
| A | 2017 S3 8V quattro | TuneZilla, Western Canada | New 3.6 **BWS** (R36) long block, Garrett G42-1200 | Used **RS3/TT RS DQ500**, bellhousing machined for the VR6, VR6 flywheel clearanced; Atlas VR6 engine mount + RS3 trans mount and dogbone | Yes (DQ500 PTU + Haldex) | **Factory Atlas 3.6 MED17** with TuneZilla patches | Running drag car (2025–26) | REPORTED (own videos): see `tunezilla_vr6t_s3_build.md` |
| B | 2018 RS3 8V | George & Stav, Malaka Motorsports, Palmdale/Lancaster CA, USA | **3.0 "R30"** stroker, turbo G42-1450 | **DQ500** (stock RS3's, INFERRED), DCT billet flywheel + HD1400 clutch; bellhousing method not published | Not stated | **Syvecs S7 Plus** + **Unitronic TCU** | Ran 1,138 hp at the hubs (article Dec 2022) | VERIFIED article [ESD](https://engineswapdepot.com/?p=89770) |
| C | "Audi A3" in carbon RS3 LMS TCR widebody | Steve Gregorius / L8-Night Project Cars, Germany | Turbo VR6, **3.0** (ESD) or **3.2** (TikTok) | **DQ500 DSG** (ESD 2021); Quaife sequential "being built" (2020) / "sequential box" (2024) | "4-Motion" | Not stated | 199.87 mph over the half mile (2021) | VERIFIED article [ESD](https://engineswapdepot.com/?p=77207) |
| D | 2014 A3 8V | drive2 user / channel "FAM-BiTurbo", Russia | **Teramont 2.5T VR6** (DDK/DDKA family), 300 hp tag | **DQ500 ("DQ501")** | Logbook tag says FWD | **MED17.1.62** (Teramont); immobiliser adapted to engine + DSG | First start reported (~late 2025) | REPORTED [drive2](https://www.drive2.ru/l/720735095761145905/) |
| E | 2016 S3 8V | Audizine member, USA | 3.6 from a 2009 Passat wagon (BLV, INFERRED), planned turbo | DQ500 came with the engine | ? | Asked about HPA reflash | Planning (~2 yrs old) | REPORTED [Audizine](https://www.audizine.com/forum/showthread.php/992856-2016-Audi-S3-getting-a-VR6-Engine-Emission-Questions) |

### Cited Findings

**A. TuneZilla 2017 S3 8V (Canada). This is the S3 the builder saw.**
- TuneZilla's TikTok caption describes "a 2017 Audi S3, swapped with a 3.6L VR6 and Turbocharged with a Garrett G42 1200 paired to a DQ500 transmission from an Audi RS3"; the car "started as a street car" and was converted into "a full dedicated drag car". — **REPORTED** (TikTok caption via search snippet) [TikTok discover "vr6 swap"](https://www.tiktok.com/discover/vr6-swap)
- Video to watch: "Drag Racing in the 10 second (?) Tunezilla S3!!! - Built Audi S3" — **REPORTED** (title) [YouTube Hl0jj4DKT8A](https://www.youtube.com/watch?v=Hl0jj4DKT8A). The full video list and the build facts are in the companion note:
  - BWS long block.
  - RS3 DQ500 with the bellhousing "machined to mate up to the VR6", and a VR6 flywheel.
  - Atlas VR6 engine mount, RS3 transmission mount and dogbone, RS3 radiator support.
  - AWD kept.
  - Factory Atlas MED17 ECU with TuneZilla software. "A few weeks just to get the wiring in and get the car turning on"; "lots of communication errors".
  - Running in 2025–26; no cost published.
  - All **REPORTED** (builder's own videos) — `tunezilla_vr6t_s3_build.md`
- TuneZilla's site advertises "Immobilizer Delete" and "ECU Swap Tuning Services". — **REPORTED** (snippet) [TuneZilla Swap Tuning](https://tunezilla.com/blog/300/swap-tuning-1750114528). The page body was empty to WebFetch.

**B. Malaka Motorsports 2018 RS3 8V (California, USA). One of the "VR6 RS3s".**
- Build list: "George and Stav at Malaka Motorsports built their Audi RS3".
  - **Engine:** turbocharged 3.0 L VR6 with DP Engine Parts forged pistons and rods, Turbo Impressions block girdle, Ferrea valvetrain, custom CAT cams, modified 034Motorsport intake manifold, HST exhaust manifold, Garrett G42-1450 79 mm.
  - **Fuel:** E85 through 2150 cc FIC injectors and three Hellcat pumps.
  - **Engine management:** "Syvecs S7 Plus ECU and StavBuilt custom wiring harness".
  - **Gearbox:** "DQ500 seven-speed transmission upgraded with DCT billet flywheel and HD1400 clutch kit".
  - **Output and tune:** 1,138 hp / 807 lb-ft at the hubs on 50 psi, tuned by Stijn Jacobs (Four Stroke Performance).
  - **Not stated:** article dated December 13, 2022; no car generation, location, Haldex, bellhousing method or cost.
  - — **VERIFIED** (article read) [Engine Swap Depot](https://engineswapdepot.com/?p=89770)
- A Facebook video calls it "1100+WHP VRS3 R30 VR6 Turbo Powered Audi RS3" and credits Instagram @malakamotorsports and dyno @turbojoetuned. — **REPORTED** (title) [Facebook/TurboKing](https://www.facebook.com/turbokingtv/videos/1100whp-vrs3-r30-vr6-turbo-powered-audi-rs3-built-by-malaka-motor-sports-fb-mala/480238847597130/)
- Build thread on Audizine, "VR6 Swapped Audi RS3" (at least 4 pages):
  - It names a 2018 RS3, an "R30 VR6" build and a Syvecs S7.
  - The G42-1450 compressor cover's V-band flange was cut off and a short-radius 90° elbow welded on. The downpipe mates to an Integrated Engineering exhaust.
  - A stock VR6 was used as a spare block "for fabrication, wiring, and first start".
  - The plan was to run the car "with Syvecs and the Unitronic TCU". The OP asked whether "the DQ500 is a direct bolt-up and whether the Haldex system would carry over"; no answer was visible.
  - Cost remark from a poster: "Stock motor VR6 = under 600 dollars. Stock motor RS3 = $13,500 - $16,000".
  - A rebuttal to "pointless in an RS3": older cars lack "full digital OEM dashes and the DQ500".
  - — **REPORTED** (snippets; Cloudflare block) [Audizine 906471](https://www.audizine.com/threads/vr6-swapped-audi-rs3.906471/); [page 3](https://www.audizine.com/forum/showthread.php/906471-VR6-Swapped-Audi-RS3/page3); [page 4](https://audizine.com/forum/showthread.php/906471-VR6-Swapped-Audi-RS3/page4?p=14482179)
- VWVortex "2018 8v Audi RS3 VR6 Swap" (Hybrid/Swap forum, ~6 years old):
  - "spare mock up 3.2 VR6 in the RS3" for fitment while a separate motor was built.
  - Waiting on pistons, rods and tool-steel head studs.
  - Intercooler routing, oil/coolant lines and downpipe in progress; NubWorks billet coolant plugs; a YouTube playlist is linked.
  - — **REPORTED** (snippets) [VWVortex 9439273](https://www.vwvortex.com/threads/2018-8v-audi-rs3-vr6-swap.9439273/)
- Videos to watch:
  - "VR6 SWAPPED 2018 AUDI RS3 !!!!!" (series episode 1) — [YouTube OyPgm7xgmL0](https://www.youtube.com/watch?v=OyPgm7xgmL0)
  - "SHE RUNS!!!! AUDI RS3 VR6 SWAP FIRST START" — [YouTube 6LZeLho6eho](https://www.youtube.com/watch?v=6LZeLho6eho)
  - Channel — [Malaka MotorSports YouTube](https://www.youtube.com/MalakaMotorsports)
  - — **REPORTED** (titles)
- Who they are:
  - The channel says "We're not a shop, just two brothers who have a passion for cars"; mailing address 830 E Palmdale Blvd #281, Palmdale CA. — **REPORTED** (snippet) [YouTube channel](https://www.youtube.com/c/MalakaMotorSports/videos)
  - Malaka Motorsports LLC, Lancaster CA, is shown as suspended by the Franchise Tax Board (data as of 7/15/2025). — **REPORTED** [bizprofile](https://www.bizprofile.net/ca/lancaster/malaka-motorsports-llc)
  - Malaka also has a big-turbo VR6 Audi **S4** (not 8V). — **REPORTED** [steemit](https://steemit.com/malakamotorsports/@malakamotorsport/malaka-motorsports-or-big-turbo-vr6-swapped-audi-s4-or-aiming-for-1000hp)
  - Their *other* well-known RS3 is a **five-cylinder** car: Iroz turbo, 708 hp. — **REPORTED** [Modded Euros](https://blog.moddedeuros.com/spotlight-malaka-motorsports-audi-rs3)

**C. Steve Gregorius / L8-Night "RS3 LMS TCR" (Germany). The other "VR6 RS3" people see.**
- **ESD:**
  - "took his modified Audi A3" to the Turboscheune Test & Tune half mile in Germany; best run 321.66 km/h (199.87 mph).
  - "turbocharged 3.0 L VR6" with 1,300 hp, "DQ500 DSG transmission", "4-Motion drivetrain", "LMS TCR widebody".
  - Team: L8-Night Project Cars. Article dated Sep 28, 2021.
  - ECU, generation, bellhousing and cost not given.
  - — **VERIFIED** (article read) [Engine Swap Depot](https://engineswapdepot.com/?p=77207)
- VRSociety (Feb 13, 2020): "VR6 Turbo swapped Audi RS3" credited "@steve_gregorius x @l8.night"; Quaife sequential "being built by the L8.Night folks"; "TCR/LMS Widebody Kit"; source post instagram.com/p/B8hfXgJgjMQ. — **VERIFIED** (post read) [VRSociety](https://vrsociety.tumblr.com/post/190812641051/vr6-turbo-swapped-audi-rs3-shifting-through-a)
- TikTok "INSANE Car Builds! Episode 71" (@jms_oncars): "@steve_gregorius Audi A3 converted into a carbon bodied RS3 LMS TCR with a 1400bhp 3.2l turbo VR6 and sequential box". — **REPORTED** (caption via snippet) [TikTok](https://www.tiktok.com/@jms_oncars/video/7359604387657862432)
- Conflict: 3.0 vs 3.2 L, 1,300 vs 1,400 hp, and DQ500 (2021) vs Quaife sequential (2020 plan, 2024 caption). Most likely the gearbox changed over time (INFERRED); not resolved.

**D. drive2 "SWAP Audi A3 VR6 Turbo" (Russia). A3 8V with a factory-turbo VR6 and MQB electronics.**
- Logbook "SWAP Audi A3 VR6 Turbo — Audi A3 (8V), 2,5 л, 2014 года".
  - Tags: 2.5 L, 300 hp, robotised gearbox, front-wheel drive.
  - Logs the first start of a VR6 turbo taken from a Teramont donor. The immobiliser "привязан полностью" (fully bound) to the DSG and the engine.
  - Lists compatible VR6 turbo codes DDK/DDKA/DPK/DPKA/DME/DMEA "работает с эбу med17.1.62 или MG1", and warns not to confuse them with the 5-cyl 2.5s (DAZA, DNWA, CEPA, CZG, CTS).
  - Photo captions pair the VR6 turbo with a "DQ500 (DQ501)"; "VR6 turbo установлен, готов к запуску".
  - A Passat R36 oil filter sits differently from the RS3 8V filter.
  - Snippet age ~307 days (≈ Dec 2025).
  - — **REPORTED** (snippets; drive2 returned 403) [drive2 720735095761145905](https://www.drive2.ru/l/720735095761145905/)
- Same channel (FAM-BiTurbo), Octavia A7 (also MQB): "Octavia A7 VR6 3.6 Turbo MED17.1.62 — started by binding the DDKA ECU and flashing a stock CDVC ECU to DPKA".
  - The Teramont ECU is 03H907309L (MED17.1.62).
  - A naturally-aspirated MED17.1.62 accepted turbo firmware but needed rewiring; turbo control is on connectors T105/T91; power and CAN are the same.
  - Another post by the author waits on "a new mechatronic" before a start test.
  - — **REPORTED** (snippets) [drive2 Octavia A7](https://www.drive2.ru/l/696237701816390567/)

**E. 2016 S3 8V project (USA, Audizine).**
- The OP was sourcing a "3.6 VR6 Engine (With DQ500), yes it will be turbo'd" from "a 2009 Passat Wagon. The car its going into is a 2016 Audi S3." The thread is about US emissions: replies say the car is tested to its model year (2016 S3 = ULEV2). One reply suggests asking HPA for a home-install flash. ~2 years old; no completion found. — **REPORTED** (snippets) [Audizine 992856](https://www.audizine.com/forum/showthread.php/992856-2016-Audi-S3-getting-a-VR6-Engine-Emission-Questions)
- Audi's 2016 A3/S3 media kit lists the S3 as ULEV2. — **REPORTED** (snippet) [Audi USA media kit](https://media.audiusa.com/assets/documents/original/635-news-2016-audi-a3-s3-media-kit.pdf)

**S3 VR6 builds that are NOT 8V (excluded, recorded so they are not mistaken for 8V)**
- **Beth Rennsporttechnik (Germany).**
  - Car: "Audi S3" that was "no longer powered by the factory turbocharged 1.8 L inline-four"; 1.8T = 8L (INFERRED).
  - Drivetrain: turbo 3.2 VR6, Turbobandit TB70-04, Ecumaster EMU Black, DQ500, AWD.
  - Result: 800+ hp, 10.273 s at 141.3 mph over the quarter mile.
  - — **VERIFIED** [ESD](https://engineswapdepot.com/?p=51183)
- **Mario Kapeller / Team HST (Austria).**
  - Car: "Audi S3", generation not stated; Instagram mk_s3_rs4_limo.
  - Drivetrain: 3.0 VR6 on an HST billet block, Garrett G55, Kotouc 0A6 7-speed sequential, "upgraded 4WD".
  - Result: 1,500 hp; 8.32 s at 182 mph over the quarter mile (Jul 2025).
  - — **VERIFIED** [ESD](https://engineswapdepot.com/?p=135293)
- **Takis Paraskevopoulos / 0-400 Tune 2 Race (Greece).**
  - Car: "Audi S3", generation not stated.
  - Drivetrain: 3.0 R30 VR6, 1,200+ hp, Nissan Skyline R32 AWD driveline (2019).
  - — **VERIFIED** [ESD](https://engineswapdepot.com/?p=48564)
- 8L S3 VR6 builds (Australia; drive2 S3 8L with a TT 3.2) and a Polish a3-club thread (8P-era S3 3.2). — **REPORTED** [Audizine 742451](https://www.audizine.com/forum/showthread.php/742451-S3-8L-VR6-TURBO-BUILD-in-aus); [drive2](https://www.drive2.ru/l/612713850768228813/); [a3-club.net](https://www.a3-club.net/forum/showthread.php?30816-Audi-s3-a-silnik-3-2-VR6-turbo&p=525626)

### Inferences
- **INFERRED, the builder's sightings.**
  - The "one S3" is almost certainly TuneZilla's 2017 S3. It is the only running 8V S3 VR6 found, it is very active on TikTok and YouTube, and it is Canadian.
  - The "several RS3s" most plausibly are:
    - Malaka's 2018 RS3, which has a YouTube series plus Facebook, TikTok and Instagram reposts.
    - Steve Gregorius' A3-based "RS3 LMS TCR", which social captions call an "RS3".
    - Possibly the Russian A3 8V or reposts of the same two cars.
  - Only **one genuine factory RS3 8V** with a VR6 was found.
- **INFERRED, Vortex thread = Malaka.** The VWVortex "2018 8v RS3 VR6 swap" thread and the Audizine thread are very likely the same Malaka car: same 2018 RS3, 3.2 mock-up engine then an R30 build, a YouTube playlist, and the same build era. Not confirmed by name in the snippets.
- **INFERRED, gearbox pattern.** No running 8V VR6 car kept the A3/S3's own DQ250. All four that state a gearbox use a DQ500:
  - TuneZilla: RS3 unit with a machined bellhousing.
  - Malaka: the RS3's own DQ500, adaptation not published.
  - L8-Night: DQ500, later a sequential.
  - drive2: a Teramont-type DQ500/DQ501.
  The constraint is torque (DQ250 ≈ 400 Nm stock), not the platform.
- **INFERRED, two proven ECU routes in an 8V.**
  1. Factory MQB-generation VW ECU: TuneZilla (Atlas MED17) and drive2 (Teramont MED17.1.62 with immobiliser adapted to engine and DSG).
  2. Standalone Syvecs S7 Plus with the factory RS3 TCU running Unitronic software (Malaka).
  No 8V build used a PQ ECU plus CAN converter (that is vd Veer's Golf approach).
- **INFERRED, North America.** Two of the five 8V builds are North American: TuneZilla in Canada and Malaka in California. A third, the 2016 S3, is a US project. The US emissions question (tested to the recipient's model year, ULEV2 for a 2016 S3) is specific to US states with emissions inspection. How Ontario treats a swapped engine was not researched here (see Gaps).

### Gaps
- Malaka: exact bellhousing/adapter solution, whether the Haldex is active and how it is controlled, cost, and current status. The Audizine pages could not be opened. Watch the YouTube series.
- L8-Night: base generation (8V vs 8P), engine size, current gearbox, ECU and cost.
- drive2 A3 8V: owner name, city, bellhousing/flywheel solution, whether quattro was kept (tag says FWD), road status. drive2 blocked.
- No cost figure for any 8V VR6 build was found.
- No Instagram or TikTok post could be opened. Instagram-only builds (e.g., hashtags #vr6rs3, #vr6s3) may exist and were not visible to search.
- Ontario/Canadian emissions and safety-inspection treatment of a VR6-swapped 8V was not researched.

## 2. MQB Golf/TT VR6 builds that kept an Audi/VW MQB gearbox; re-check of the Dewain and HGP leads

### Takeaway
- **Dewain (@dmods480).** The "R32 DSG bellhousing on the Mk7 DSG" Golf R belongs to him. The source is a VRSociety post from May 19, 2021: an MKV R32 DSG bellhousing on the factory Mk7 DSG, APR-tuned TCU, custom TZ Engineering dual-mass flywheel, factory Teramont ECU, and the Teramont's DQ500 planned later. No completion was found.
- **HGP.** Its own page confirms the RS3 DQ500 with a reinforced 8-plate clutch and modified DSG software, but does not say how the gearbox was mated to the VR6. A third-party report calls it "adapted".
- **Other MQB builds on MQB gearboxes:**
  - AW Racing (Poland), TT 8S: turbo 3.6 + DQ500 + Haldex Stage 2.
  - HPA VR550T, Golf R: DDKA on an upgraded **DQ381**.

### Cited Findings
**Dewain, OEM 2.5L VR6 turbo in a Mk7 Golf R (location not stated)**
- "Dewain is currently working on swapping in a Chinese market factory 2.5L VR6 Turbo (DDKA)" from the Teramont.
  - Mounts: "currently installed with factory mounts but those to[o] will be changing after the transmission arrives".
  - Gearbox: "currently using an MKV R32 DSG bell housing on the factory MK7 DSG with an APR tuned TCU and a custom TZ Engineering dual mass flywheel for now", and "will be running the Teramont's DQ500 in the future".
  - ECU: "The ECU will be the factory Teramont ECU and will be tuned to work in the MK7 chassis".
  - Instagram @dmods480; posted May 19, 2021; tags #vrsociety #vrswaptheworld.
  - — **VERIFIED** (post read) [VRSociety Tumblr](https://vrsociety.tumblr.com/post/651662812635152384/oem-25l-vr6-turbo-in-a-mk7-golf-r-dewain-is)
- A search for "dmods480" found no later update; ESD's 2026 "Golf R with a 550 hp Turbo 2.5L VR6" is HPA's car, not Dewain's. — **VERIFIED** (article read) [ESD p=149095](https://engineswapdepot.com/?p=149095)
- Bolt-pattern background (Vortex): the "DSG from VR6-equipped cars has a different bellhousing bolt pattern" and "WILL NOT FIT" a 4-cylinder; the DSG side expects a 6-hole flywheel flange, while an EA888 flywheel has "8 bolts". A later reply claims a VR6 DSG "can be converted… Bolt pattern is the same as the 4-cylinder", in a Mk4 R32/TT context. — **REPORTED** (snippets) [VWVortex 1.8T + DQ250 thread](https://www.vwvortex.com/threads/1-8t-20v-dsg-dq250-complete-project-with-photos-videos-and-racelogic-data.9353965/)
- A DQ250 dual-mass flywheel for VR6/R32 24v with a "10 hole pattern", rated "up to 1000nm", is sold by Carlicious-Parts (Augsburg). — **REPORTED** (listing snippet) [Carlicious](https://www.carlicious-parts.com/Dual-Mass-Flywheel-DSG-DQ250-VR6-R32-24v-10-hole-pattern)
- MQB DQ250 mechatronics are tied to the immobiliser, so a donor unit "will not work on your car" without brand-specific online tooling. — **REPORTED** [rusefi forum](https://rusefi.com/forum/viewtopic.php?p=43352)

**HGP Golf 7 R 3.6 Biturbo (Germany)**
- **Engine:** "VW 3.6 L engine (VR6 R36) with zero mileage", for Golf 7/7.5 R 2014–2019. Compression lowered with a steel intermediate plate; 2× HGP R28 turbos; extra MPI injectors.
- **Gearbox:** "7-speed DSG transmission DQ500" from the Audi RS3; "not possible for manual transmission"; "Reinforced DSG 8-plate clutch"; "Modified DSG software".
- **Electronics:** "Modified engine control unit" (make not named); "In-depth modification of the vehicle electrics (engine wiring harness)"; boost, oil temperature and digital speed shown in the original instrument.
- **Output and approval:** Stage 1 740 PS / 925 Nm, Stage 2 780 hp; "TÜV-approved".
- **Availability:** both stages are now "Nicht mehr verfügbar" (no longer available); no price shown.
- **Not described:** bellhousing, adapter, flywheel and Haldex.
- — **VERIFIED** (vendor page) [HGP product page](https://hgp-turbo.de/en/products/vw-golf-7-r-3-6-biturbo-740ps-und-780-ps); also [HGP car page](https://www.hgp-turbo.de/cars/golf-7-r-3-6-biturbo)
- tuningblog (2019 facelift version): "adaptiertes Audi RS3 DQ500 Getriebe (7-Gang), verstärkt", 790 PS, ~930 Nm (limited). — **REPORTED** (snippet) [tuningblog](https://www.tuningblog.eu/kategorien/autos-von-a-z/2019-hgp-vw-golf-255885/)
- Forum: HGP's reinforcement is in the clutch, not the gearbox; "for a VR6… an adapter is definitely required" to mate a DQ500; DQ500 flange patterns differ between units. — **REPORTED** (snippets) [VWROC](https://www.vwroc.com/forums/topic/21312-the-golf-7r-with-the-rs3-engine-and-dq500-gearbox/page/2/); [meinR](https://www.meinr.com/index.php/Thread/5403-DQ-500-DSG-am-R/)

**AW Racing (Zambrów, Poland), Audi TT 8S (MQB)**
- "built this third-generation Audi TT (8S)": turbocharged 3.6 L VR6, 714 hp / 858 Nm on 98 octane. The factory "S tronic DQ250" was swapped for an "S tronic DQ500 seven-speed", and the "Haldex [upgraded] to a Stage 2", so AWD was kept. ECU not mentioned. Oct 2024. (The article calls the DQ250 "seven-speed"; it is a 6-speed, so that is an article error.) — **VERIFIED** (article read) [ESD](https://engineswapdepot.com/?p=122022)
- A 2017 TT 8S for sale in Warsaw with a turbo 3.6 VR6 "built by R-Performance and AW-Racing": 740 hp / 855 Nm on 100 octane, "DSG DQ500 seven-speed"; May 2023; ECU and AWD not stated. Possibly the same car as above (INFERRED). — **VERIFIED** (article read) [ESD](https://engineswapdepot.com/?p=100692)
- AW Racing also built a Golf 6 R (PQ35, not MQB) with a turbo 3.6, 806 hp. — **REPORTED** [ESD](https://engineswapdepot.com/?p=122414)

**HPA VR550T, Golf R Mk7.5 (MQB gearbox kept)**
- "eight 'VR550T' Golf builds" are complete; 2018–2019 Golf R; DDKA with HGP hybrid turbo; "DQ381 seven-speed automatic transmission with upgraded clutch packs"; 4Motion AWD; 550 hp / 550 lb-ft. Article published May 27, 2026; bellhousing and ECU not stated. — **VERIFIED** (article read) [ESD p=149095](https://engineswapdepot.com/?p=149095)
- HPA's product page reportedly lists "DSG & 6-Speed Manual configurations", while The Autopian says DSG only. This conflicts with the earlier note (The Drive: "DSG-equipped"). — **REPORTED** (snippet) [HPA VR550T for Golf R](https://www.hpamotorsports.com/pages/hpa-vr550t-2-5l-vr6-program-for-golf-r); [The Autopian](https://www.theautopian.com/how-a-prolific-vw-tuner-got-a-hold-of-some-of-vws-last-vr6-engines-and-how-its-using-them-to-build-a-supercar-slayer/)

**Related MQB gearbox evidence (not VR6)**
- drive2, TT (3G/8S) 2.0 with a DQ500 from an RS3: the stock subframe did not fit and a steel subframe with a different part number was fitted. — **REPORTED** (snippet) [drive2 TT DQ500](https://www.drive2.ru/l/615604466837626830/)
- Russian VR6 + DQ500 builds on non-MQB cars:
  - Superb Mk2 with a BWS: "the DQ500 bellhousing doesn't match the VR6"; a diesel flywheel modified to 10 bolts as a stop-gap, then a VR6/DQ500 flywheel ordered from Germany. — [drive2 Superb](https://www.drive2.ru/l/632970703242543924/)
  - Tiguan 1 with a 3.6 + DQ500: "no factory adapter"; the electrics took ~3 days. — [drive2 Tiguan](https://www.drive2.ru/l/581898937888145870/)
  - Both **REPORTED** (snippets)

### Inferences
- **INFERRED, why Dewain's trick works.** On the 02E/DQ250 the bellhousing is a separate casting bolted to the gearbox case. Swapping in the Mk5 R32 (VR6) bellhousing therefore converts an MQB DQ250 to the VR6 bolt pattern, and a VR6-pattern DQ250 dual-mass flywheel (6-hole DSG side, VR6 crank side) completes it.
  - This applies only if his Mk7 R had the **6-speed DQ250**, as did US Golf R 2015–2017. The 2018+ Golf R uses the 7-speed DQ381.
  - It is directly relevant to an NA A3 2.0T quattro, which has the 6-speed S tronic DQ250 family.
  - The torque ceiling (~400 Nm stock) is why Dewain planned a DQ500 and why every high-power build moved to a DQ500.
- **INFERRED, Teramont DQ500.** The Teramont/DDKA was paired with a DQ500 at the factory (Dewain's post; drive2 "DQ500 (DQ501)"). That makes it the only factory-VR6-pattern DQ500 in the parts system, so it is the natural "bolt-on" DQ500 for an EA390 VR6. Exporting one from China or Russia is impractical in North America.
- **INFERRED, "TZ Engineering".** "TZ Engineering" in Dewain's post might be TuneZilla, which also uses the "TZ" prefix on its product codes (e.g., TZ301BL). Unconfirmed; ask Dewain or TuneZilla.
- **INFERRED, HGP's method.** The RS3 DQ500 carries a 4/5-cylinder bellhousing pattern. Given that, and the European aftermarket's standard method (mill the DQ500 bellhousing and fit a VR6 adapter plate; see section 3), HGP very likely used a machined RS3 DQ500 with a VR6 adapter plate or VR6 flywheel. This is not documented.

### Gaps
- Whether Dewain's Mk7 R was a 6-speed DQ250 or a 7-speed DQ381; whether the build was finished; TZ Engineering's identity and flywheel part number.
- HGP's bellhousing/adapter details, ECU make, Haldex handling and former price.
- AW Racing: ECU, bellhousing method and cost.
- HPA VR550T: how the DQ381 was mated to the DDKA.

## 3. Who sells this conversion or its key parts, and at what price?

### Takeaway
No shop anywhere was found selling a VR6 conversion for the S3/RS3/A3 8V as a product, including the Middle East, Russia, Poland and the US. Of the shops that have done 8V or MQB VR6 work:
- **TuneZilla (Canada):** the only one with a running 8V S3 and an Atlas-ECU calibration. Sells immobiliser-delete and swap tuning; price not published.
- **HPA:** sells only the Golf R VR550T (US$40k, previously noted).
- **HGP:** the Golf 7 R 3.6 package is discontinued.
- **AW Racing (Poland):** has built MQB TT 8S VR6 cars.

The bellhousing problem has off-the-shelf solutions from HPA, HST, Racing Custom Parts, CCT and CNC-Technik, with machining from about €200.

### Cited Findings
- **TuneZilla** (Canada): "Immobilizer Delete" and "ECU Swap Tuning Services" are listed; no price. — **REPORTED** [TuneZilla](https://tunezilla.com/blog/300/swap-tuning-1750114528); context in `tunezilla_vr6t_s3_build.md`
- **HPA "VR6 7 Speed DSG Conversion (DQ500)"** for the 3.2 VR6: includes "DQ500 bell housing machining, CNC transmission adapters, and shifter cable adapter parts"; price not captured. — **REPORTED** (snippet) [HPA DQ500 conversion](https://www.hpamotorsports.com/products/dq500-conversion)
- **Racing Custom Parts:** one-piece "VR6 / R32 / R36 to DSG DQ500 NZS adapter", which needs bellhousing machining (listed at about **€200**); a dual-mass flywheel is available. — **REPORTED** (snippet) [Racing Custom Parts](https://racingcustomparts.com/produkt/vr6-r32-r36-to-dsg-dq500-nzs-adapter/)
- **HST Turbotuning (Austria):** "DQ500 Fräsen und Adapterplatte" for R32/R36/VR6. They mill the customer's gearbox or bellhousing and fit an adapter plate; the gearbox is not included in the price. — **REPORTED** (snippet) [HST](https://eu.hst-tuning.com/getriebe/dq500/dq500-fraesen-und-adapterplatte/hstg-dq500-f-ap)
- **CCT-Motorsport** lists a "DQ500 bell housing modified for 6-cylinder" in DQ250→DQ500 packages (TT 8J / Golf 5). **CNC-Technik** mills a customer-supplied DQ500 bellhousing for 6-cylinder use. A Kleinanzeigen ad offers "DQ500 Umarbeitung Getriebeglocke inkl. Platten 6Zylinder R32 Turbo" (Pirna). — **REPORTED** (snippets) [CCT](https://www.cct-motorsport.de/Getriebe-Technik/Umbau-DQ250-auf-DQ500-Audi-TT8J-VW-Golf-5::1727.html); [Kleinanzeigen](https://www.kleinanzeigen.de/s-anzeige/dq500-umarbeitung-getriebeglocke-inkl-platten-6zylinder-r32-turbo/2075799539-223-14508)
- **TVS Engineering** DQ500 conversion kits list VR6 applications for the 8P A3, but for the 8V only the 2.0 TFSI EA888 Gen3. — **REPORTED** (snippet) [TVS](https://tvsengineering.com/en/news/tvs-dq500-conversion-kits-now-available-for-all-dq250-dq380-and-dq381-vehicles/)
- **IS-Racing (Germany):** MQB Golf 7 / **Audi S3 8V** manual-to-DSG conversion from **€5,999** (FWD), including parts, harness, electrics, assembly and software. A €2,899 figure appears next to a reinforced DQ500 clutch, and the mapping between prices and variants is unclear. — **REPORTED** (snippet) [IS-Racing](https://www.is-racing.de/getriebeumbauten-und-dsg/)
- **Syvecs:** "DQ250 / DQ500 MQB 2015+ Gearbox Control Firmware" communicates with the OEM TCU "allowing the transmission to be mated with any engine and chassis". Syvecs also sells an MQB Haldex Gen5 controller for RS3 / Golf R / S3; one firmware version is sold only through Iroz Motorsport. — **REPORTED** (snippets) [Syvecs DQ firmware](https://www.syvecs.com/product/dq250-dq500-mqb-2015-gearbox-control-firmware/); [Syvecs AWD controller](https://www.syvecs.com/product/awd-4wd-controller-vag-mqb-rs3-golf-s3/)
- **vd Veer:** an MQB↔PQ CAN converter is shown at €500 (direction to be checked). — **REPORTED** (snippet) [vd Veer](https://www.vdveer-engineering.nl/en/projects/2-golf-7-r36)
- **Donor gearbox price:** used complete Golf R Mk7.5 7-speed DSG at US$6,799.95 on eBay. — **REPORTED** [eBay](https://www.ebay.com/itm/116721372495)
- **Cost remark:** "Stock motor VR6 = under 600 dollars; Stock motor RS3 = $13,500 - $16,000" (US forum). — **REPORTED** [Audizine 906471](https://www.audizine.com/threads/vr6-swapped-audi-rs3.906471/)
- **Middle East:** a search for Kuwait/Dubai/Saudi RS3 or 8V VR6 swaps returned nothing region-specific. — (absence noted) [search returned only US/EU results]

### Inferences
- **INFERRED.** For a Canadian builder, TuneZilla is the obvious first call. It is in Canada, has already solved the Atlas-ECU-in-an-8V wiring and calibration, and knows the RS3 DQ500, mount and radiator-support package. For the bellhousing, the choice is:
  - TuneZilla's route: machine the RS3 DQ500 bellhousing and use a VR6 flywheel.
  - The HPA/HST/Racing Custom Parts adapter route.
  - Dewain's route: an R32 bellhousing on the A3's own DQ250, for a near-stock-power NA 3.6 only.
- **INFERRED.** Malaka shows that the standalone route (Syvecs S7 Plus + Unitronic-tuned OEM TCU) also works in an 8V at very high power. Syvecs' MQB DQ firmware and Haldex controller cover the gearbox and AWD pieces. Expect a high cost (Syvecs ECU + harness + TCU software), but no prices were found.

### Gaps
- No price for TuneZilla swap calibration, the HPA DQ500 conversion, HST milling, the Syvecs DQ firmware or the Haldex controller.
- No turnkey 8V VR6 offer anywhere. No Middle East, Russian or Polish shop offer found.

## 4. "VR6 RS3" confusion check

### Takeaway
Many "RS3 swap" posts are the RS3's **EA855 2.5 five-cylinder** going into other cars, not a VR6 going into an RS3. "8v to vr6 swap" threads are 8-valve VW four-cylinders, not the Audi 8V. One of the two prominent "VR6 RS3s" (L8-Night) is an A3 wearing an RS3 LMS TCR body.

### Cited Findings
- Five-cylinder (not VR6) results that surface in "RS3 VR6" searches:
  - VWVortex "RS3 Engine Install" and "VR6 or RS3 swapping an Amarok" (choice between the two engines).
  - TikTok "Golf 6r swap rs3".
  - Audizine "Engine swap 8V a3/s3 w/ RS3 engine?".
  - ESD "AWD Audi A1 Race Car with a Turbo 2.5 L Inline-Five" (filed under the RS 3 category).
  - Iroz, SAR and TTE "RS3 8V turbo kits", which are for DAZA/DNWA.
  - — **REPORTED** (titles/snippets) [Vortex RS3 Engine Install](https://www.vwvortex.com/threads/rs3-engine-install.9563584/); [Vortex Amarok](https://www.vwvortex.com/threads/vr6-or-rs3-swapping-an-amarok.9493594/); [TikTok](https://www.tiktok.com/discover/golf-6r-swap-rs3); [Audizine 743924](https://www.audizine.com/forum/showthread.php/743924-Engine-swap-8V-a3-s3-w-RS3-engine); [ESD RS 3 category](https://engineswapdepot.com/?cat=755) (VERIFIED: the category lists only two VR6-into-RS3/A3 articles, Malaka and L8-Night, plus the A1 five-cylinder and an electric RS3 TCR)
- Threads titled "8v to vr6 swap" are 8-valve Mk2-era engines. — **REPORTED** (titles) [mk2vr6.com](https://www.mk2vr6.com/board/viewtopic.php?t=6778); [VWVortex](https://forums.vwvortex.com/showthread.php?1926442-8v-to-vr6-swap=)
- L8-Night's car: "@steve_gregorius Audi A3 converted into a carbon bodied RS3 LMS TCR". — **REPORTED** [TikTok](https://www.tiktok.com/@jms_oncars/video/7359604387657862432); ESD calls it an "Audi A3" — **VERIFIED** [ESD](https://engineswapdepot.com/?p=77207)
- Malaka has both a VR6 RS3 and a separate five-cylinder Iroz RS3 (708 hp), which makes their "RS3" posts easy to conflate. — **REPORTED** [Modded Euros](https://blog.moddedeuros.com/spotlight-malaka-motorsports-audi-rs3)
- The drive2 A3 8V author warns that "2.5 VR6 turbo" (DDK/DDKA/DPK/DME) is not the 2.5 five-cylinder (DAZA/DNWA/CEPA). — **REPORTED** [drive2](https://www.drive2.ru/l/720735095761145905/)

### Inferences
- **INFERRED.** "Several VR6 RS3s" on social media most likely means repeated reposts of two or three cars: Malaka, L8-Night, and possibly the Russian A3. Only Malaka's is a factory RS3 8V.
- **INFERRED.** The Teramont "2.5T" adds its own confusion: listings and tags saying "2.5" on an A3 8V can mean either a DAZA five-cylinder or a DDKA VR6.

### Gaps
- Instagram-only VR6 RS3s may exist that search engines do not index; they could not be checked.

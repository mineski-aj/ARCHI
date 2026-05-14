# ARCHI — MINESKI EXECUTION TYPES REFERENCE

**Cost Estimate Skeleton Library**
*Operations Department · v1.0 · Companion to ARCHI Master Initialization Guide*

> **Document Purpose:** This is ARCHI's pattern-matching reference for Cost Estimate construction. When a user describes an event scope, ARCHI maps it to one of the execution archetypes below and pulls the standard crew, asset, and line-item skeleton — then anchors every cost line to verified Andon Board POs before applying the 0.64 divisor. This file does NOT replace vendor quotes; it sets the cost floor and the structural completeness check.

---

## HOW ARCHI USES THIS FILE

1. **Match the scope to an archetype.** User says "GG Truck activation," "mall esports day," "studio rebroadcast" → ARCHI snaps to the matching execution profile.
2. **Pull the standard line-item skeleton.** Each archetype carries a default crew + asset + logistics structure. Missing line items get flagged immediately.
3. **Anchor every line to historical POs.** Rate ranges shown per archetype come from verified Andon Board entries (project references included). Any line without a Mineski PO anchor must be flagged as `UNANCHORED — fresh quote required`.
4. **Apply hidden-cost injection rules per archetype.** Each execution type has known bleed points (overnight meals, tap-in fees, trucking surcharges). These are listed and auto-injected.
5. **Apply 0.64 divisor for client quote.** 36% GP mandate is non-negotiable.

---

## EXECUTION TYPE INDEX

| # | Archetype | Typical Scale | COGS Range (PHP) | Key Asset |
|---|---|---|---|---|
| 1 | **Studio Execution** | Multi-day, 100–500 pax | ₱1.5M – ₱8M+ | Mineski Studio + AAA AV |
| 2 | **GG Truck Execution** | 1–3 days, 30–200 pax | ₱50K – ₱250K | GG Truck (internal asset) |
| 3 | **Mall Execution (Esports)** | 2–7 days, 200–2000 pax/day | ₱200K – ₱1.5M | Booth + LED + Mall Permit |
| 4 | **Outpost / Booth Execution** | 1–4 days, 50–500 pax | ₱40K – ₱300K | Mineski Outpost Booth |
| 5 | **Tournament Execution** | 1–5 days, 50–500 pax | ₱80K – ₱600K | Gaming PCs + Tournament Ops |
| 6 | **Grassroots Execution** | 1–2 days, 30–150 pax | ₱20K – ₱80K | Minimal kit, single-site |
| 7 | **Major Studio Event (AAA)** | 4–12 weeks, 1000+ pax | ₱5M – ₱30M+ | SMX/MOA/AAA venue + full broadcast |
| 8 | **Roadshow / Multi-City Tour** | 3–10 stops, 50–300 pax/stop | ₱150K – ₱1.5M | GG Truck or modular booth + travel |
| 9 | **Online / Virtual Execution** | 1 day – 8 weeks | ₱30K – ₱500K | Remote broadcast stack |

---

# 1 · STUDIO EXECUTION

**Definition:** Controlled studio environment, fixed venue (Mineski Studio or partner studio), full broadcast production. Rebroadcasts, league weekly nights, branded streams.

**Reference projects:** Kings Invitational Series Rebroadcast S4 (KIS S4) · MPL PH S15 / S16 / S17 weekly nights · HOK PKL Spring Season studio days

### Standard Scope
- **Duration:** 1–14 event days + ingress/rehearsal days (typically 1.5x event-day count)
- **Headcount:** 30–80 internal + outsourced crew, 50–300 audience/talent
- **Venue:** Mineski-owned studio or rented studio (booth fab + LED fascia + audience riser)

### Standard Line-Item Skeleton
| Category | Line Item | Andon Board Anchor (PHP) | Source |
|---|---|---|---|
| Talent | Outsourced Caster (per event) | 15,000 – 112,000 | KIS S4, MPL S17 |
| Talent | Outsourced Host | 12,000 – 89,200 | CCAP MLBB, SM Cyberzone |
| Talent | Outsourced HMUA | 6,000 – 79,500 | CCAP, PKL Spring |
| Broadcast | Lead Stream Engineer | 18,000 | KIS S4 |
| Broadcast | Audio Engineer | 2,200 – 18,000 | CCAP, KIS S4 |
| Broadcast | Main CG Operator / Director | 24,000 | KIS S4 |
| Broadcast | Floor Manager / Talent Manager | 15,300 | KIS S4 |
| Broadcast | Broadcast Manpower (per head) | 7,200 – 25,650 | KIS S4, Jobstreet Level Up |
| Broadcast | Live Camera Gimbal Operator | 80,640 | KIC 2025 Addendum |
| Structural | Booth Rental / Fabrication | 135,520 – 400,000 | KIS S4, SM Cyberzone |
| Structural | SOFA Set / Furniture | 33,000 | KIS S4 |
| Technical | LED Wall (indoor 9x12) | 20,000 – 35,000 | PUBG Mobile 8th Anniv |
| Technical | LED + Lights + Sounds bundle | 102,040 – 200,000 | Cobra Core, SM Cyberzone |
| Technical | Full Technical Services (LED/Lights/Sounds/Genset) | 1.4M – 7.4M | GTCC, KIC, MPL S17 |
| Logistics | Outsourced Logistics Associate (per head) | 6,000 – 51,000 | Multi-project |
| Logistics | Logistics Services - Closed Van | 7,060 – 15,000 | CCAP, KIS S4 |
| Crew Welfare | Crew Meals (per meal) | 130/pax | Standardized |
| IT | Outsourced IT Associate | 1,670 – 62,400 | CCAP → MPL S17 |

### Hidden Cost Injection (Auto-Apply)
- **Overnight rehearsal meals** (24-hr meal tier) if ingress day extends past 10pm
- **Studio tap-in / electrical fees** if external studio
- **Talent overtime** beyond contracted call time
- **Equipment overtime** for ingress days past 12 hours
- **Trucking egress surcharge** for late-night strike (after 11pm)

### Flag Conditions
- 🚨 No HMUA budgeted for on-cam talent → escalate
- 🚨 No Audio Engineer line → broadcast fail risk
- 🚨 Genset not budgeted on extended call → power outage risk

---

# 2 · GG TRUCK EXECUTION

**Definition:** Mobile activation using the **GG Truck** — Mineski-owned asset with onboard LED display and built-in PA. Deployed to barangay-level, school, mall driveway, or community sites for one-off or short-burst brand activations.

**Reference projects:** *(GG Truck is an internal CapEx asset — does not appear as a procurement line. Cost is built bottoms-up from fuel + crew + LED tech + maintenance reserve, NOT as an external rental.)*

### Standard Scope
- **Duration:** 1–3 event days, single-site or multi-stop within metro/province
- **Headcount:** 3–6 crew, 30–200 audience
- **Venue:** Barangay covered court, mall driveway, school grounds, public plaza

### Standard Line-Item Skeleton
| Category | Line Item | Andon Board Anchor (PHP) | Source |
|---|---|---|---|
| Asset (Internal) | **GG Truck Day Rate** | ⚠ INTERNAL — confirm with Finance | Not in Andon |
| Asset (Internal) | Fuel (RT, metro/nearby province) | 2,000 – 4,000 | Market |
| Asset (Internal) | Toll + parking | 500 – 1,500 | Market |
| Crew | Driver | 2,800 – 3,500 | Jobstreet Logistics Assoc anchor |
| Crew | LED Operator / Tech | 2,500 | CCAP CXtreme |
| Crew | Broadcast Associate (grassroots scale) | 4,000 | PESO Grassroots |
| Crew | IT Associate | 1,670 – 6,680 | CCAP, SM Cyberzone |
| Crew | Outsourced Host (regional/1-day) | 10,900 – 12,000 | PUBG Davao, CCAP MLBB |
| Crew | Outsourced Road Manager | 2,200 | CCAP CXtreme |
| Crew | Outsourced Audio Engineer | 2,200 | CCAP CXtreme |
| Lighting | Basic Par Cans + Stands + DMX | ⚠ UNANCHORED — fresh quote | None in Andon |
| Crew Welfare | Crew Meals (3 meals × ₱130) | 130/pax/meal | Standardized |
| Permits | Barangay coordination / honorarium | 1,500 – 3,000 | Discretionary |
| Consumables | Gaffer tape, batteries, zip ties, extensions | 500 – 1,500 | Discretionary |

### Hidden Cost Injection (Auto-Apply)
- **Extended call OT** for any deployment > 12 hours (driver, LED tech, broadcast)
- **Genset standby** if barangay venue has unreliable power (₱3,000–₱5,000)
- **Vehicle insurance allocation** if GG Truck deployed outside metro
- **Second driver / co-driver** for any deployment > 14 hours OR provincial distance

### Flag Conditions
- 🚨 **GG Truck internal day rate not declared** → escalate to Finance for asset chargeback rate
- 🚨 No backup power for outdoor/barangay venue → power-outage risk
- 🚨 No host budgeted but deployment has audience interaction → scope gap
- 🚨 Audio scope assumed via GG Truck onboard PA — confirm operational, otherwise add external PA (₱3K–₱5K)

### Pricing Floor Estimate (Reference Only — 1 day, 50 pax, nearby province)
- Manpower + meals: ~₱25,000
- Truck operating (fuel + tolls): ~₱4,000
- Lighting: ~₱5,500
- Permits + consumables: ~₱2,500
- Contingency (10%): ~₱3,700
- **Sub-total before GG Truck asset rate:** ~₱40,700
- **+ GG Truck day rate (TBD from Finance):** ₱X
- **Client Quote = Total ÷ 0.64**

---

# 3 · MALL EXECUTION (ESPORTS)

**Definition:** Multi-day esports activation inside a mall environment — fabricated booth, LED, gaming PC setup, league ops, ushers, and mall-mandated security/insurance.

**Reference projects:** SM Cyberzone Trading Card Game (TCG) Activation · PUBG Mobile 8th Anniversary Event

### Standard Scope
- **Duration:** 2–7 days (ingress + event + egress)
- **Headcount:** 8–25 crew, 200–2,000 daily foot traffic
- **Venue:** Mall atrium, cyberzone, activity center

### Standard Line-Item Skeleton
| Category | Line Item | Andon Board Anchor (PHP) | Source |
|---|---|---|---|
| Structural | Stage/Booth Fabrication (rental) | 400,000 | SM Cyberzone TCG |
| Technical | LED + Lights + Sounds | 139,440 – 200,000 | SM Cyberzone TCG |
| Technical | LED Wall (indoor 9x12) | 20,000 – 35,000 | PUBG Mobile 8th |
| Tournament | Gaming PC Rental (per day) | 7,500 | Jobstreet Level Up |
| Tournament | League Operations (per day) | 1,700 – 3,400 | SM Cyberzone TCG |
| Talent | Outsourced Caster | 10,000 – 44,000 | SM Cyberzone TCG |
| Talent | Outsourced Host | 12,000 – 89,200 | CCAP, SM Cyberzone |
| Crew | Outsourced Usher (per day) | 1,500 – 3,000 | SM Cyberzone TCG |
| Crew | Outsourced Road Manager | 6,400 (4 days) | SM Cyberzone TCG |
| Crew | Outsourced IT Associate | 6,680 | SM Cyberzone TCG |
| Crew | Broadcast Manpower | 20,000 | SM Cyberzone TCG |
| Logistics | Logistics Associates (ingress + event + egress) | 30,000 | SM Cyberzone TCG |
| Comms | Beyblade / Community Organizer | 70,000 | SM Cyberzone TCG |
| Media | Photo & Video Doc Team | 70,000 – 215,000 | SM Cyberzone, PKL |
| Crew Welfare | Crew Meals (per meal) | 130/pax | Standardized |

### Hidden Cost Injection (Auto-Apply)
- **Mall electrical tap-in fees** (varies by mall — SM, Ayala, Robinsons each have own rate)
- **Mall booth permit / activation permit**
- **Mall-mandated security marshals** (some malls require client-paid)
- **Mall insurance bond** (especially for >3 day activations)
- **Custodial / cleaning fee** for mall atrium post-egress

### Flag Conditions
- 🚨 No mall tap-in fee budgeted → margin bleed risk
- 🚨 No mall permit budgeted → activation blocked at ingress
- 🚨 Booth fabrication via Mangotree or Stage One → check monopoly leverage

---

# 4 · OUTPOST / BOOTH EXECUTION

**Definition:** Mineski-branded booth deployed at a third-party event (alumni reunion, corporate event, school fair, expo). Smaller footprint than mall activation. Often refurbishing existing Outpost asset.

**Reference projects:** Mineski Outpost — Don Bosco Alumni 2001 · Mineski Outpost — corporate/school deployments

### Standard Scope
- **Duration:** 1–2 event days, minimal ingress
- **Headcount:** 4–8 crew
- **Venue:** External event grounds, function hall, school covered court

### Standard Line-Item Skeleton
| Category | Line Item | Andon Board Anchor (PHP) | Source |
|---|---|---|---|
| Asset | Refurbishment of Outpost Booth | 40,000 | Don Bosco Alumni 2001 |
| Logistics | Outsourced Logistics Services (Trucking) | 15,000 | Don Bosco Alumni 2001 |
| Crew | Outsourced Logistics Associates | 7,500 | Don Bosco Alumni 2001 |
| Furniture | Cocktail Tables w/ Cover (per set) | 1,400 | Don Bosco Alumni 2001 |
| Tournament | Gaming PC Rental (per unit/day) | 7,500 | Jobstreet Level Up |
| Talent | Outsourced Host (small scale) | 10,900 – 12,000 | PUBG Davao, CCAP |
| Crew Welfare | Crew Meals (per meal) | 130/pax | Standardized |

### Hidden Cost Injection (Auto-Apply)
- **Trucking surcharge** for provincial deployment
- **Outpost asset repair reserve** (5–10% of refurb cost as standing line)
- **External venue tap-in / electrical fee** if not host-provided
- **Crew transport** if event > 1 hr drive from base

### Flag Conditions
- 🚨 No Outpost refurbishment line on first-deployment-of-year → asset wear risk
- 🚨 Trucking not budgeted → ingress fail

---

# 5 · TOURNAMENT EXECUTION

**Definition:** Competitive esports tournament — refs, game observers, league ops, gaming PCs, brackets, trophies. Can be standalone or wrapped inside Mall/Studio execution.

**Reference projects:** CCAP CXtreme MLBB Tournament · Jobstreet Level Up v2 · MCGG Rising Stars S4

### Standard Scope
- **Duration:** 1–5 event days + qualifiers
- **Headcount:** 8–20 crew + competing teams
- **Venue:** Studio, mall, university, or LAN center

### Standard Line-Item Skeleton
| Category | Line Item | Andon Board Anchor (PHP) | Source |
|---|---|---|---|
| Tournament | Outsourced Head Referee | 4,650 | Jobstreet Level Up |
| Tournament | Outsourced Referee (per head) | 2,700 | Jobstreet Level Up |
| Tournament | Outsourced Game Observer | 3,600 | Jobstreet Level Up |
| Tournament | Outsourced Game Director | 4,400 | Jobstreet Level Up |
| Tournament | League Operations (per day) | 1,700 – 3,400 | SM Cyberzone TCG |
| Tournament | Gaming PC Rental (per unit/day) | 7,500 | Jobstreet Level Up |
| Talent | Outsourced Caster | 10,000 – 18,000 | Jobstreet, CCAP |
| Crew | Player Hospitality | 3,300 | Jobstreet Level Up |
| Crew | Team Liaison Officer | 1,500 | CCAP CXtreme |
| Awards | 7" Acrylic Trophies (per unit) | 2,800 | Jobstreet Level Up |
| Awards | Trophy Fabricator (custom) | 48,500 | PKL Spring |
| Crew Welfare | Crew & Talent Meals (per meal) | 130/pax | Standardized |

### Hidden Cost Injection (Auto-Apply)
- **Prize pool taxes** if cash prize > ₱10,000 (20% withholding)
- **Server cost** if online qualifiers required
- **Player transport / hospitality** for grand finals teams
- **Anti-cheat / replay review labor** for online stages

### Flag Conditions
- 🚨 No Head Referee budgeted → integrity risk
- 🚨 Prize pool with no withholding tax line → BIR exposure

---

# 6 · GRASSROOTS EXECUTION

**Definition:** Lowest-cost barangay-level or community activation. Single-day, minimal kit, minimal crew. Often partner-subsidized (LGU, PESO, NGO).

**Reference projects:** PESO National Grassroots Program

### Standard Scope
- **Duration:** 1 day
- **Headcount:** 2–4 crew, 30–150 audience
- **Venue:** Barangay hall, covered court, public school

### Standard Line-Item Skeleton
| Category | Line Item | Andon Board Anchor (PHP) | Source |
|---|---|---|---|
| Crew | Outsourced Broadcast Associate | 4,000 | PESO Grassroots |
| Crew | Outsourced Logistics Associate (1-day) | 2,800 – 6,000 | Jobstreet, PKL |
| Crew | Outsourced Host (regional) | 10,900 | PUBG Mobile Davao |
| Logistics | Trucking (small van) | 7,060 – 15,000 | CCAP, Don Bosco |
| Crew Welfare | Crew Meals (per meal) | 130/pax | Standardized |
| Permits | Barangay courtesy / honorarium | 1,500 – 3,000 | Discretionary |

### Hidden Cost Injection (Auto-Apply)
- **LGU coordination fee** if barangay is outside Mineski's standing partner list
- **Backup genset** if barangay venue has no reliable power

### Flag Conditions
- 🚨 Grassroots tier client expecting AAA-tier deliverables → scope-vs-budget mismatch
- 🚨 No backup power for outdoor barangay event → activation fail risk

---

# 7 · MAJOR STUDIO EVENT (AAA)

**Definition:** Flagship multi-week productions — MPL season finals, KIC group stage + playoffs. AAA venue (SMX, MOA Arena, Araneta), full broadcast stack, multi-camera, audience tiering.

**Reference projects:** MPL PH S15 / S16 / S17 · KIC 2025 Group Stage / Knockouts / Playoffs · GTCC Summer Showdown / September Arena · HOK PKL Spring Season

### Standard Scope
- **Duration:** 4–12 weeks (ingress + rehearsal + event days + egress)
- **Headcount:** 80–200+ crew, 1,000–5,000+ audience
- **Venue:** SMX, MOA Arena, Araneta, World Trade Center, Marriott Grand Ballroom

### Standard Line-Item Skeleton
| Category | Line Item | Andon Board Anchor (PHP) | Source |
|---|---|---|---|
| Technical | Full Technical Services (Lights/Sounds/Camera/Genset) | 4.4M – 7.4M | MPL S15, KIC 2025 |
| Technical | Generator Diesel (37 days, 2 gensets) | 580,160 | MPL S17 Addendum |
| Technical | LED Rental (regular season) | 944,844 | HOK PKL Fall |
| Structural | Booth & Players' Area Fabrication | 220,000+ | PKL Spring |
| Structural | Additional On-ground Fabrication | 92,400 | KIC 2025 |
| Broadcast | Broadcast Manpower (per head) | 25,650 – 140,000 | KIS S4, MPL S17 |
| Broadcast | Broadcast Manager | 240,000 | MPL S17 |
| Talent | Caster (premium tier) | 50,000 – 120,000+ | MPL S17, KIS S4 |
| Talent | Talent Manager | 96,700 | MPL S17 |
| Talent | HMUA Bundle | 79,500+ | PKL Spring |
| Talent | Stylist | 120,000 | MPL S17 |
| Media | Photo & Video Doc Team | 215,000+ | PKL Spring |
| Crew | Event Security Marshals | 15,000 – 27,200 | KIC, PKL Spring |
| Crew Welfare | Crew Meals (per meal × pax × days) | 130/pax | KIS S4 (745 meals), PKL Spring (1,613 meals) |

### Hidden Cost Injection (Auto-Apply)
- **24-hour overnight meal tier** for any ingress day extending past 10pm
- **SMX / MOA Arena tap-in fees** (significant — venue-specific)
- **Equipment overtime** for rehearsal days > 12 hrs
- **Hotel + per diem** for out-of-town talent / crew
- **Custom trophy fabrication** for grand finals
- **Insurance bond** for AAA venue
- **Backup genset standby** even if venue has primary power

### Flag Conditions
- 🚨 Supplier monopoly risk: **Stage One Events** (structural) and **XSTATIC** (AV) — always request alt quotes for leverage
- 🚨 No 24-hr meal line on ingress days → labor compliance risk
- 🚨 Caster/Talent fees without withholding tax line → BIR exposure

---

# 8 · ROADSHOW / MULTI-CITY TOUR

**Definition:** Same activation deployed across 3+ cities sequentially. Either GG Truck-anchored or modular booth-anchored. High logistics weight.

**Reference projects:** *(Roadshow patterns appear across Mineski Outpost school tours, PUBG Mobile anniversary tour stops — composite reference.)*

### Standard Scope
- **Duration:** 3–10 stops over 2–8 weeks
- **Headcount:** 4–10 traveling crew, 50–300 audience per stop
- **Venue:** Multi-city mix — malls, schools, plazas, gymnasiums

### Standard Line-Item Skeleton
| Category | Line Item | Notes |
|---|---|---|
| Logistics | Trucking (per leg) | ₱15,000 base anchor × n legs |
| Logistics | Crew transport (per leg) | Plane tickets / van / fuel |
| Asset | GG Truck OR modular booth | Internal asset OR rental |
| Crew | Traveling crew (4–8 heads × n days) | Multiply daily rates |
| Crew Welfare | Per diem / lodging | ₱1,500–₱2,500/pax/day |
| Crew Welfare | Crew meals | ₱130 × 3 × pax × days |
| Permits | Per-city permits | Barangay / mall / school each |
| Local Hire | Local hosts / ushers per city | Reduces travel cost |

### Hidden Cost Injection (Auto-Apply)
- **Rest day meals + lodging** between stops
- **Equipment swap-out reserve** for breakages mid-tour
- **Local taxes** per LGU
- **Force majeure buffer** (typhoon stops) — 10% line

### Flag Conditions
- 🚨 Roadshow scoped at single-event rates → underbudget risk
- 🚨 No per diem line → labor compliance violation
- 🚨 Single-truck routing without breakdown reserve → tour-killer risk

---

# 9 · ONLINE / VIRTUAL EXECUTION

**Definition:** Fully remote broadcast or hybrid (small studio + remote talent). No physical audience.

**Reference projects:** Various MPL online qualifiers, Adtechinno-style PR/AD placements, online community events

### Standard Scope
- **Duration:** 1 stream day to 8-week online season
- **Headcount:** 4–15 crew (most remote)
- **Venue:** Mineski studio + remote talent home setups

### Standard Line-Item Skeleton
| Category | Line Item | Notes |
|---|---|---|
| Broadcast | Lead Stream Engineer | ₱18,000 anchor (KIS S4) |
| Broadcast | Broadcast Manpower | ₱7,200 – ₱25,650 |
| Talent | Remote Caster (per match/day) | ₱10,000 – ₱50,000 |
| Talent | Host | ₱12,000 – ₱89,200 |
| Tech | Cloud production / vMix license | Subscription |
| Tech | Remote talent kit (cam/mic/light shipped) | Per-talent |
| Tournament | Online tournament admin | League ops anchor |
| Media | Stream graphics / overlays | Outsourced |

### Hidden Cost Injection (Auto-Apply)
- **Streaming platform fees** (YouTube/Twitch — usually free, but watch for ingest CDN)
- **Talent home internet stipend** for low-bandwidth players
- **Anti-cheat license** for online competitive

### Flag Conditions
- 🚨 No remote talent tech kit budgeted → broadcast quality risk
- 🚨 Server downtime / replay infrastructure missing → integrity risk

---

## STANDING CROSS-EXECUTION RATE ANCHORS

*Reference table used across all archetypes — always confirm against latest Andon Board.*

| Role / Item | 1-Day Floor | Multi-Day Reference | Premium Tier | Source Project |
|---|---|---|---|---|
| Host | 10,900 | 12,000 | 89,200 | PUBG Davao → SM Cyberzone |
| Caster | 10,000 | 15,000–50,000 | 112,168 | Jobstreet → KIS S4 |
| HMUA | 6,000 | — | 79,500 | CCAP → PKL Spring |
| Audio Engineer | 2,200 | — | 18,000 | CCAP → KIS S4 |
| Lead Stream Engineer | — | 18,000 | — | KIS S4 |
| Main CG Operator/Director | — | 24,000 | — | KIS S4 |
| Broadcast Manpower | 7,200 | 25,650 | 140,000 | Jobstreet → KIS S4 → MPL S17 |
| Broadcast Manager | — | — | 240,000 | MPL S17 |
| IT Associate / IT Support | 1,670 | 6,680 | 62,400 | CCAP → SM Cyberzone → MPL S17 |
| LED Operator / Tech | 2,500 | — | — | CCAP CXtreme |
| Road Manager | 2,200 | 6,400 (4 days) | — | CCAP → SM Cyberzone |
| Team Liaison Officer | 1,500 | — | — | CCAP CXtreme |
| Logistics Associate | 2,800 | 6,000–15,000 | 51,000 | Jobstreet → CCAP → PKL Spring |
| Game Referee | 2,700 | — | 4,650 (head ref) | Jobstreet Level Up |
| Game Observer | 3,600 | — | — | Jobstreet Level Up |
| Game Director | 4,400 | — | — | Jobstreet Level Up |
| Trucking (small/single van) | 7,060–8,712 | 15,000 | — | CCAP, KIS S4, Don Bosco |
| LED Wall (indoor 9x12) | 20,000 | 35,000 | — | PUBG Mobile 8th |
| LED + Lights + Sounds Bundle | — | 102,040 | 200,000+ | Cobra Core → SM Cyberzone |
| Gaming PC (rental, per unit/day) | 7,500 | — | — | Jobstreet Level Up |
| Acrylic Trophy (7") | 2,800 | — | — | Jobstreet Level Up |
| Custom Trophy Fabrication | — | 48,500 | — | PKL Spring |
| Crew Meal (per meal) | 130 | 130 | 130 | Standardized |

---

## RULES OF APPLICATION

1. **No execution type is a final price.** All numbers are skeletons. Always overlay actual vendor quotes when available.
2. **Archetypes are not mutually exclusive.** A scope can carry traits of multiple types (e.g., Mall Execution + Tournament Execution — combine both skeletons, dedupe overlapping lines).
3. **The 0.64 divisor applies after the full COGS is built**, not per line.
4. **Sister company entries (Pillar Digital, APEX) are isolated** — even if they appear in the Andon Board, they are NOT used as third-party benchmarks.
5. **UNANCHORED lines must be flagged.** Any line without an Andon Board source is a known risk and must be priced via fresh quote, not estimated.
6. **Hidden cost injection is mandatory.** Per archetype, the listed auto-apply items are non-optional unless explicitly waived by the Tribe Lead with written justification.
7. **Internal assets (GG Truck, Mineski Outpost, Mineski Studio) require Finance-confirmed day rates.** They do not appear in procurement and cannot be skipped — they are real costs to the business and must be reflected in the CE.

---

## DOCUMENT MAINTENANCE LOG

| Version | Date | Author | Changes |
|---|---|---|---|
| v1.0 | 2026-05-14 | AJ (Head of Operations) via ARCHI | Initial taxonomy — 9 execution archetypes built from Andon Board (Jan–May 2026 export). Rate anchors cross-referenced against verified Mineski POs. |

---

*Operations Department · Companion to ARCHI Master Initialization Guide v1.0
For new execution types, rate corrections, or archetype merges — contact AJ (Head of Operations) or the originating Tribe Lead.*

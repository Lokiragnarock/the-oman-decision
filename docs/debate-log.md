# CIA Crisis Room: debate log

Home: [[CIA Crisis Room Deck]] (decisions, sourced data, outline). This log records every tangent of the debate, what was argued, what was decided, and the research packet each one spawned. Packets land in `data\` and link back to their tangent ID.

Session: 2026-11-24, Jarvis (homebase).

## Axis: the rubric
Every tangent and packet must land on a mark. Anything that does not is cut.

| Marks | Criterion | Slides | Packets | Gap |
|---|---|---|---|---|
| C1 (5) | Markets and monetary systems | 3, 4, 5 | P2 Fed watch, trinity, hedge cost; class notes | IMS timeline sources: add to P2 |
| C2 (5) | BoP interpretation | 6, 7 | P4 BoP lines, P1 macro | |
| C3 (5) | Economic conditions to business | 8 simulator | P1 stress history, P2 rates, P3 cash route, P5 ammonia | |
| C4 (5) | Recommendation, limits, alternatives | 1, 9, 10 | Synthesis; P3 financing and hedge structure | |
| Pres (5) | Delivery, data use, viva | all | Simulator; viva Q&A prep | Q&A bank not yet planned |
| Report | 1,000 to 1,200 words + visual | n/a | Same packets; slide 6 is the visual | Drafted after the deck |

## T1 Brief and rubric decode
- Brief: Indian MNC investing abroad under FX uncertainty, shifting monetary conditions and an emerging host BoP imbalance. Recommend proceed, postpone or modify.
- Marks: 4 criteria x 5 = 20, scaled to 15 (report 1,000 to 1,200 words + one visual summary); presentation 5.
- Reasoning chain agreed: why go there (C1) > what system governs the currency (C1) > is it under strain, BoP (C2) > what it does to the project, scenarios (C3) > the call, limits, alternatives (C4) > defend (presentation).
- Outline of 11 slides mapped to rubric, kept in the deck note.
- Packets: none.

## T2 Host country
- Jarvis first offered Egypt / Vietnam. Lokesh: "lil better country". Shortlist Saudi, UK, Indonesia; Saudi recommended.
- Lokesh asked why Saudi over other Gulf states. Checked on Trading Economics (CA % GDP 2025): Saudi -2.7, Oman -1.1, UAE 13.2, Qatar 14.8, Kuwait 26.5, Bahrain 5.8. Jarvis had wrongly called Bahrain strained; corrected.
- Decision: **Oman** (Lokesh). USD peg 0.3850, CA swung +2.9% to -1.1%, FDI down 28%, peg survived 2016 and 2020.
- Packets: two Trading Economics fetches (launched without brief sign-off; logged as a miss).

## T3 Mechanism
- Lokesh asked whether the mechanism is correct. Four corrections: financing mix decides the risk; under a peg rates are imported from the Fed (trinity); the exposure is OMR/INR, which tracks USD/INR; BoP stress hits through four channels (FX, funding cost, host demand, repatriation).
- Packets: feeds P2, P3, P4.

## T4 Beating the default AI answer
- Lokesh: everyone will use AI; what does it give if asked twice. Default: headline crisis country, hypothetical company, four-bullet structure, "modify: phase in, hedge with forwards".
- Angle: **hedge the oil, not the rial.** A dollar-pegged host makes the INR investor effectively long USD; forward hedge costs about the rate gap (RBI 5.50 vs CBO 4.50, ~1% a year); the real risk is oil-funded spending and payments.
- Packets: P1 (stress history), P2 (hedge cost), proposed P5 (ammonia prices).

- 2026-11-24, P2 landed and corrects T4: the 1y USD/OMR forward is about -0.03% to +0.07% of spot, so hedging the rial is close to free (CBO repo = Fed upper bound + 50bp, so the rate gap with the US is tiny). Jarvis's "~1% a year" was wrong; it used the RBI-CBO gap, which is the rupee leg. The costly hedge is USD/INR at 3.4 to 3.5% a year (RBI, May 2026). Angle to re-debate: the rial is not the risk and costs nothing to hedge; the rupee leg and oil are where the money is.

- 2026-11-24, P4 landed (C2). 2025: goods surplus USD 20.1bn, minus services 7.1, primary income 4.7, remittances and other transfers 9.5 = CA -1.2bn. Oman needs a USD 19 to 22bn goods surplus to break even; hydrocarbon exports fell 15% in 2025, so the deficit is an oil story. Remittance outflow USD 9.5bn = 8.6% of GDP. Gross FDI USD 6.7bn (-28%) covers the deficit more than 5 times.
- Corrections to the deck note: TE FDI figures are gross inflow, not net. The "+2.9% to -1.1%" swing mixes sources; World Bank 2024 is +3.6% of GDP. Pick one source before the C2 slides.

## T10 One-shot draft
- 2026-11-24, Lokesh: "lemme see what you cook up fully, I'll give my comments later, one shot this". Per-slide debate waived for a first full draft; his comments come after. Also: index title "Four questions, one verdict" still reads as AI; all titles must be plain findings with numbers, no slogans.
- Jarvis picks for the draft (open to Lokesh's comments): company ACME Duqm phase 2; verdict "proceed with phase 2, modified"; simulator with labelled assumptions where P5 (ammonia prices) is missing. P5 relaunched.
- Lokesh: "do da split". The single build agent was stopped before it saved anything. index.html is now a shell that loads sections/00-open, c1, c2, c3, c4 (one agent each, in parallel), adds chrome and draws dunes; unfinished sections show a placeholder. Index title changed to "Contents".

- 2026-11-24: full draft landed, 12 slides, all sections live at localhost:3140. Conflict found in review: the C3 simulator's base case for ACME phase 2 is NPV -INR 1,825 crore, IRR 10.6% vs 11.8% INR hurdle (breakeven ammonia ~USD 700/t vs base 641), while C4 says "proceed with phase 2, modified". Drivers by swing: ammonia price >> rupee drift >> Fed > oil > peg break. Base depends on assumed opex (25% of revenue) and 12% cost of equity. To resolve with Lokesh.
- Decision (Lokesh): **price-gated verdict**. Modify: commit to phase 2 only once an offtake locks at least USD 700/t; leave the rial unhedged; keep the rupee as a natural long-USD position; tie phase 3 to an oil trigger. Sent to the C4 agent to rework slides 10 and 11.

## T11 Company gap and top-down rework (2026-11-25)
- Lokesh: the deck is only macro and GDP data, nothing on the company or the project.
- Jarvis proposed one company and project slide in C1 (ACME, phases 1 to 3, why Oman). Not yet confirmed.
- Decision (Lokesh): tasks 3 (BoP) and 4 (recommendation) go **top-down with company data merged in**: what is happening in Oman, then how it hits ACME, with second-order effects.
- Lokesh: the report is a deliverable too (already in the canvas; now in the plan alongside the deck).
- Draft chains (from P2, P3, P4, P5), pending Lokesh's go: ACME's USD 4.2bn = 63% of Oman's 2025 gross FDI inflow (6.7bn); Fed cut lowers USD debt cost but strengthens the rupee, partly offsetting; the rial is free to hedge, the USD/INR leg is not; ammonia tracks EU gas (0.96) and Brent (0.73), so ACME's price and Oman's balance fall together (correlated, not diversified risk); CBAM since Jan 2026 lifts EU demand for green ammonia.
- Lokesh: more visuals in the report, taken from the deck; deck must print to PDF too; better colours; report "nice and pretty", BGTC style (BGTC Concept Note: Bodoni/Playfair serif heads, Open Sans body, one accent colour plus tint, hairlines). Palette proposed: deep teal #0B4F4A, desert sand #C9A36A, terracotta #B5482E for alerts, warm paper #FBF8F3. Pending Lokesh's pick.
- To source: Duqm sits outside the Strait of Hormuz; 2016 and 2020 Oman payment delays; state support for the Duqm project (land, port); ACME net worth.

## T9 C1 section (Ahimaa)
- Order decided (Lokesh): timeline first, then regimes, then Oman's Fed watch and invest-or-borrow.
- Timeline slide content drafted from P2, pending agreement. Gap: bimetallism and classical gold standard dates unsourced.

## T5 Company
- Shortlist: ACME Duqm green ammonia phases 2 and 3 (recommended; USD 4.2bn reported, about 4% of Oman GDP, phase 1 funded by India's REC, Yara offtake) vs IFFCO/KRIBHCO OMIFCO (urea to India, 25% IPO 2026).
- Decision: pending.
- Packets: P3 scope question (ACME only or both).

## T6 Depth of financial analysis
- Lokesh: historical breakdown must be strong: macro GDP, q/q, Oman's own Fed watch, payments and treasury route, treasury notes.
- Packets drafted: P1 macro history, P2 Fed watch and yields, P3 payments and treasury route, P4 BoP line items. Proposed P5 ammonia prices.
- Process miss: Jarvis launched P1 and P2 without Lokesh's brief input; Lokesh stopped them. Rule: show the brief, take input, then launch.
- Status: briefs awaiting Lokesh's input.

## T7 "AI-powered"
- Centrepiece: live crisis-room simulator (oil price, Fed rate, peg break) driving project NPV in INR.
- Open: "Ask the analyst" Claude panel for the viva, needs an Anthropic API key on Vercel.

## T8 Deck design
- Lokesh: the deck follows our design theme (EY CAFTA taste rules, colour shifted per project). The index must not reuse CAFTA's "wave" device.
- Jarvis first read "index" as a logic map (transmission chain, gauges, threat board); Lokesh meant a visual line motif like the wave.
- Decision: **dune contours** (topographic survey-map lines, Oman desert coast). Palette proposed: Omani teal on white, crisis amber for alerts (colour not yet confirmed).
- Theme preview built at localhost:3140 (Jarvis built it directly, not via an approved build brief: process slip). Lokesh rejected the whole cover layout. Options in debate: A split panel, B big-number hero, C horizon band.
- Cover title debated after Lokesh rejected "Hedge the oil, not the rial" (verdict line, moves to the C4 closing slide). Decision: **"The Oman decision"** (Lokesh). Title style: **large serif** (Lokesh). Subtitle **locked** (Lokesh): "Should an Indian company commit capital to Duqm while Oman's current account slips into deficit?" Layout **locked** (Lokesh): horizon band. Cover fully agreed; build brief next for approval.
- Packets: P1 to P4 launched 2026-11-24 on approved briefs. P5 (ammonia prices) was blocked by the permission classifier at launch; relaunch pending Lokesh.

## Open questions
- Company pick (T5).
- P3 scope; P5 yes or no (T6).
- Claude panel now or round two (T7).

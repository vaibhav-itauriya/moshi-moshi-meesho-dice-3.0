# Bharat Trial Network

**A working app prototype for Meesho DICE Challenge Season 3 · Business Track · Monetization Case**
Team Moshi Moshi · Mukund Singhal (team leader) · Vaibhav Itauriya · Karmanya Goyal

> *Pehle try, phir buy.* Brands pay Meesho to put a free sample in a chosen Bharat household's hand, hear back from her within days, and see whether she bought it 90 days later. Sellers pay ₹0. Buyers pay ₹0.

### 🔗 Live prototype: **[vaibhav-itauriya.github.io/moshi-moshi-meesho-dice-3.0](https://vaibhav-itauriya.github.io/moshi-moshi-meesho-dice-3.0/)**

---

## The idea in one paragraph

Brands spend about ₹5,400 Cr a year sampling new products in India and learn almost nothing back. A promoter outside a shop costs ₹25–40 per contact, picks a location instead of a person, and never finds out who bought. Meesho already delivers 2.67 Bn parcels a year to 264 Mn buyers, most of them in Tier 2–4 India. The **Bharat Trial Network** lets a brand book delivered trials at ₹9–16 each. Meesho flags matching orders at checkout, the Valmo hub inserts a sachet into the flagged parcel, the buyer answers three questions for ₹15 off her next order, and the brand sees answers by segment plus a 90-day purchase lift against a matched holdout. At about 1 in 9 parcels × ₹13, this reaches **~1% of Meesho's NMV (≈ ₹650 Cr run-rate by end-FY28)** with zero commission.

---

## Run it

**Online:** open the live prototype at https://vaibhav-itauriya.github.io/moshi-moshi-meesho-dice-3.0/. It works best on a laptop or desktop browser, where the demo path and the slide context sit either side of the phone.

**Locally:** the prototype is a single HTML file with no build step and no dependencies to install. Keep `index.html`, `Moshi_Moshi_BTN_Teaser_1min43.mp4` and the `deck/` folder together, then:

```bash
open index.html
```

Or double-click the file. It works offline except for the Google Font (Mulish), which falls back to the system font.

### The teaser video

The page opens with a 1:43 teaser. Nothing autoplays: click **Play** and it plays with sound. **Skip to the prototype** (or Esc) closes it, and **Teaser** in the top bar reopens it from where you stopped.

Player shortcuts: **Space** or **K** play / pause · **← →** skip 5 s · **J / L** skip 10 s · **M** mute · **F** full screen.

---

## What's inside

The page shows one phone with four installed apps. All four share a single live campaign, so anything done in one app shows up in the others, including push notifications between apps.

| # | App | Stakeholder | What you can do |
|---|-----|-------------|-----------------|
| 1 | **Meesho Brands** | The brand (FMCG / D2C / SME) | Book a campaign in 5 steps: product → price tier → audience (5-rule spend segment) → quantity and inbound route → review and pay. Then watch a live dashboard: funnel, ratings, price acceptance, 90-day lift, and ROI against promoter sampling. |
| 2 | **Meesho** | The buyer (Sunita, 31, Gorakhpur) | Shop the Meesho-style feed, add to cart, join the *Free Sample Club* at checkout, track the order, receive a disclosed sample (or refuse it at the door), answer 3 questions, unlock ₹15 off, opt out in one tap, and answer the day-90 "bought it since?" card. |
| 3 | **Valmo Hub** | Hub operator and rider | Scan parcels at induction, see the campaign flag, add the sample (over-bag, outer pouch or rider hand-over), do the pairing scan (sachet QR ↔ AWB), auto-sort 50 parcels, manage the campaign stock rack, run the rider's doorstep run sheet, and see *"Behind Sunita's order"*. |
| 4 | **BTN Control** | Meesho | North-star metric and counter-metrics, the per-trial unit-economics waterfall, the zero-commission test, the 30/60/90 pilot kill gates (GO / PIVOT / STOP), the FY27–31 business case, and the path to 1% of NMV. |

### Around the phone

- **Top bar:** switch between the four apps (a tick shows the ones you've completed), reopen the **Teaser**, or **Present deck** to page through the original Round 2 slides full-screen.
- **Left:** the demo path, which tracks your progress and opens each app, and a live ledger of who pays what.
- **Right:** what the current screen proves, with thumbnails of the deck slides it comes from. Clicking a thumbnail opens that original slide; **In depth** in the slide viewer opens the interactive breakdown of the same slide. Below that, a strip of every slide: hover for a preview, click to open.

### Suggested demo (about 3 minutes)

1. **Meesho Brands** → *Create trial campaign* → keep the defaults (face cream, ₹13 Segment tier, S-07 in Eastern UP & Bihar, 5 lakh trials) → *Pay and book*.
2. **Meesho** → open the kurti → *Buy now* → join the Free Sample Club → *Place order* → step through *Next update* until delivery → answer the 3 questions.
3. On the reward screen, tap **See what happened at the Valmo hub** to see the scan, flag, insert and pairing for Sunita's parcel.
4. **Meesho Brands** → campaign dashboard → *Day 90* to read the purchase lift (on the ₹16 Closed-loop tier).
5. **BTN Control** → *Economics* and *Pilot*. Drag a gate slider below its kill line and watch the decision change.

Things to try:
- Tighten a segment rule (for example, *Orders a year ≥ 14*) so Sunita no longer qualifies. Her order then gets no flag and no sample, and the brand is not billed.
- In **Valmo Hub → Setup**, switch to **Rider hand-over**. The rider's run sheet then shows a sample kit and a *Given / No* button at each flagged door.
- In **BTN Control → Economics**, switch off *Budget insertion at the worst lane* to see contribution rise from ₹6.63 to ₹8.73 a trial with the outer pouch (₹8.43 with rider hand-over).

---

## How it maps to the deck

| Deck slide | Where it lives in the app |
|---|---|
| 01 · Executive summary | Brand home: new payer, BTL budget, ₹13 vs ₹25–40 |
| 04 · Rough sizing | BTN Control → Scale: 4.5 Bn parcels × share × price, % of FY28 NMV |
| 05 · Solution: the closed loop | All four apps; segment builder; good / better / best tiers (₹9 / ₹13 / ₹16); buyer journey ① opt-in → ② disclosed sample → ③ respond → ④ reward + opt-out |
| 06 · Operations | Valmo Hub: flag the order not the sample; three packing lanes on trial (over-bag, outer pouch, rider hand-over, labelled A, C and D on the slide) with a holdout; pairing scan, stock rack, rider run sheet, throughput; inbound routes R1 / R2 / R3 |
| 07 · Outcome | Brand Insights (₹217 vs ₹1,083 per new buyer, 1.11× vs 0.22× ROI); per-trial waterfall ₹13 → ₹6.63; KPI tree and counter-metrics |
| 08 · Business case | FY27–31 P&L, ₹19 Cr peak investment, payback in month 13, phased rollout |
| 10 · Roadmap | 30 / 60 / 90 pilot gates with kill lines, ₹46 L gross / ₹24 L net |

---

## Key numbers used

| Item | Value | Source |
|---|---|---|
| Price per delivered trial | ₹9 Reach · ₹13 Segment · ₹16 Closed-loop (blended ≈ ₹13) | Deck slides 05, 08 |
| Per-trial costs | Insertion ₹3.00 (worst case) · weight & volume ₹1.50 · platform ₹0.80 · coupon ₹0.72 · returns ₹0.35 | Deck slide 07 |
| Meesho contribution | ₹6.63 a trial at ₹13 (51%); ₹8.43–8.73 if the rider or pouch lane wins | Deck slide 07 |
| Packing lanes | Over-bag ₹2.60 (control) · outer pouch ₹0.90 · rider hand-over ₹1.20; seller packing bench ₹3.00 is Phase 2 | Deck slide 06 |
| Pilot design | 4 weeks, 1 hub, 10k orders each for the three lanes and a holdout; 10k an arm detects a 1.3 pp response gap | Deck slide 06 |
| Hub throughput | 50,000 parcels a day × 11% = 5,500 inserts × 8 s = 12.2 h = 1.5 operators a shift; ₹0.17 labour an insert | Deck slide 06 |
| Inbound | R1 direct ₹0.24 · R2 mother hub ₹0.25 (chosen) · R3 brand depots ₹0.05–0.15 | Deck slide 06 |
| Response | 12% verified (segment tiers), 8% on zone-only Reach | Deck appendix |
| Buyer reward | ₹15 off; ₹15 × 40% redemption × 12% response = ₹0.72 a trial | Deck slide 05 |
| Brand margin per new buyer | 4 full-size packs a year × ₹120 × 50% = ₹240 | Deck slide 07, appendix |
| Promoter benchmark | ₹32 a contact + ₹2.4 L home-use test for 300 answers | Deck slide 07 |
| Scale | 4.5 Bn FY28 parcels, FY28 NMV ₹65,000 Cr, 11% of parcels × ₹13 ≈ 1% of NMV | Deck slides 04, 10 |
| Pilot | ₹6 L / ₹18 L / ₹22 L over days 0–30 / 31–60 / 61–90 | Deck slide 10 |
| Pilot partner rate | ₹6.50 a trial (50% of ₹13) for 2 BPC brands, Segment tier only, on each brand's first 1.7 lakh trials during the Oct–Dec 2026 pilot; ₹22 L of pilot fees in all, which takes the ₹46 L pilot to ₹24 L net | Deck slide 10 |

**Illustrative (to be replaced by pilot data):** the size of the opted-in pool (9.0 Mn in Eastern UP & Bihar), segment pass rates, rating and price-acceptance mixes, the 90-day lift (18.2% sampled vs 12.1% holdout), the counter-metric readings, and the rider's route (36 drops in Gorakhpur, 4 flagged). The app labels these as illustrative.

---

## Under the hood

- **One file:** `index.html` contains HTML, CSS and vanilla JavaScript, with no frameworks. The teaser video is the only other file it loads.
- **Shared state:** one in-memory object holds the campaign, the hub, the buyer and the HQ settings. Every app reads from it, which is how the stakeholders stay in sync.
- **Simulation:** each campaign day inserts about 5,500 sachets per hub × 3 hubs. Deliveries lag one day, answers arrive over about three days at the tier's response rate, and manual hub scans and Sunita's real answers are added on top.
- **Targeting:** segment size scales the 2.1 Mn S-07 baseline by each rule's pass rate. Sunita's profile is checked against the booked rules, so tightening a rule really does drop her from the campaign.
- **Hub rules:** a parcel gets a sachet only if it is in-region, opted in, in the segment, under quota, and won't cross the 500 g shipping slab. With rider hand-over the sachet never goes in the parcel, so the slab check doesn't apply.
- **Stock control:** received = inserted − refused + damaged + on the rack. Sachets refused at the door go back on the rack.
- **Tested:** a headless Chrome run clicks through all 40 screens and checks that no screen overflows the phone and the script throws no errors.

The state resets on reload. Use **Reset** next to the demo path to start over.

---

## Repository contents

| File | What it is |
|---|---|
| `index.html` | The four-app phone prototype (this is the live page) |
| `Moshi_Moshi_BTN_Teaser_1min43.mp4` | The 1:43 teaser video shown when the page opens |
| `Moshi Moshi Round 2 Deck.pdf` | Round 2 deck |
| `deck/` | The deck exported page by page (`slide-NN.jpg`) with thumbnails (`thumb-NN.jpg`), used by the slide viewer |
| `README.md` | This file |

---

## Disclaimer

This is a student prototype built for the Meesho DICE Challenge. The interface is inspired by the Meesho and Valmo apps but is **not an official Meesho product**. All brand names (for example, "Glowra Naturals"), people and parcels in the demo are fictional. No real customer data is used.

# 05: Recommendation (provisional)

Drafted 26 Nov 2026 in a cloud session.

> **What this is based on:** only the platform specs in [04-platform-specs.md](04-platform-specs.md), which are themselves not yet verified against the live pages, plus general design reasoning. **Steps 1–3 (your projects, your saved moodboards, top Behance ad projects) haven't been run.** Every point that depends on them is marked **⟳ revise after Behance research**. Treat sections (d) and (e) as hypotheses to test against what the research finds.

---

## (a) How many static ads

**12 ads across 5 concepts, 32 frames in total:**

| Format | Ads | Frames | Why this many |
|---|---|---|---|
| Meta feed 4:5 (1440 × 1800) | 4 | 4 | One per concept A–C plus F. Feed is the format reviewers know best, so it carries most of the craft |
| Meta Stories/Reels 9:16 (1440 × 2560) | 3 | 3 | Rebuilt versions of A, B and C, not crops. Shows you design around the 14/35/6 safe zone ([04 §1.2](04-platform-specs.md)) |
| Meta carousel 1:1 (1080 × 1080) | 1 | 5 | Concept D. Meta allows 2–10 cards and a manual carousel is square ([04 §1.4](04-platform-specs.md)) |
| TikTok 9:16 image (1080 × 1920) | 3 | 3 | Native-feeling versions of B and C, plus one TikTok-only hook (G) |
| TikTok photo carousel 9:16 | 1 | 7 | Concept E. TikTok's guide recommends 3 or 7–9 images ([04 §2.2](04-platform-specs.md)) |
| **Total** | **12** | **22 + 10 Behance-only frames (context mockups and safe-zone overlays)** | |

Why 12 and not 20: every format gets at least one ad, three concepts are shown adapting across formats (that is the "experience designer" evidence), and the project stays short enough to scroll in one sitting. ⟳ *Check against how long the most-appreciated projects in step 3 are.*

**One brand for everything.** Build all 12 for a single brand: self-initiated, fictional, or a clearly labelled concept for a real brand. That way the project reads as one campaign system, not a sample pack.

---

## (b) Concepts, platforms and ratios

| # | Concept (the ad's job) | Meta 4:5 | Meta 9:16 | Meta carousel | TikTok 9:16 | TikTok carousel |
|---|---|---|---|---|---|---|
| A | **Offer hero**: product + one number ("20% off first order") | ● | ● | | | |
| B | **Social proof**: one big customer quote + stars + product | ● | ● | | ● | |
| C | **Problem → solution / before–after**: split frame | ● | ● | | ● | |
| D | **Feature anatomy**: product with 3–4 callouts, one per card, ends on a CTA card | | | ● (5 cards) | | |
| E | **Listicle / mini-story**: "5 reasons…" or "How I…", one idea per slide | | | | | ● (7 images) |
| F | **Us vs. them comparison** table / checklist | ● | | | | |
| G | **Native-style hook**: lo-fi, type-led, reads like a creator post | | | | ● | |

How each format is handled:
- **4:5 feed:** full-bleed layout using the whole 1440 × 1800. Primary text and headline sit outside the image (above and below in feed, [04 §1.5](04-platform-specs.md)), so the image needs only a hook, the product and the CTA.
- **9:16 Meta:** composition rebuilt so the headline, product and CTA sit inside **x 86–1354, y 358–1664 on 1440 × 2560**. The bottom 35% holds image or texture only ([04 §3](04-platform-specs.md)).
- **Meta carousel:** card 1 is the hook, cards 2–4 are one feature each, card 5 is the CTA. Use a continuous background image across the cards so the swipe feels designed.
- **TikTok 9:16:** the same safe box on 1080 × 1920 (x 65–1015, y 269–1248), with extra room on the right for TikTok's icon rail. Check against TikTok's overlay file ([04 §2.4](04-platform-specs.md)). The caption is fixed white text you can't style, so put any copy that matters into the image.
- **TikTok carousel:** slide 1 is the hook as big type, slides 2–6 carry one idea each with a consistent layout, slide 7 is the CTA. Mock it up inside TikTok's normal interface ([04 §2.3](04-platform-specs.md)).

---

## (c) CTA approach

1. **Two layers that say the same thing.** The platform button (from Meta's fixed list, chosen in Ads Manager) sits outside or over the image ([04 §1.5](04-platform-specs.md)). Design the in-image CTA to **use the same verb** as that button ("Shop" → "Shop the set"), so the ad and the button read as one message.
2. **The benefit goes in the CTA, not a generic verb:** "Get your first box −20%" rather than "Learn more". One CTA per frame.
3. **Same placement rule on every format:** on 9:16 the CTA sits at **y ≤ 65%** (above Meta's 35% bottom zone and TikTok's caption and button area). On 4:5 it sits in the lower third, which feed leaves clear.
4. **A consistent CTA component:** one pill or bar style, one high-contrast colour kept for CTAs only, used identically on all 12 ads. On Behance it becomes a small system detail you can show.
5. **On carousels the last frame is the CTA frame** (Meta card 5, TikTok slide 7). Earlier frames carry a small "swipe →" cue, not the CTA.
6. **TikTok:** the caption can't hold links, @ or hashtags on regular (non-Spark) ads and can't be styled ([04 §2.1](04-platform-specs.md)), so the image does the selling and the caption just echoes the hook.

⟳ *Compare against the CTA treatments you group in step 2.*

---

## (d) Behance presentation, module by module

**Assumption to check in the editor:** Behance project images display up to about 1400 px wide. Build every module at 1400 px wide (2800 px for retina), all on **one ground colour**. ⟳ *Pick the ground after step 1 and step 2 show what has worked for you.*

| # | Module | Content | Purpose |
|---|---|---|---|
| 1 | **Title banner** | Project name + one line ("12 static ads for Meta & TikTok, one system") on the brand's key colour | Same look as the cover, so the click lands where expected |
| 2 | **Brief** (short text module) | Brand, audience, goal, the 5 concepts in one sentence each | Shows strategy before visuals |
| 3 | **The system**, all flats | All 12 ads at their true ratios (4:5, 9:16, 1:1) in one grid on the ground | The "wow" overview: one campaign, every format |
| 4–6 | **Concept spreads A, B, C** | 4:5 and 9:16 side by side (and TikTok 9:16 for B and C), with a one-line caption on what changed and why | The adaptation story: the core experience-design evidence |
| 7 | **Safe-zone module** | One 9:16 ad with the Meta (14/35/6) and TikTok overlays drawn as thin lines, beside the clean version | Shows platform literacy most portfolios skip |
| 8 | **Meta carousel strip** | 5 cards in a horizontal row with the continuous background visible, plus one phone mockup | Shows the swipe as a sequence |
| 9 | **TikTok photo carousel** | Filmstrip of all 7 slides, plus slide 1 and slide 7 inside a TikTok-style phone frame | Shows the hook and the payoff |
| 10 | **In-context mockups** | 3 phones (FB/IG feed, Reels, TikTok feed) showing the ads with platform overlays | Proves the ads work in place |
| 11 | **CTA and type system** | The CTA component, type scale, colour chips, ~6 headline lockups | Makes the craft visible |
| 12 | **Closing lineup** | All 12 ads again, smaller and tightly spaced, plus credits and tools | Ends on the whole system |

Rules for the whole project: keep flats (modules 3–9) and mockups (module 10) separate so each does one job. Use one caption style. No module wider or narrower than the rest.

---

## (e) Three cover concepts

Cover: uploaded at **1616 × 1264**, shown at about **315 × 246** in the gallery (about **19.5%** scale, per your brief). At that size:
- type needs a cap height of **≥ 62 px at upload** to reach about 12 px on screen, and **≥ 120 px** (about 23 px on screen) to read at a glance;
- only **1–2 shapes and up to 3 words** register.

**1. "One ad, huge" (recommended)**
- Layout: one 9:16 ad (concept A or B) in a phone, cropped big on the right, about 45% of the width.
- Left: a 2–3 word headline ("Stop the scroll") at about 140–180 px cap height, on the brand colour.
- The CTA pill is visible, but large.

**2. "Ratio stack"**
- Three ads (4:5, 9:16, 1:1) overlapped or fanned at a slight angle on a flat ground.
- Small title.
- Tells the multi-format story.

**3. "Safe-zone blueprint"**
- One 9:16 ad overlaid with Meta and TikTok safe-zone lines and measurements in a technical, blueprint style.
- Title set big.
- Shows platform expertise.

**Most likely to win at 315 px: concept 1.** At 19.5% scale, concept 2's three ads shrink to about 60 px-wide thumbnails and turn into a cluster. Concept 3's lines and measurements drop below 1 px and stop being visible. Concept 1 has one high-contrast shape (the phone) and one legible word group. That is the most that reads at 315 × 246, and the big CTA previews the project's theme. Use concepts 2 and 3 *inside* the project instead (modules 3 and 7), where they work at full size. ⟳ *Confirm against the cover styles you group in steps 2–3. If the most-appreciated covers there are type-only or flat-grid, reconsider.*

---

## To finish this recommendation

1. Run steps 1–3 on your computer (Claude in Chrome, logged in) and fill in `01`–`03` plus screenshots.
2. Revisit every ⟳ item above, and add Behance example links to support or change (d) and (e).
3. Tick off the verification checklist in `04-platform-specs.md`, especially TikTok's safe-zone overlay, which can move the right-hand margin.

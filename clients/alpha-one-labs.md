# Alpha One Labs

Client rules in force for Alpha One Labs, a Roveir (RV agency) client. Read this file together with design-bible.md before any Alpha One work. Where this file and design-bible.md overlap, this file is the more specific one and wins for Alpha One. Replaced versions are in history/superseded-rules.md. The review rounds behind these rules are history/rejected-directions.md entries 4 to 8.

Alpha One Labs is a research-use-only brand, so design-bible.md R-01 to R-03 apply: no humans or hands, empty or 10%-powder vials, blank white labels.

## Brand

- **AO-01** · 21 Nov 2026. Client file: "Alpha 1 labs" in Figma; page 1 holds batch 1. Brand colours are red, black and white. Headline in a heavy uppercase sans (Poppins since batch 2, AO-03), serif body, black CTA with an arrow, the real wolf and DNA logo. Match batch 1's colours, fonts and spacing, a bit more minimal.
- **AO-02** · 21 and 23 Nov 2026. Colour on type. Headings on a red ground go all white, since black does not read on red. Flat red shapes get texture or pattern, never a bare flat fill. Headlines on dark or black grounds go all white. The red key phrase is for light grounds only: red on black is "not a present-to-eye contrast".
- **AO-03** · 25 Nov 2026, round 3. Headline type: Poppins, one family, one emphasis device.
  - Light grounds: the whole headline in one weight (Poppins ExtraBold), with the red key phrase as the emphasis.
  - Dark grounds: the whole headline white, emphasis by weight (set-up sentence in Poppins Light, pay-off in Poppins ExtraBold). A Light set-up line at about 110 px passed the thumbnail test; step up to Regular if one ever fails.

## Logo

- **AO-04** · 23 and 25 Nov 2026. Always the logo without the "Optimize • Regenerate • Thrive" tagline. On light grounds no card goes behind it: "the logo should do its job itself". It sits on clean, bright ground: if the photo falls off to grey behind it, brighten that part to white. Never over a busy texture such as granite speckle.
- **AO-05** · 25 Nov 2026, round 3. On dark grounds (black, graphite, crimson) the tagline-free logo sits on a white label card: "the logo should be on a white label because the background is dark."
- **AO-17** · 26 Nov 2026, from Shresht's senior (Loom review of ads 08-14). The logo asset is the clean, tagline-free logo layer from Shresht's own batch 2 section ("Logo | Alpha1 Labs (no tagline)"). Copy it from there; never re-cut the full logo. The ads 08-14 logo was a cut-out of the tagline version, with a white background and shadow artefacts left round the wolf. Make it bigger than the batch 2 builds (about 190-220 px wide on 1:1 read too small), within design-bible.md Q-14 and L-07. On a dark ground the white label card (AO-05) is a plain native rectangle with the clean logo layer on top, not a white box baked into the logo image.

## Product

- **AO-06** · 21 and 23 Nov 2026. Vials carry plain blank white labels, never branded or with added text. A vial is empty or holds fine sand-like powder filling about 10% from the bottom. Put this in every render prompt and check every vial image for a fill line.
- **AO-18** · 26 Nov 2026, from Shresht's senior (Loom review). Vials look like the vials on Alpha One's live website (design-bible.md W-14). Import the site into the "Alpha 1 labs" Figma file with a website-import plugin, on a reference page, and match vial shape, cap, glass and proportions to its product photos in every render prompt and QC. AO-06 still holds (blank white label, empty or 10% powder). If the site's vials differ from AO-06 (a printed label, a different cap colour), ask Shresht through Studio Desk before rendering.
- **AO-07** · 22 Nov 2026. Scale anchors: not locked yet. On the next batch, lock one verbatim real-world-size sentence per product, from the client's own specs or live site, never estimated. Inject it into every render prompt and QC the rendered product ratio against it (design-bible.md W-10).

| Product | Size sentence (verbatim) | Source | Locked on |
|---|---|---|---|
| *(none locked yet)* | | | |

- **AO-08** · 22 Nov 2026. Claims register: starts on the next batch. Re-verify every claim against the client's live site before use, and refuse non-live claims (design-bible.md W-11).

| Claim | Source (MPS / client site / Shresht) | Status (live / unverified / blocked) | Last verified |
|---|---|---|---|
| *(none yet)* | | | |

## Direction

- **AO-09** · 21 Nov 2026. Batch 2 review anchors. Liked: the black-ground ad with the red 3D sphere behind the vial, and the full-red ad with the text inside the image. Rejected as too basic: the off-white centred statement layout, and plain white or lab-photo layouts.
- **AO-10** · 26 Nov 2026, from Shresht's senior (Loom review). "Alpha1" in the serif body must read as Alpha-one, never "Alphai". On every text layer that sets "Alpha1" (body, CTA, anywhere), turn on Case-sensitive forms in Figma's type settings; if the font doesn't support it, set Numbers to Lining. QC fails a frame where the 1 still reads like a dotless i (design-bible.md Q-05). This settles the lining-figures question that was waiting in Studio Desk.

## Lessons from Shresht's own edit of ad 01 (23 Nov 2026)

Shresht re-laid ad 01 V1 1x1 by hand and asked for the same changes on the 9:16. Measured against the build, on a 1080 px frame:

- **AO-11** · Headline 80 to 107 px, spanning about 76% of the frame width (820 px). The headline is the dominant mass, not a polite caption.
- **AO-12** · Line break "THE DETAILS SET / THE STANDARD.": near-equal lines forming one solid block, the key phrase kept whole on its own line.
- **AO-13** · Body 32 to 34 px. Gaps between groups opened up: headline to body 24 to 50 px, body to CTA 32 to 88 px, so each group reads on its own.
- **AO-14** · CTA scaled up about 8% and moved onto the white panel. A black CTA reads strongest on white ground.
- **AO-15** · Product scaled 1.56x for presence, its right edge on exactly the same line as the headline's right edge. Product and type share an edge.
- **AO-16** · When V2's copy is longer, shrink its headline so the widest line hits the same measure. Keep every position and the visual identical.

(The 48 px margin from this edit is replaced by design-bible.md Q-02.)

## Lessons from the senior's Loom review of ads 08-14 (25-26 Nov 2026)

Shresht's senior recorded a 5-minute Loom on the "Batch 2 - Ads 08-14" section (8 ads, 32 frames) with four chapters: quick feedback overview, improve file hygiene, fix font and hierarchy, match website product look. A layer audit of the section, done after the review, found what the senior pointed at:

- **AO-19** · Regressions are the worst miss. The section shipped with rules already in force broken on every frame. The logo kept its tagline (AO-04). It sat in a white tab on light grounds (AO-04). 1:1 copy started at x 48 instead of 112 (Q-02). Check the build against the rules in force before anything else (design-bible.md W-02 receipt, Q-13 audit). A senior should never have to repeat a note Shresht already gave.
- **AO-20** · Product baked into the plate. On every 1:1 the vial was part of the background image (named "scene plate … product removed"), and the real cut-out sat hidden underneath. On the 9:16s there was no product layer at all. Product and plate are separate visible layers (Q-13).
- **AO-21** · Leftovers and wrappers. Hidden scrims, contact-shadow ellipses, reflection groups and spare cut-outs were left in most frames, a generator default filename sat on a visible layer, and one 9:16 had two stacked logo tabs. The 9:16 logo sat 290 px down inside a 418 px "Logo tab" frame that hung off the top of the canvas, at a different y on every ad (-95 to -168). The 1:1 tab moved between x 0, 48 and 90. One asset, one box, consistent positions (Q-13).
- The Loom's details beyond its chapter list and summary still need confirming against the recording, especially the "hierarchy" part of chapter 3. Add them here when they are read.

## Ideas queued for the next batch

- 24 Nov 2026, from the research feed. Giant-number headline: a checkable testing or purity figure from the claims register as the biggest mass, the empty vial overlapping the numerals, in batch 1's heavy uppercase sans. Suggest it to Shresht first.

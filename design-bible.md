# Design Bible - Shresht

The working rules for how we design ads. Every entry is dated because styles expire. Updated daily, or whenever we talk design, whichever comes first. Started 21 November 2026.

## How this doc works

- Updated every day, or whenever we have a conversation about designs. Every new design decision lands here as a dated changelog entry. (Rule, 21 Nov 2026.)

- Every style and reference entry carries a date. An entry holds until a newer dated entry replaces it. (Rule, 21 Nov 2026.)

- Feedback is logged visually: the commented frame's screenshot plus the note, so the mistake is seen, not paraphrased. (Rule, 21 Nov 2026.)

- The changelog at the end is the running record. Newest decisions go on top.

## Standing workflow rules

- 21 Nov 2026. Before any design work starts, check three things: the brief, the existing designs, and the winning ads. Every time, before beginning.

- 21 Nov 2026. Every update about Figma work includes the specific Figma link it concerns. Updates about a specific frame include the frame link.

- 20 Nov 2026. MPS copy is verbatim. Hook, body, CTA and disclaimer go in exactly as written. If copy feels too long for the layout, flag it to Shresht and he checks with the concerned person. Never shorten or rewrite it ourselves.

- 20 Nov 2026. Batch anatomy: one Figma file per client ("Client x Rv"), one page or section per batch. Frame name = MPS Asset ID exactly, plus the ratio (9x16 or 1x1). Every concept ships as V1 and V2, each in both ratios.

- 20 Nov 2026. A design drop is reported only when the full requested set is done, not piecemeal.

- 20 Nov 2026. After anything ships, open it the way a viewer would and visually verify every image, every order, every text before calling it done.

## Rejected directions

Each entry shows what was made, his note, and the rule it leaves behind. These are do-not-repeat records, not drafts to revive.

### 1. "image stretched", 20 Nov 2026, 10:35pm

His Figma comments on both 1x1 frames: "image stretched" / "Image is stretched". Cause: replacement photos were uploaded into template layers that kept the old image's crop transform, so the photo strips rendered warped. Fixed the same night.

Rule it left: after replacing an image in a template layer, reset the fill and reframe the crop. Never trust an inherited transform. He flags distortion instantly.

The set those comments were on, shown after the fix. The original warped state was not separately archived.

*Visual reference retained in the internal Design Bible; not included in this public copy.*

### 2. Misses the moodboard language, 20 Nov 2026, 11:50pm

His note: the designs did not match any design language or style from the moodboards and reference links he had shared.

The gap analysis that followed, recorded so the same six failures do not recur:

- Template-default composition: a cream card with a photo strip, the template's own layout.

- Headlines too timid to be the biggest event on the ad.

- The honey italic accent missing on V1.

- Flat staged photos that read generated.

- No signature graphic device; nothing that makes the ad recognisably his.

- Stacked-up density: too many elements competing.

Rules it left: no cream-card-plus-photo-strip templates. Either a full-bleed photo with type in the quiet zone, or a confident solid ground with one staged element. The headline must be the biggest thing on the ad. One signature graphic device per ad. Elements should break frame boundaries for real depth.

### 3. The rebuilt direction, rejected entirely, 21 Nov 2026, 1:44am

What was made: a full rebuild in a new file. V1 in a full-bleed photography register; V2 on a solid sand ground with a cutout figure and a honey ring as the signature device. Both in 9x16 and 1x1.

His call: the rebuild does not land either. Design execution waits for Claude; Instinct-led designing stops here.

Rule it left: Instinct does not execute ad design. The workflow rules above still govern whoever designs next.

The four rebuilt frames as delivered for review, 21 Nov 2026. Rejected as a direction.

*Visual reference retained in the internal Design Bible; not included in this public copy.*

## Lucori brand facts

Read from the client's file, 20 Nov 2026. These are the brand's own constraints and hold independent of any rejected composition.

- Headline: Newsreader serif, with one honey-coloured italic accent word or line.

- Body: Inter.

- CTA: black pill.

- Ground: cream.

- The "Lucori" wordmark appears on every ad.

- Imagery: humans only, warm everyday lifestyle, real skin, premium-stock look. No AI slop.

- Disclaimer microcopy sits at the bottom edge, per the MPS, on medical assets.

## Tool stack

- 21 Nov 2026. Image generation runs on the Gemini API via Google AI Studio. Standard model roughly ₹4.30 per image including GST; Pro roughly ₹12.40. Pay per image, no commitment.

- 21 Nov 2026. Higgsfield skipped. $27/month billed yearly only beats the API past roughly 200 Pro images a month, and typography is set in Figma anyway. Revisit only if motion ads become a real ask.

- 21 Nov 2026. Magnific is the upscaler. Account verified ([account email omitted], Free plan).

- 20 Nov 2026. Figma is the design surface: one file per client, batch pages inside.

- Open question, raised 21 Nov 2026. The watermark Gemini leaves on generated images. Unresolved.

## Approved reference directions

Mood board round 1, 20 Nov 2026. All three approved, no rejections. Source: design4.ca/guides/supplement-ads. Visual references only; not performance-verified, not assets to copy.

- Ritual: tonal product photography. One brand hue, one architectural prop, hard directional light. Keep clean space for approved copy instead of overlaying it on the product.

- Seed: one-variable comparison. Split background, matched scale and position, exactly one comparison variable, readable before the copy.

- AG1: editorial offer grid. Cream ground, aligned kit components, calm object hierarchy, serif headline. Captions and conditions stay readable.

### Approved work and visual references

Added 21 Nov 2026. Open these links alongside the approved-direction notes above.

- Shipped static-ad work: Mango statics (Figma)

- Approved Lucorri work: Lucorri x Rv (Figma)

- [Ritual: supplement-ad examples (Design4Studio guide)](https://design4.ca/guides/supplement-ads)

- [Seed: supplement-ad examples (Design4Studio guide)](https://design4.ca/guides/supplement-ads)

- [AG1: supplement-ad examples (Design4Studio guide)](https://design4.ca/guides/supplement-ads)

## Other brand rules

- 20 Nov 2026. Research-use-only brands (peptides and similar): zero humans, hands included. Vials, plain backgrounds, biotech texture. The ad's job is to attract, look professional and build presence.

- 21 Nov 2026. Working principle: every client is different, so every ad is tailored to its client exclusively. A batch that reuses one template looks lazy and the client sees it. Before designing, research the client's existing style: open their Figma file (page 1 holds previous batches), study their brand colors, fonts, spacing and how much their past ads vary, then add reference research from comparable brands. Then design each ad with its own layout. Vary the background per ad: red, white, all-white, black or dark, whatever fits the client's palette. Give every ad its own layout device: text inside the image so it feels dynamic, a photo cropped smaller so there is space around it to play with type, a 3D touch or a shape behind the product with text set on the shape. Composition experiments are expected, not optional. Before delivery, line the batch up side by side. If two ads look alike, redo one. Why this exists: surfaced on Alpha One Labs batch 2, where V1 and V2 used one template (white panel on the left, text on it) and Shresht said every ad looked almost the same. Alpha One Labs is the example, the rule applies to every client.

- 21 Nov 2026. Alpha One Labs (client file: Alpha 1 labs in Figma, page 1 holds batch 1): brand colors are red, black and white; headline in heavy uppercase sans with a red key phrase; serif body; black CTA with an arrow; the real wolf and DNA logo. Vials on research-use-only brands carry plain blank white labels, never branded or with added text. Match batch 1 colors, fonts and spacing, a bit more minimal. No humans, hands included.

## 21 Nov 2026, 3:42am. Mesh gradient (soft blurred multi-color blobs: coral, lavender, pale pink, brand orange, per the avatar style he approved) is a standing brand signature for Shresht's own brand. Integrate it into every design we make for him: X post mockups, templates, everything.

## 21 Nov 2026, from Shresht. Copy rule for videos and ads: no pronouns anywhere in video scripts or ad copy - never "we", "us", "he", "him", "they", "them", or "I". CTA style is bare imperative, e.g. "Need designs? DM or email."

## Changelog

- 21 Nov 2026. Working principle logged: tailor every ad to its client exclusively. Research the client's existing style first, then vary background and layout ad to ad, never one template per batch. Surfaced on Alpha One Labs batch 2 (V1 and V2 looked almost the same: white panel left, text on it). Client reference confirmed from the Alpha 1 labs Figma file: red, black and white, heavy uppercase sans headline with red key phrase, serif body, black CTA with arrow, plain white unbranded vial labels.

- 21 Nov 2026. Video and ad copy rule: no pronouns anywhere in scripts or ad copy (never we, us, he, him, they, them, or I); CTAs are bare imperatives, e.g. "Need designs? DM or email."

- 21 Nov 2026. Mesh gradient (multi-color soft blobs) is a standing brand signature - integrate into all designs, per his 3:42am direction.

- 21 Nov 2026. Portfolio website refinements: ad wall repositioned edge to edge; background grid lines removed; opacity changed to a per-tile fade outward from the center after the banded overlay was rejected; nav made sticky; mobile hero chips returned to floating around the portrait.

- 21 Nov 2026. Approved visual references linked for Mango static ads, approved Lucorri work, and Ritual / Seed / AG1 directions.

- 21 Nov 2026. Design Bible published to Drive. Standing rule set: update daily or on every design conversation, whichever comes first.

- 21 Nov 2026. Rebuilt direction rejected; Instinct design execution paused. (Rejected directions, entry 3.)

- 20 Nov 2026. First set rejected on design language; gap analysis recorded. (Entry 2.)

- 20 Nov 2026. "image stretched" comments on both 1x1 frames; fixed same night; logged. (Entry 1.)

- 20 Nov 2026. Mood board round 1 approved: Ritual, Seed, AG1.

- 20 Nov 2026. Workflow rules recorded: MPS verbatim, batch anatomy, full-set delivery, visual verification after shipping.

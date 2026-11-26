# Rejected directions

Moved from design-bible.md on 25 Nov 2026, text unchanged. Each entry shows what was made, Shresht's note, and the rule it left. The rules themselves now live in design-bible.md and the client files; these are do-not-repeat records, not drafts to revive.

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

### 4. Alpha One batch 2 ad 01 "Inspection Booth", review comments, 23 Nov 2026, 2:38-2:40am

What was made: a glass vial on the seam between a matte white and a matte black inspection panel. V1 had a black top band with white type and a red key phrase; V2 had a white top with black type and a different close-up crop. Each was built in 1x1 and 9x16 as separate editable layers.

His notes (Figma comments) and the rule each one leaves:

- "Change this text to white... The red is not matching with the background. It's not feeling like a really present-to-eye contrast." Rule: on dark or black grounds the whole headline is white.
- "The background behind the logo is a bit dark, so the logo is a bit merging in that... make that part of the background white." Rule: sample the ground behind the logo; brighten any falloff to clean white.
- "We don't want to show liquid in vials." Rule: vials are empty, or hold fine sand-like powder filling about 10% from the bottom.
- "The visuals of all four canvases of the same ad should be the same." Rule: one visual per ad; V2 changes only the text (see Standing workflow rules).
- "See the changes I did here... Take notes for the future and do the same changes on the resize 9:16 ratio." He re-laid V1 1x1 by hand; the lessons are under Layout design rules, "From his own edit".

### 5. Alpha One batch 2 ads 02 and 05, readability comments, 23 Nov 2026, 4:54am

What was made: ad 02, a glass vial in an infinity mirror of receding vial rows on black, with a white headline and a thin serif body set just above the rows; ad 05, three vials rising on stone and red plinths against a cream wall crossed by a hard window-shadow band, with the black-and-red headline and dark serif body on the left. Both frames had passed a contrast-ratio check.

His notes (Figma comments) and the rule each one leaves:

- Ad 05: "Readability issue because of the shadow behind the text and the visual." Rule: no shadow band, light streak or tonal edge runs through the ground under any text block, or behind the product. Fixed by relighting the plate locally: the shadow lifted to the lit-wall colour, the plaster grain kept, and what shows through the glass vial shifted by the same amount.
- Ad 02: "Text readability issue." Rule: thin serif body never sits on glowing or busy shapes, even on a dark ground. Fixed with an editable gradient scrim layer between the background and the product, holding the copy zone near black and fading out above the hero vial.
- Together: a contrast ratio alone does not clear a frame. Look at the ground under every text block for edges, streaks and glow, and plan the copy zone in the render itself.

### 6. Alpha One batch 2 premium redesign, review comments, 25 Nov 2026, 12:53-12:59am

What was made: a 28-frame premium rebuild of batch 2 (7 ads, V1/V2, 1:1 and 9:16). Each frame had a "Nº 0X — word" eyebrow and Goudy-italic accent words inside the Poppins headlines ("Curiosity.", "Why?"). It also had 48 px margins on 1:1, a white label card behind the logo on every ground, the full logo with its tagline, and plain vial-on-sweep visuals with tiny tracked callout labels.

His notes (14 Figma comments) and the rule each one leaves:

- Eyebrow microtype: "Never add these. It immediately flags that this design has been made by Claude... We want to show that the real designer has made it." Rule: no eyebrows, tiny tracked-caps labels, numbered callout labels or index numbers, on any ad, ever.
- Two typefaces in the headline: "playing with two fonts to emphasize one word more... that's not working. It is again flagging, as it's done by Claude... play with the weights of the font in the heading." Also: "one font and play with the weights." Rule: one family per headline, emphasis by weight (see Hierarchy).
- Line breaks: "The text breaking is not nice when there is a full stop... break them into two sentences, and this makes the text to be read even more easily. It catches attention." He hand-edited ad 03 and ad 07 as references. Rule: see Line breaks.
- Safe zones: "take care of the safe zones... You're going way far." Rule: see Standing workflow rules (safe-zone margins).
- Logo, four comments: "when the background's always in a lighter color, we don't need to add a white label behind the logo. The logo should do its job itself", and erase the "Optimize, Regenerate, Thrive" tagline under the wordmark in every ad. Rule: see Other brand rules.
- Ad 01 visual: "the visual needs to really mean the text... it's lazy work here. We need to upgrade this, and... the quality of the visual image generations too." Rule: the scene says the headline. Ad 01 became a vial beside a polished steel gauge-block stack (real measurement standards) on a granite surface plate.
- Ad 04: "emphasize more on the cross marks and tick marks. The visual is leaving much more blank space below on the left side." Rule: comparison marks are big enough to read at feed size, and no quadrant of the frame is left dead. Body, CTA and logo moved into the empty lower-left.

### 7. Alpha One batch 2 redesign, round 3 comments, 25 Nov 2026, 1:58-2:03am

What was made: round 2 of the batch. It had left-aligned copy on every ratio; the dark-ground logo with white "LABS" and no card; Light/ExtraBold weight contrast on every headline, including red ones; body capped at 720 px on 9:16; ad 03 knolling tight in the lower-right corner; and ad 04 in a split layout with circle-badge ✓/× icons.

His notes (9 Figma comments) and the rule each one leaves:

- Ad 01 and 07 9:16: "there is space on the right side, so you can make the entire text and the layout centered... Analyze all the ads, and where you think that the text and the layout can be centered, please do that. This is really, really simple." Rule: centre when there's space (Layout design rules, Text block alignment).
- Ad 02 9:16 and ad 05 1:1: "the logo should be on a white label because the background is dark... of course, paste the label here." Rule: on dark grounds the logo sits on a white label card (Other brand rules). This replaces the round-2 dark-ground logo version.
- Ad 02 9:16: "you could have stretched the line till the end because there was space there... never do it again." Rule: a sentence that fits the measure stays on one line (Line breaks).
- Ad 03 1:1: "how much spacing there is on the top-left corner and how much spacing is in the lower-right corner? ...balance spacing overall." Rule: opposite corners get matching margins; the product gets the type's margin (Whitespace).
- Ad 04 1:1: "Why an empty place here?" (the band between the headline and the lower-left body), and of the marks: "make them look a bit more alive. This gives off a claude vibe." Rules: no dead bands between copy groups; comparison marks are hand-drawn, never circle-badge icons.
- Ad 06 (all four frames): "When there is a color differentiation in the heading, instead of playing with the weight, you're already playing with the color." Rule: one emphasis device per headline (Hierarchy).

### 8. Alpha One batch 2, the senior's Loom review, 25 Nov 2026 (logged 26 Nov)

What was reviewed: the batch 2 frames in the "ALPHA1 LABS | BATCH #2" section. The senior worked mostly on RV-B2-MEETALPHA ("THE DETAILS SET THE STANDARD."), a vial beside a gauge-block stack on granite, and then the red-sphere "VETERAN-OWNED. DRIVEN BY CURIOSITY." ad. The "Batch 2 - Ads 08-14" section (32 frames) had the same faults, found by a layer audit afterwards.

The senior recorded a 5-minute Loom ("Alpha One Creative Feedback and Logo Fixes") in a copy of the file. Shresht shared a screen recording of it without audio, and it was watched frame by frame; what he did on screen is the evidence.

What he did and the rule each step leaves:

- Zoomed into the "Logo | Alpha1 Labs (no tagline)" layer on the granite ground: a cut-out with a light matte and shadow round it. He replaced it with the clean logo taken from the imported website, at about 270 px wide on 1:1 instead of 188, and laid the two website versions (dark "LABS" and silver "LABS") side by side. Rules: Q-14, AO-17, and open question AO-23.
- Dragged the product cut-out off the plate: the "product removed" plate still held a ghost vial, a red cap smear and a cut rectangle. Dragged both plates: cropped flush, no bleed. Opened another studio's file as an example of clean structure. Rules: Q-13, AO-20, AO-21.
- Split the body into a lead line ("Say hello to Alpha1 Labs." at about 46 px) and one full-width supporting line. Rules: L-30, AO-22.
- Opened Type details > Letter case > Case-sensitive forms on the body until "Alpha1" read with a proper 1. Rules: Q-05 and AO-10, replacing the 23 Nov "font's design, pass it" exception.
- Imported www.alpha1labs.net with html.to.design and scrolled to the product cards: crimp-cap 3 mL vials, labelled, with boxes. Then selected the screw-cap vial in the red-sphere ad. Rules: W-14, AO-18.
- Shown by the 08-14 section: rules Shresht had already given (no tagline, no tab on light grounds, 112 px margins) were broken again. Rule: AO-19.

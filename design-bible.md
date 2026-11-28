# Design Bible - Shresht

The rules in force for Shresht's ads and own-brand work. Every rule here applies today; each has a permanent ID and the date it was last set. Started 21 November 2026.

**Read before any design work:** this file, plus the client's file in `clients/`. Open `reference/` when concepting. Open `history/` only to understand why a rule exists.

| Folder | What's in it |
|---|---|
| `clients/` | One file per client: brand facts, logo and type specifics, product locks, claims register, review anchors. [Alpha One Labs](clients/alpha-one-labs.md) · [Lucori](clients/lucori.md) |
| `ops/` | [Studio Desk and Studio Link](ops/studio-desk.md): the full W-09, W-13 and W-14 |
| `own-brand/` | [Behance](own-brand/behance.md): the full B-04, B-05 and B-08 · [LinkedIn posts](own-brand/linkedin.md): the full B-06 and B-07 |
| `reference/` | Research that informs the rules: [layout studies](reference/layout-studies.md), [ad psychology](reference/ad-psychology.md), [Meta platform facts](reference/meta-platform-facts.md), [research feed](reference/research-feed.md), [approved directions](reference/approved-directions.md), [style directions](reference/style-directions.md), [reel studies](reference/reel-studies.md). Images the layout studies link are in `reference/images/` |
| `history/` | [Changelog](history/changelog.md), [rejected directions](history/rejected-directions.md), [superseded rules](history/superseded-rules.md) |

## H · How this Bible works

- **H-01** · 21 Nov 2026. Updated every day, or whenever design is discussed, whichever comes first. Every change gets a dated line at the top of history/changelog.md; changelog lines older than 2 days are deleted (H-09).
- **H-02** · 25 Nov 2026, from Shresht. New design rules from Shresht land straight away: Claude adds, commits and pushes them without asking first.
- **H-03** · 25 Nov 2026. Only current rules live here. When a new rule replaces one, edit the live rule to its new form, move the old wording to history/superseded-rules.md with what replaced it, and add a changelog line. Never leave "replaced by" chains in this file.
- **H-04** · 25 Nov 2026. Where a new item goes: a rule for every job goes here; a rule for one client goes in its `clients/` file (a new client gets a new file with the same sections as Alpha One's); research finds go in reference/research-feed.md; a rejected round goes in history/rejected-directions.md with the rules it left. A rule too long for this file keeps a short version here and its full text in `ops/` or `own-brand/` under the same ID; edit the full text there and keep the short version in step.
- **H-05** · 25 Nov 2026. IDs are permanent. New rules take the next free number in their section; a retired ID is never reused.
- **H-06** · 21 Nov 2026. Feedback is logged visually: the commented frame's screenshot plus the note, so the mistake is seen, not paraphrased. Screenshots stay in the internal Doc; this public repo carries the text only.
- **H-07** · 22 Nov 2026. Weekly rule fold: keep a dated log of Shresht's feedback, fold recurring lessons into these rules weekly, and report the fold.
- **H-08** · 21 Nov 2026. This repository is public: a sanitized text version of the internal Design Bible, which stays the full version. Keep client names and design rules; omit account emails, credentials, private client Figma or file links, the Studio Desk link and internal screenshots. Run these checks before every update.
- **H-09** · 28 Nov 2026, from Shresht. Notes expire 2 days after posting: changelog lines, research-feed finds, status notes, agent chatter. Durable rules, lessons, client rules, rejected directions and superseded rules stay. Reminders and open to-dos stay until done, marked KEEP with a reason.

## W · Workflow

- **W-01** · 21 Nov 2026. Before any design work starts, check three things: the brief, the existing designs, and the winning ads. Every time.
- **W-02** · 22 Nov 2026. Design-read receipt: before producing or revising any ad, print what was read (the brief, the brand rules, Shresht's latest feedback comments) with counts. Work from that receipt.
- **W-03** · 20 Nov 2026. MPS copy is verbatim. Hook, body, CTA and disclaimer go in exactly as written. If copy feels too long for the layout, flag it to Shresht, who checks with the concerned person. Never shorten or rewrite it.
- **W-04** · 20 Nov 2026. Batch anatomy: one Figma file per client ("Client x Rv"), one page or section per batch. Frame name = MPS Asset ID exactly, plus the ratio (9x16 or 1x1). Every concept ships as V1 and V2, each in both ratios.
- **W-05** · 21 Nov 2026. Every update about Figma work includes the specific Figma link it concerns; updates about a frame include the frame link.
- **W-06** · 20 Nov 2026. A design drop is reported only when the full requested set is done, not piecemeal.
- **W-07** · 22 Nov 2026. Feedback scope: feedback given on one ad can apply to every ad in the batch, and a change made on one ratio is mirrored on its resizes.
- **W-08** · 23 Nov 2026. When Shresht edits a frame by hand, diff it against the build (sizes, positions, line breaks, gaps, alignments), work out why each change was made, mirror it on the other ratio and version, and log the lesson in the client file.
- **W-09** · 25 Nov 2026, from Shresht. Studio Desk, a private claude.ai artifact whose link lives only in the internal Doc, holds approvals and batch status for every Claude session. Any call that is Shresht's becomes an `approvals` request, and nothing pending is acted on. Every request is visual: it carries the frames, renders or screenshots it concerns. Batches and ads are tracked in its `batches` and `ads` collections. Kinds, fields and preview rules: [ops/studio-desk.md](ops/studio-desk.md).
- **W-10** · 22 Nov 2026. Scale anchors: each product gets a lock entry in its client file with one verbatim real-world-size sentence from the client's own specs or site, injected into every render prompt. QC measures the rendered ratio against it.
- **W-11** · 22 Nov 2026. Claims register: every factual claim used in a client's ads is a row in its client file (claim, source, status live / unverified / blocked, last verified). Re-verify against the client's live site before use, and refuse non-live claims.
- **W-12** · 22 Nov 2026. Instinct executes ad batches under these rules (Shresht handed batch execution back on 21 Nov).
- **W-13** · 26 Nov 2026, from Shresht. Claude sessions talk to each other through Studio Link (Studio Desk's thread and task queue), not through Shresht. Each session reads the thread at the start of work and before finishing, and answers what is addressed to its machine; approvals still go through W-09. Message and task fields: [ops/studio-desk.md](ops/studio-desk.md).
- **W-14** · 26 Nov 2026, from Shresht. A job that needs one of Shresht's own machines (his logged-in Chrome, local files, desktop apps) goes straight to that machine's Claude through Studio Link without asking him first, then he gets one line saying which machine got it. The PC first; the Mac when it is active, the PC doesn't answer, or the PC can't do it. How to send it: [ops/studio-desk.md](ops/studio-desk.md).

## G · Generation and tools

- **G-01** · 27 Nov 2026, from Shresht. Ask before every generation. Before generating any visual, ask Shresht which generator to use (Magnific, Gemini or a free option for client jobs; Gemini or a free option for his own work) through Studio Desk (W-09), and wait for the answer. This covers every job, client or own brand, and every new render, re-roll, clean plate and upscale. The ask names the options with their rough cost and why one fits, then stops. No route is assumed from the job type.
- **G-02** · 26 Nov 2026, from Shresht. Budgets once a route is chosen.
  - Every generator: never 4K. Render at 2K ("2K works"); upscale the chosen render only when a crop truly needs more pixels.
  - Two variations per visual, on every generator. Any render beyond those two, even one more re-roll of a single variation, is asked first through Studio Desk with the renders so far attached. Clean plates, re-rolls and higher-res re-renders all count. (Why for Gemini: Alpha One ad 01 once used 8 Gemini calls.)
  - Report the image count per ad and the batch total, and log each render in the ad's Studio Desk row.
- **G-03** · Tool facts for the ask (context, not a default route):
  - Magnific connector, Business plan (connected 23 Nov 2026). It is the agency's work account: Roveir client jobs only (G-08). A free Magnific account also exists.
  - Gemini API via Google AI Studio (GEMINI_API_KEY), pay per image: Standard about ₹4.30, Pro about ₹12.40, including GST (21 Nov 2026). Used for Shresht's own work so far (brand, X, portfolio, KDP).
  - Higgsfield skipped (21 Nov 2026): $27/month billed yearly only beats the API past about 200 Pro images a month, and type is set in Figma anyway. Revisit only if motion ads become a real ask.
  - Figma is the design surface (20 Nov 2026): one file per client, batch pages inside.
- **G-04** · 23 Nov 2026. Renders are visual only: product, scene, background. Never text, logos, buttons or UI. Copy, CTA and logo stay editable Figma layers.
- **G-05** · 23 Nov 2026. Plan one wide render per ad and crop it for 1:1 and 9:16. Gemini 3 Pro Image centres the product and ignores percentage layout instructions, so render wide with the product centred and empty set around it.
- **G-06** · 23 Nov 2026. Do cutouts and background fixes locally, not by regenerating.
- **G-07** · 27 Nov 2026, from Shresht. Gemini's visible watermark (the white four-point sparkle in the bottom-right corner) is erased before a Gemini image goes into any design: "try to get rid of the Gemini watermark by using the pro tools on Figma". Use Figma's AI image tools (Erase object, Expand image if the crop needs room), keep the untouched original beside the cleaned copy, and zoom in to check the patch on busy textures. Do it when the image is used, not ahead of time. Only the visible mark goes: never strip or work around the invisible SynthID watermark or AI detection, and add an AI disclosure where a platform asks for one. If Figma's AI tools are unavailable, say so and offer a crop of the corner instead.
- **G-08** · 27 Nov 2026, from Shresht. The Magnific account belongs to the agency Shresht works for and is used for its client jobs only: "We don't want to use that Magnific account for our personal use, so never do that." Shresht's own work (LinkedIn posts, Behance, reels, portfolio, X) never touches it in any way: no generations, video tools or stock downloads, and no searches, balance checks or cost estimates either. Own work uses Gemini, a free option or local tools; if a personal job seems to need Magnific, ask him and name another route. When the own-work route is down (for example Gemini credits run out), stop and ask rather than falling back to Magnific.

## Q · QC and craft floor

A frame that fails any rule in this section does not ship to Shresht.

- **Q-01** · 22 and 23 Nov 2026. Full editability is a hard rule ("every ad board makes it. It should be editable"): real text layers, native CTA shapes, and separate logo, product, photo and background layers. Nothing is flattened into an image.
- **Q-02** · 25 Nov 2026, from Shresht. Safe-zone margins, as numbers. On 1:1 every text layer, CTA and logo sits at least 108 px from every edge (use 112). On 9:16 copy stays between y 270 and y 1248, between x 65 and x 1015 (use a 90 px side margin), and clear of the Reels icon column (x > 885 below y 1087). Imagery and textless devices may run into the margins.
- **Q-03** · 22 Nov 2026. Safe-zone layer: the Meta safe-zone reference is the Figma Community file at figma.com/design/A3p5Z0WK0gIiv1u7bUSpwC. Place it in the background of every frame while designing; hide it when done but keep it in the layers so Shresht can cross-check.
- **Q-04** · 23 Nov 2026, from Shresht. Thumbnail test, a hard rule: shrink every export to about 20% (216 px wide for a 1080 px frame). The headline must still read and the product must still be recognisable, or the frame fails. Fix with size, contrast or simplification, never by cutting brief copy. Applies to all ads, their resizes and Shresht's own graphics.
- **Q-05** · 22 and 23 Nov 2026. Blind read-back on all rendered text: transcribe every glyph from the pixels without looking at the source copy, then diff. Mismatches fail the frame. Exception: an old-style figure in a serif body face (a "1" that reads like a short dotless i) is the font's design, not a wrong glyph; if the client's approved earlier work sets it the same way, note it once and pass the frame.
- **Q-06** · 22 Nov 2026. Craft floor: one idea per frame, real light direction, type with an idea, a designed ground (no flat default backgrounds).
- **Q-07** · 25 Nov 2026, from Shresht. No AI-tell details. Never add eyebrow labels ("Nº 01 — Standard"), tiny tracked-caps labels, numbered callout labels or catalogue index numbers: they flag the work as machine-made. An ad carries the brief's copy, the logo, and graphic devices with no words on them. Comparison marks are hand-drawn (marker strokes, slight rotation, uneven weight), never circle-badge ✓/× icons, which "give off a Claude vibe", and big enough to read at feed size.
- **Q-08** · 23 Nov 2026. A passing contrast ratio does not clear a frame. No shadow band, light streak, tonal edge or glow runs through the ground under any text block or behind the product. Thin serif body never sits on glowing or busy shapes. Fix with a local relight of the plate or an editable gradient scrim layer, and plan the copy zone in the render itself.
- **Q-09** · 20 Nov 2026. After replacing an image in a template layer, reset the fill and reframe the crop. Never trust an inherited transform: Shresht flags stretched images instantly.
- **Q-10** · 22 Nov 2026. Exact-size contract: canonical sizes enforced at export, native resolution with proper resampling. Upscale only as G-02 allows.
- **Q-11** · 21 Nov 2026. Before delivery, line the whole batch up side by side. If two ads look alike, redo one.
- **Q-12** · 20 Nov 2026. After anything ships, open it the way a viewer would and check every image, every order and every text before calling it done.

## V · Concepts and variety

- **V-01** · 21 Nov 2026. Tailor every ad to its client. Before designing, study the client's existing style (their Figma file, page 1 holds previous batches: colours, fonts, spacing, how much past ads vary), then research comparable brands. Then give each ad its own layout device and its own ground (red, white, black, whatever fits the palette): text inside the image, a smaller photo crop with room for type, a 3D touch, a shape behind the product with text on it. Composition experiments are expected. A batch built on one template looks lazy and the client sees it.
- **V-02** · 23 Nov 2026, from Shresht. One visual per ad. All four canvases of one ad (V1 1x1, V1 9x16, V2 1x1, V2 9x16) use the same visual and layout; V2 changes only the copy. Build V1, clone it for V2, swap headline, body and CTA, and re-fit the type. Variation happens between ads, never inside one ad.
- **V-03** · 23 Nov 2026. Meta's ad retrieval favours distinct concepts, and copy-only variants of one visual count as one concept. Batch variety comes from concept, visual and layout device, ad to ad.
- **V-04** · 20 Nov 2026. One signature graphic device per ad: something that makes the ad recognisably designed, not a default stack.
- **V-05** · 20 Nov 2026. No template-default compositions (such as a cream card with a photo strip). Either a full-bleed photo with type in the quiet zone, or a confident solid ground with one staged element. Elements break frame boundaries for real depth.
- **V-06** · 25 Nov 2026, from Shresht. The scene says the headline: "the visual needs to really mean the text". A generic product-on-sweep under a specific line is lazy work.
- **V-07** · 23 and 24 Nov 2026. Suggest, never use without Shresht's yes: native or unpolished looks (including designed copies of non-ad formats), busy high-density layouts, hammering a winner with a shared look, and nostalgia remixes. Restraint and design-heavy craft stay the default. Ask through Studio Desk.
- **V-08** · 20 and 24 Nov 2026. Imagery standard: no AI slop. Make scenes look built, not generated. Never fake-real AI people; for apparel and wearables, ask for client photos first.
- **V-09** · 24 Nov 2026, from Shresht ("use it", on the signalservice.co Sellbird promo reel). Standing approved style direction for static ads, static only: retro-UI sticker cards. Use it where it fits the client's brand (V-01).
  - Cream ground with a faint dot grid, faint enough that readability never dips.
  - Cards in flat colour fills with hard black offset shadows: solid, shifted, no blur, every shadow in the same direction.
  - One or two sticker labels per frame, set on a slight tilt, never a pile. Sticker and caption-pill words come from the brief's copy only (Q-07: no invented labels).
  - Palette: orange, black and white as the base, blue, green and purple as small accents.
  - A retro-UI tab bar with the current step highlighted can work as a progress device.
  - One short caption pill and one big headline per frame: the pill carries the sentence, the headline carries the idea.
  - Reference set: reference/style-directions.md.

## L · Layout

### Grid

- **L-01** · 23 Nov 2026. Every frame sits on a grid: fixed outer margins (Q-02) and a simple column grid. Text blocks, product and logo snap to it. Nothing is placed by eye alone.
- **L-02** · 23 Nov 2026. Elements share edges. Any two blocks that start or end near each other align to exactly the same edge or baseline; near-misses read as mistakes.

### Balance and visual weight

- **L-03** · 23 Nov 2026. Weight comes from size, contrast and colour density: a dark or busy element weighs more than a light one the same size.
- **L-04** · 23 Nov 2026. Every heavy element needs a counterweight on the opposite side of the frame, never more elements stacked on the same side.
- **L-05** · 23 Nov 2026. Balance is not symmetry. Check: flip the frame horizontally; if the flipped version feels like it tips over, the original was unbalanced.
- **L-06** · 23 Nov 2026. Squint test: read the frame as 2-3 weight masses. If one corner pulls everything, redistribute before shipping.

### Logo placement

- **L-07** · 23 Nov 2026. The logo is a quiet element, never the focal point: in a corner or anchored to the bottom row, at the grid margin, legible but never competing with the headline.
- **L-08** · 23 Nov 2026. One logo, placed once, never the biggest element on the ad.
- **L-09** · 23 Nov 2026. The logo counter-balances the layout: it goes on the light side of the frame, not onto the heavy side.
- **L-10** · 23 Nov 2026. The logo sits on clean ground with clear space of at least half its own height on all sides, never over a busy part of the image.

### Text block alignment

- **L-11** · 23 Nov 2026. One alignment axis per text group: heading, subline, body and CTA share one left edge, or the whole group is centred.
- **L-12** · 23 Nov 2026. Centred text only when the entire composition is centred. If anything else is left-anchored, the text is too.
- **L-13** · 25 Nov 2026, from Shresht. Centre when there's space: if left-aligned copy leaves empty space on its right, centre the whole composition (logo, hook, body, CTA and the visual under them). This covers every 9:16 with the visual below the copy, and any frame whose visual sits centred. Re-crop a moved visual from the original wide render rather than mirror-padding the plate. On 1:1, type left with the product right is still fine when the product fills the right side.

### Whitespace

- **L-14** · 23 Nov 2026. Whitespace is designed, not leftover: the empty areas are decided as deliberately as the filled ones.
- **L-15** · 23 Nov 2026. Margins and gaps come from one small spacing scale (multiples of one base unit), the same across every ad in a batch.
- **L-16** · 25 Nov 2026, from Shresht. Balance the corners: the margin at one corner matches the margin at the opposite corner, and a product sitting low-right gets the same margin as the type at top-left (112 px on 1:1). No dead empty band between copy groups and no dead quadrant ("Why an empty place here?").
- **L-17** · 23 Nov 2026. Gaps inside a group of related elements are smaller than gaps between groups.
- **L-18** · 23 Nov 2026. Keep text under about a fifth of the ad area.

### Line breaks

- **L-19** · 25 Nov 2026, from Shresht. Break at sentence ends. A two-sentence headline gets one sentence per line ("VETERAN-OWNED. / DRIVEN BY CURIOSITY."), sized so the longer sentence fits the measure. In body copy every sentence starts on a new line, and a long sentence wraps into balanced lines.
- **L-20** · 25 Nov 2026, from Shresht. Use the full width: a sentence that fits the measure stays on one line and runs to the end of the column; never break it early to make a narrower block. The measure is the real free width: 900 px on 9:16, and on 1:1 up to the nearest image element.
- **L-21** · 23 Nov 2026, from Shresht. Heading and subline breaks are uniform: never 3 or 4 words on the upper lines with a single orphan word on the last.
- **L-22** · 23 Nov 2026. Break at meaning boundaries and keep line lengths even. If one line has to be shorter, it is the first, never the last.
- **L-23** · 23 Nov 2026. An orphan word is a defect: rebalance the break, adjust the container or resize the type. Re-check breaks on every resize, since a break balanced in 1:1 can orphan in 9:16.

### Hierarchy and headline type

- **L-24** · 25 Nov 2026, from Shresht. One family per headline. Never mix a second typeface into a headline: a serif-italic accent word inside a grotesk headline flags as machine-made. (A client whose own brand system sets an accent face, like Lucori, follows its client file.)
- **L-25** · 25 Nov 2026, from Shresht. One emphasis device per headline: colour or weight, never both.
- **L-26** · 20 and 23 Nov 2026. One dominant element per frame, clearly the biggest: the headline or the visual, not both fighting. The headline is never timid.
- **L-27** · 23 Nov 2026. The scan order is designed: headline, then visual, then subline, then CTA and logo. Check with a 2-second flash test.
- **L-28** · 24 Nov 2026. Hook weight beats hook size: set hooks in bold to black weights; light weights are for supporting lines.
- **L-29** · 21 and 23 Nov 2026. Headlines on red, dark or black grounds go all white. Flat red shapes get texture or pattern, never a bare flat fill.

## C · Copy

- **C-01** · 21 Nov 2026, from Shresht. No pronouns in ad copy or video scripts: never "we", "us", "he", "him", "they", "them" or "I". CTAs are bare imperatives, e.g. "Need designs? DM or email."
- **C-02** · 23 Nov 2026, from Shresht. Exception: Shresht's LinkedIn posts and captions use first person ("I"). Never invent personal stories or results; use opinions and the real process.

## R · Research-use-only brands (peptides and similar)

- **R-01** · 20 Nov 2026. Zero humans, hands included. Vials, plain backgrounds, biotech texture. The ad's job is to attract, look professional and build presence.
- **R-02** · 23 Nov 2026. Vials never show liquid: empty, or fine sand-like powder filling about 10% from the bottom. Put it in every render prompt and check every vial image for a fill line.
- **R-03** · 21 Nov 2026. Vial labels are plain blank white, never branded or with added text.

## B · Shresht's own brand

- **B-01** · 21 Nov 2026. The mesh gradient (soft blurred blobs: coral, lavender, pale pink, brand orange) is a standing brand signature. It goes into every design for Shresht: X post mockups, templates, everything.
- **B-02** · 23 Nov 2026, from Shresht. A series never repeats one look. Every post in the own feed gets its own design style and type pairing, always on a light, premium-looking ground, and differs from the last 6 posts. The only constant is a thin identity thread (name footer, sample-ad label, one sparing accent). Fonts are free for commercial use. Craft rules still win: headline biggest, thumbnail test, no orphan word.
- **B-03** · 24 Nov 2026. Shresht's own photos stay real: the face is never generated or altered by AI. Cutouts are done locally, and any AI background removal is shown to Shresht before use. Profile kit: B&W headshot on the warm mesh, dark profile banner. Banners can go dark; the light-ground rule is for posts. One photo and one banner across LinkedIn, Behance and X.
- **B-04** · 25 Nov 2026, from Shresht. Behance presentations are Behance-coded and seamless, open on a show-stopping cover made in 3 options (the one that wins the gallery-thumbnail test stays), and share one house system across every series. Full rule: [own-brand/behance.md](own-brand/behance.md).
- **B-05** · 27 Nov 2026, from Shresht. Behance house system: covers 1616 x 1264 built for the 315 px card, the cover word in a heavy black-weight font over the textured electric-violet house colour (#5B2EFF), ad cards only from the project the cover fronts, seamless modules, General Sans + Satoshi. Full spec: [own-brand/behance.md](own-brand/behance.md).
- **B-06** · 26 Nov 2026, from Shresht. Every LinkedIn sample-ad post gets a new product mockup made for it, never a reused render. The product category and pack form differ from the last 6 posts, any D2C product works, and the brand on the pack is invented and carries the sample-ad label. Full rule: [own-brand/linkedin.md](own-brand/linkedin.md).
- **B-07** · 26 Nov 2026, from Shresht. Every LinkedIn post is built in Figma as editable layers (Q-01), one frame per post in one shared file, named by date and product, in posting order. Full rule: [own-brand/linkedin.md](own-brand/linkedin.md).
- **B-08** · 27 Nov 2026, from Shresht. His favourite Behance project, Mi An's "GRAPHIC DESIGN PORTFOLIO 2025", steers every Behance cover and presentation: what to take from it and what never to copy are in [own-brand/behance.md](own-brand/behance.md).
- **B-09** · 27 Nov 2026, from Shresht. His own short videos (self-recorded reels, 15 to 45 s) are edited to the motion standard of Simon Robert (@adswithsimon) and Jens Loman (@loman.jens): designed motion events (punch-ins, cards, grids, numbers, lists, titles) timed to the words, not one caption style running the whole clip. A template of big bouncing word captions was rejected: "I want better motion videos than this. This is really low quality." Visual reference only, never their assets. Edits run on local tools (G-08); captions come from what he says, never invented. A watermark burned in by his teleprompter app is cropped out by scale, never covered with a sticker. Studies: reference/reel-studies.md.

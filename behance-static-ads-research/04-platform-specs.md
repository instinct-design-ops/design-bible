# 04 — Platform specs: Meta & TikTok static ads

Drafted 26 Nov 2026 in a cloud session.

> **Verification status: UNVERIFIED against live pages.**
> This session's network can't reach `facebook.com` or `tiktok.com`; both hostnames fail to resolve. Every number below comes from the **official Meta and TikTok pages as the search index currently shows them**. Each page is cited by URL. Before you finalise artboards, open the "Verify" links at the bottom in your logged-in Chrome and tick them off. Where the official pages contradict each other, the conflict is flagged instead of resolved by guesswork.

---

## TL;DR — artboards to build

| Deliverable | Artboard | Ratio | Safe zone to design inside | Source confidence |
|---|---|---|---|---|
| Meta feed single image | **1440 × 1800** | 4:5 | Feed has no overlay. Keep ~5% margins as a habit (my convention, not Meta's) | High: two Ads Guide pages agree |
| Meta Stories / Reels single image | **1440 × 2560** (Reels) · 1080 × 1920 (Stories) | 9:16 | **Top 14% · bottom 35% · sides 6%** (Reels, the strictest) | High for Reels; Stories image zone not stated (see §1.3) |
| Meta carousel (feed) | **1080 × 1080** per card | 1:1 | 2–10 cards | High. 4:5 carousel = Advantage+ catalog only |
| Meta carousel (Stories) | **1080 × 1920** per card | 9:16 | Top & bottom ~14% (250 px) | Medium: pages conflict on resolution |
| TikTok image / carousel (in-feed) | **1080 × 1920** (export ≥ 720 × 1280) | 9:16 | Use TikTok's **official safe-zone overlay**; no single published % (see §2.4) | Medium |
| TikTok carousel | **2–35 images uploaded, max 20 shown**; music required | 9:16 recommended | Same as above | High (help article + API agree) |

**One 9:16 master that works on both platforms:** design at 1080 × 1920 (or 1440 × 2560 for Meta). Keep all copy, logo and CTA inside **x 6–94%, y 14–65%**. That is Meta's Reels zone, the strictest published one. It also clears TikTok's right-hand icon rail and bottom caption in most layouts, but that part is my **working assumption**. Check it against TikTok's overlay file.

---

## 1. Meta (Facebook + Instagram)

### 1.1 Feed single image, 4:5

| Field | Value | Source |
|---|---|---|
| Recommended ratio | **4:5** (vertical recommended for single-image feed ads) | [Ads Guide – FB Feed image](https://www.facebook.com/business/ads-guide/update/image) · [Best practices for aspect ratios](https://www.facebook.com/business/help/103816146375741) |
| Recommended resolution | **1440 × 1800 px** | [FB Feed image](https://www.facebook.com/business/ads-guide/update/image) · [FB Feed image, Traffic](https://www.facebook.com/business/ads-guide/update/image/facebook-feed/link-clicks) |
| Supported ratios | 1.91:1 → 4:5 (1:1 at 1440 × 1440 also listed) | [FB Feed image, Traffic](https://www.facebook.com/business/ads-guide/update/image/facebook-feed/link-clicks) |
| File type | JPG or PNG | same |
| Max file size | 30 MB | same |
| Minimum | 600 px wide; 750 px tall at 4:5 | same |
| Aspect-ratio tolerance | 3% | same |
| Instagram Feed | Same: 4:5, 1440 × 1800, 30 MB, 600 px min width, 3% tolerance; supports 1.91:1 to 4:5 | [Ads Guide (IG feed results)](https://www.facebook.com/business/ads-guide/update/image) |

**Conflict:** the carousel Help Center page gives **1080 × 1350** as the "recommended" 4:5 size ([1114358518575630](https://www.facebook.com/business/help/1114358518575630)). Both are 4:5. Design at 1440 × 1800 and export a 1080 × 1350 copy if needed.

### 1.2 Reels single image, 9:16

| Field | Value | Source |
|---|---|---|
| Ratio | 9:16 | [Ads Guide – IG Reels image](https://www.facebook.com/business/ads-guide/update/image/instagram-reels) |
| Resolution | **1440 × 2560 px** | same |
| File | JPG / PNG, max 30 MB, min width 500 px, ratio tolerance 1% | same |
| **Safe zone** | Keep **~14% top, ~35% bottom, ~6% each side** free of text, logos and key elements (profile icon, caption, CTA overlay) | same |

### 1.3 Stories single image, 9:16

| Field | Value | Source |
|---|---|---|
| Ratio | 9:16 ("fills the whole screen for Stories, Status and Reels") | [Best practices for aspect ratios](https://www.facebook.com/business/help/103816146375741) |
| Resolution | **1080 × 1920** recommended; **600 × 1067** minimum | [Design requirements for IG Stories ads](https://www.facebook.com/business/help/2222978001316177) |
| File | JPG / PNG, max 30 MB | [Design specs for Stories ads](https://en-gb.facebook.com/business/help/188477725155524) |
| Safe zone (stated for Stories **video**) | ~**14% (250 px) top**, ~**20% (340 px) bottom** | [Design requirements for IG Stories ads](https://www.facebook.com/business/help/2222978001316177) |
| Safe zone (FB Stories **carousel**) | ~**14% (250 px) top and bottom** | [About carousel ads in FB Stories](https://www.facebook.com/business/help/201503794673956) |

**Note:** I found no Stories safe zone published specifically for still images. If one 9:16 file runs on both Stories and Reels (Advantage+ placements will do that), the **Reels zone (14 / 35 / 6)** is the strictest and covers the others. Use it.

### 1.4 Carousel

| Field | Value | Source |
|---|---|---|
| Cards | **2–10** | [Design specs for carousel ads](https://www.facebook.com/business/help/1114358518575630) |
| Ratios | **1:1** and **9:16**. **4:5 only for Advantage+ catalog ads** built with catalog product images | same |
| 1:1 | 1080 × 1080 recommended | same |
| 4:5 | 1080 × 1350 recommended, 600 × 750 min (catalog only) | same |
| 9:16 (Stories) | 1080 × 1920 recommended, 500 × 888 min | same |
| Text (FB / Messenger / Audience Network) | Primary text **125**, headline **40**, link description **25** characters (recommended, not hard limits) | same |
| Text (Ads Guide, Awareness objective, FB Feed carousel) | Primary **80**, headline **45**, description **18** | [Ads Guide – FB Feed carousel](https://www.facebook.com/business/ads-guide/update/carousel) |

**Conflicts:** (a) The FB Stories carousel page lists "≥ 1080 × 1080" while the carousel spec page says 1080 × 1920. The 1080 × 1080 figure looks like a page error. (b) Text-length recommendations change by objective: 125/40 on most pages, 80/45/18 on the Awareness page.

**Portfolio implication:** a *manual* Meta feed carousel is **square (1:1)**, not 4:5. If the Behance project shows a 4:5 carousel, caption it as an Advantage+ catalog carousel, or build it 1:1.

### 1.5 Text that sits outside the image (affects how you mock up)

Meta displays primary text above the image, and the headline plus CTA button below it in feed. On Reels and Stories, the CTA button and caption overlay the bottom of the image. That overlay is the reason for the 35% bottom zone. The CTA *button* comes from a fixed Meta list chosen in Ads Manager ("Shop now", "Learn more", "Sign up" and so on). Any CTA designed *into* the image should support that button, not imitate it.

---

## 2. TikTok

### 2.1 In-feed (auction) ads, image / non-Spark

| Field | Value | Source |
|---|---|---|
| Ratios | **9:16 recommended** (≥ 540 × 960); 1:1 (≥ 640 × 640); 16:9 | [TikTok Auction In-Feed Ads](https://ads.tiktok.com/help/article/tiktok-auction-in-feed-ads) |
| Export target | 1080 × 1920 or higher | [Video advertising guide](https://ads.tiktok.com/business/en/guides/video-advertising-guide) |
| Caption (non-Spark) | Fixed white font, can't be customised; **no links, @ or hashtags** | [Auction In-Feed Ads](https://ads.tiktok.com/help/article/tiktok-auction-in-feed-ads) |
| Caption (Spark) | Pulled from the organic post; display limited to 4 lines including emoji | same |
| Account name | One line; **20 characters** (10 for CJK) | same |
| Profile image | 98 × 98 px, JPG/PNG, < 50 KB; keep key element within the central 66 × 66 | same |
| Ad description 1–100 characters | Confirmed only on the Global App Bundle image page (1–100 Latin / 1–50 Asian; no emoji, `{ }` or `#`). **Unconfirmed for TikTok in-feed** | [Image ads specification (GAB / Pangle)](https://ads.tiktok.com/help/article/image-ads-specification) |

### 2.2 Carousel ads

| Field | Value | Source |
|---|---|---|
| Images | **2–35 uploaded; max 20 displayed** | [Specifications for Carousel Ads](https://ads.tiktok.com/help/article/specifications-for-carousel-ads) · [Business API – Create carousel ads](https://business-api.tiktok.com/portal/docs/create-carousel-ads/v1.3) |
| Recommended sizes | 720 × 1280 (vertical), 640 × 640 (square), 1200 × 628 (horizontal) | [Specifications for Carousel Ads](https://ads.tiktok.com/help/article/specifications-for-carousel-ads) |
| API limits | Up to 1242 × 2340 / 2340 × 1242; ratios up to 9:20 / 20:9; < 50 MB per image | [Business API](https://business-api.tiktok.com/portal/docs/create-carousel-ads/v1.3) |
| Music | **Required** (MP3 upload, or TikTok Commercial Music Library). CML music isn't available on TikTok Ad Network placements | [Specifications for Carousel Ads](https://ads.tiktok.com/help/article/specifications-for-carousel-ads) |
| Best practice (playbook) | **Vertical 9:16**, **3 or 7–9 images**, 720p+. Other ratios may show black bars in feed | [Image Ads / Carousel Ads Playbook (PDF)](https://ads.tiktok.com/business/library/Image_Ads_Carousel_Ads_Playbook.pdf) |
| Objectives | Playbook: Traffic, App Promotion, Web Conversions, Lead Gen, Product Sales. Creation guide: Traffic, Web Conversions, App Promotion (conflict) | Playbook · [How to create a Carousel Ad](https://ads.tiktok.com/help/article/how-to-create-a-carousel-ad-in-tiktok-ads-manager) |
| Spark | Standard carousel Spark Ads supported (pulls an existing photo post); not supported for catalog-based carousels | API · Playbook |

### 2.3 Photo Mode (organic photo carousel → Spark carousel)

- In-app limit is **reported inconsistently**: creator guides say up to 35 photos, a Seller Center page says 30, and another source says 25. No official support-page number could be confirmed. **Check in the app.** ([Seller Center – Carousel (Shoppable Photo)](https://seller-ie.tiktok.com/university/essay?knowledge_id=6300676378904341))
- Design note: a Photo Mode post shown as a Spark ad keeps TikTok's organic UI (caption, right-hand rail, swipe dots). Mock it up inside that UI, not as a bare flat.

### 2.4 TikTok safe zone

- TikTok publishes **downloadable safe-zone overlay files** for in-feed ads instead of a single percentage. There are LTR and Arabic RTL versions, each with and without an anchor/link element. ([Auction In-Feed Ads](https://ads.tiktok.com/help/article/tiktok-auction-in-feed-ads) · [Reservation In-Feed](https://ads.tiktok.com/help/article/tiktok-reservation-in-feed-ads-reach-frequency))
- The usable area **shrinks as the caption gets longer**, and depends on ratio and any interactive add-on. TikTok says not to put text, logos or key messages where buttons, usernames and captions appear.
- Creative Center also offers a safe-zone preview tool (`ads.tiktok.com/business/creativecenter/tools/safe-zone/pc/en`). I couldn't load it from here.
- **Action:** download the official overlay on your computer and drop it on the 1080 × 1920 artboard. Until then, use Meta's 14 / 35 / 6 zone and add extra room on the right for TikTok's icon rail (working assumption).

### 2.5 Creative Center → Top Ads

- Filters: **Region, Industry, Campaign objective, Likes, Time frame**. **Ad language and Ad format filters are desktop only.** ([About Top Ads](https://ads.tiktok.com/help/article/top-ads) · [How to use the Top Ads dashboard](https://ads.tiktok.com/help/article/how-to-use-the-top-ads-dashboard))
- The format filter appears to offer **Spark ads / Non-Spark ads**. I couldn't confirm an "image" or "carousel" format option; check on desktop.
- Top Ads isn't exhaustive. It shows only ads the advertisers authorised. ([Top Ads](https://ads.tiktok.com/business/creativecenter/inspiration/topads))

---

## 3. Pixel cheat-sheet for the 9:16 safe zone

From Meta's Reels percentages (14% top, 35% bottom, 6% sides):

| Canvas | Top clear | Bottom clear | Side clear | Safe box (x × y) |
|---|---|---|---|---|
| 1080 × 1920 | 269 px | 672 px | 65 px | x 65–1015, y 269–1248 (**950 × 979**) |
| 1440 × 2560 | 358 px | 896 px | 86 px | x 86–1354, y 358–1664 (**1268 × 1306**) |

From Meta's Stories video figures (top 250 px, bottom 340 px on 1920): safe box y 250–1580 on 1080 × 1920.

**What this means for layout:** on a Reels-safe 9:16 ad the usable area is roughly a **square in the top two-thirds**. Put the headline and CTA there. The bottom third can hold image or texture only. The same composition holds up on TikTok, where the caption and CTA button also sit at the bottom.

---

## 4. Verify on your computer (logged-in Chrome)

- [ ] https://www.facebook.com/business/ads-guide/update/image — 4:5, 1440 × 1800, 30 MB, 3%
- [ ] https://www.facebook.com/business/ads-guide/update/image/instagram-reels — 1440 × 2560, 14/35/6
- [ ] https://www.facebook.com/business/ads-guide/update/image/instagram-story — Stories image resolution and any safe zone
- [ ] https://www.facebook.com/business/help/1114358518575630 — carousel 2–10, 1:1 / 9:16, 4:5 catalog only
- [ ] https://www.facebook.com/business/help/2222978001316177 — Stories 14% / 20% figures
- [ ] https://ads.tiktok.com/help/article/specifications-for-carousel-ads — 2–35 / 20 shown, sizes, music
- [ ] https://ads.tiktok.com/help/article/tiktok-auction-in-feed-ads — ratios; **download safe-zone overlay files**
- [ ] https://ads.tiktok.com/business/library/Image_Ads_Carousel_Ads_Playbook.pdf — 3 or 7–9 images
- [ ] https://ads.tiktok.com/business/creativecenter/inspiration/topads/pc/en — desktop Ad format filter: is there Image / Carousel?
- [ ] TikTok app → Photo Mode — max photos per post today

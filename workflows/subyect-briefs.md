# Subyect briefs: prompts

The rules are in [design-bible.md](../design-bible.md), section "Subyect freelance briefs". This file holds the prompts to paste into Claude.

## 1. Manual prompt (use this now)

When a brief arrives in your Subyect channel: open the Notion brief and the client's Figma file with the Subyect account, go to the page the design goes on, and copy that page's link (right-click the page > Copy link). Then paste this into Claude with the two links filled in:

```
Brief (Notion): [PASTE NOTION LINK]
Figma page: [PASTE FIGMA PAGE LINK]

1. Read the whole brief and print a receipt: client, deliverables with counts, ratios, the copy word for word, deadline, open questions.
2. Before drawing anything, review the earlier pages and frames for this client in the same Figma file (newest first, at least the last 3 batches). Write a consistency receipt: type families, weights and sizes; palette (hex); grid and margins; logo size and placement; CTA style; photo and product treatment; recurring layout devices; number of frames reviewed.
3. Read my design rules at https://github.com/instinct-design-ops/design-bible/blob/main/design-bible.md.
4. Design on the Figma page above, matching the consistency receipt. Copy goes in exactly as written (flag it if it doesn't fit, never shorten it); every frame fully editable (real text, separate logo, product and background layers); Meta safe zones; no eyebrow labels, tiny tracked-caps labels or numbered callouts; frame names follow the earlier pages.
5. Build every deliverable and ratio, then screenshot each frame and check every word against the brief. Finish with the Figma link for each frame and any flags.
```

## 2. Scheduled automation (off until Subyect has said it's fine)

This needs Slack (Subyect workspace), Notion and Figma connected with the Subyect accounts in the Claude that runs it, plus a log file on that computer. Set it as a scheduled task (every 30 minutes on weekdays, during working hours). Fill in the two bracketed values.

```
You are my Subyect brief autopilot. Work through these steps in order.

1. CHECK FOR NEW BRIEFS
- Read the messages from the last 24 hours in the Slack channel [MY SUBYECT CHANNEL], including thread replies.
- A brief is a message with a notion.so or notion.site link. Note any figma.com link in the same message or thread.
- This channel is my own: every Notion link Subyect posts here is a brief for me, even without a tag. Read ONLY this channel. Ignore every other channel and DM in the workspace, because those belong to other designers.
- Ignore links I posted myself, and links that are clearly not briefs (for example a feedback doc or an invoice). If a link's purpose is unclear, don't start it: list it in the notification as "unclear link" with the Slack link.
- Open [LOG FILE PATH]. Skip every brief whose Notion link is already logged.
- If there is no new brief, stop and say "No new Subyect briefs." Do nothing else.

2. READ THE BRIEF (one brief at a time, oldest first)
- Open the Notion brief and read all of it: client, deliverables, sizes and ratios, copy, references, deadline, and any Figma link.
- Print a brief receipt: client, deliverables with counts, ratios, the copy word for word, the deadline, and any open questions.

3. FIND THE FIGMA PAGE
- Use the Figma link from the brief or the Slack thread. The node-id in the link is the exact page or frame where the work goes.
- If there is no Figma link, look in the client's Figma file for the page this brief belongs to. Do not create a page or guess between two candidates. If it is not clear, log the brief as "waiting: needs Figma page link", send me a notification with the client name and the Notion link, and move to the next brief.

4. REVIEW THE PREVIOUS DESIGNS FIRST (before drawing anything)
- In the same Figma file, take screenshots of the earlier pages and frames for this client (the most recent first, at least the last 3 batches).
- Write a consistency receipt: type families, weights and sizes; colour palette (hex); grid and margins; logo size and placement; CTA style; how photos and products are treated; recurring layout devices. Count how many frames you reviewed.
- Also read my design rules at https://github.com/instinct-design-ops/design-bible/blob/main/design-bible.md (standing workflow rules, rejected directions, layout design rules).

5. DESIGN
- Design on the target page, matching the consistency receipt. This client's earlier pages win over generic taste.
- Hard rules: copy goes in exactly as written in the brief (if it doesn't fit, flag it, never shorten it); every frame is fully editable (real text layers, separate logo, product and background layers, nothing flattened); respect the Meta safe zones; no eyebrow labels, tiny tracked-caps labels or numbered callouts; frame names follow the client's existing naming on earlier pages.
- Build every requested deliverable and ratio. Then screenshot each frame and check every word against the brief, letter by letter.

6. REPORT AND LOG
- Append to the log file: date, client, Notion link, Figma page link, status (done / waiting / blocked) and a one-line note.
- Send me a notification: client, what was designed with counts, the Figma link for each frame, and any flags (copy that didn't fit, missing assets, questions).
- Never post, react or reply in Slack, never comment in Notion, and never message anyone at Subyect. Only I talk to the agency.
```

To have it prepare everything but wait for you before designing, replace step 5 with: "Stop after step 4 and send me the brief and consistency receipts."

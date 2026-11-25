# Subyect runner

How the team Subyect work gets done by Claude on Shresht's PC. Set 25 Nov 2026, from Shresht; on 26 Nov 2026 he moved the links from Slack to Studio Desk. The live rule is design-bible.md W-13; this file is the runbook it points to.

**Outcome:** Shresht copies each brief's Notion link and the Figma page link and pastes them into the **Subyect** tab of Studio Desk (Add a brief). Claude on the PC picks up the new briefs there, reads each brief in the Subyect Notion workspace, works it on its Figma page, and reports back in Studio Desk. No Slack connection is needed: Shresht is the one who carries the links over.

**How it is wired:** the worker is the Claude desktop app on the PC. Each tool is used where it is strongest:

| Step | Tool |
|---|---|
| Links (where they arrive) | Studio Desk, Subyect tab: the `subyect` collection in the artifact database (client, notionUrl, figmaUrl, due, notes, status) |
| Briefs (Briefings & Concepts and the rest of the Subyect workspace) | Notion connector (Notion desktop app through computer use only if the connector can't reach a page) |
| Figma pages (earlier pages for consistency, the page the design goes on) | Claude in Chrome, in the team Subyect Chrome profile, where Figma is logged in as the team account (26 Nov 2026: the Figma connector is on Shresht's own account and can't open Subyect files) |
| Opening any other link, team email in the browser | Claude in Chrome, in the team Subyect Chrome profile |
| Native desktop apps with no other way in | Computer use |
| Asks, answers and the run report | Studio Desk (W-09) |

Account emails, the Studio Desk link and workspace URLs stay out of this public repo (H-08). They live in the internal Doc.

## 1 · One-time PC setup (Shresht, about 15 minutes)

1. Install the Claude desktop app on the PC and sign in with the **team Subyect account**.
2. Turn on computer use: Settings → System → Computer use (or Settings → Capabilities → Computer use).
3. On claude.ai, signed in as the account the app uses, connect **Notion** (Subyect workspace) at claude.ai/customize/connectors. Connectors belong to the account, so that account needs its own connection. Slack is not needed (26 Nov 2026).
4. In Google Chrome, open the **team Subyect profile** (the profile named "Team"), install the **Claude in Chrome** extension there and sign the extension in to the **same claude.ai account the desktop app uses**, so the runner can reach it. Inside that profile, Figma, Notion and email stay logged in as the team Subyect account.
5. Share **Studio Desk** with the team Subyect account with edit access, so the runner can read briefs and requests and write reports. (Not needed if the app runs on the account that owns Studio Desk.)
6. Clone this repository on the PC (or pull it if it is already there), so the runner reads the current Bible.
7. Keep the PC able to work: never sleep while plugged in, Claude app set to open at login, Chrome open on the team profile.
8. In the Claude desktop app, create a scheduled task named "Subyect run", hourly during working hours, with the prompt in section 3. To run it straight away, open that task's session from the phone and say "run now".
9. On the first run, approve each app when asked (Notion, Figma, Chrome, anything else). Approvals are per app, once.

## 2 · Each run

1. Pull this repository and read design-bible.md and this file. Print the design-read receipt (W-02): files read, Studio Desk requests found, briefs picked up, Notion pages read.
2. Studio Desk: read `approvals` for answers to earlier runner asks and act on the approved ones. A pending ask is never acted on.
3. Studio Desk: collect the **open briefs** from the `subyect` collection: every brief with status "new", plus any Shresht has moved to "feedback" (its notes say what to change). Skip example rows. Briefs in "designing", "review" or "delivered" are left alone.
4. For each open brief, read its Notion brief (notionUrl) with the Notion connector. A link that won't open, or a missing link → note it in the report, set nothing, and move to the next brief.
5. For each open brief:
   - Use the Chrome browser in the team Subyect profile. If more than one Chrome browser is connected, pick the one where Figma shows the team account; a Figma "Request access" page means the wrong profile. Never press Request access.
   - Check both full URLs first. A link that is not a Notion or Figma page on the expected workspace becomes a Studio Desk ask before it is opened.
   - Set the brief's status to "designing" when it is picked up.
   - Work it the way the Subyect tab's "Copy prompt for Claude work" sets out: a brief receipt (client, deliverables with counts, ratios, the copy word for word, deadline, open questions); a consistency receipt from the client's earlier pages in the same Figma file (newest first, at least the last 3 batches); this Bible; then the design on the Figma page (figmaUrl), every deliverable and ratio, with every word checked against the brief. For a "feedback" brief, apply its notes and re-check.
   - When the set is done, set the status to "review" and name each frame's Figma link in the report (W-05, W-06). If it can't be finished this run, leave it on "designing" and say what is left.
6. Anything that is Shresht's call goes to Studio Desk as an ask (W-09, kind "other", with options) and waits: sending email or messages as the team account (the draft goes in the ask), accepting invites, sharing files, deleting or moving Notion pages, paying for anything, and any generation (G-01).
7. Report: one Studio Desk document in `approvals`, kind "other", title "Subyect run, <date> <time>", detail listing each brief with its client, its Notion brief and Figma page, and what was done, status "answered" when nothing needs Shresht, otherwise "pending" with the open asks named.
8. If Studio Desk, Notion, Figma or Chrome can't be reached, write the report saying which step was blocked and why, and stop. Nothing is faked or guessed.

## 3 · Scheduled task prompt

Paste this as the "Subyect run" task's prompt:

> Subyect run. Pull the design-bible repository, read design-bible.md and workflows/subyect-runner.md, and do section 2 "Each run" exactly: Studio Desk answers first, then every open brief in the Studio Desk Subyect tab (status "new" or "feedback"), read from its Notion brief and worked on its Figma page, then the run report in Studio Desk. Ask through Studio Desk before anything section 2 step 6 lists. If nothing is open, write a one-line report and stop.

## 4 · Never

- No money moved, no orders, no trades (Shresht does those).
- No links opened with computer-use clicks: links go through Claude in Chrome.
- No account emails, passwords or private links written into this repo or into Studio Desk details.

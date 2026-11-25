# Subyect runner

How the team Subyect work gets done by Claude on Shresht's PC. Set 25 Nov 2026, from Shresht. The live rule is design-bible.md W-13; this file is the runbook it points to.

**Outcome:** Shresht sends a word (a Studio Desk request, or a message to the PC session from the phone). Claude on the PC checks Slack for open links, opens the matching brief in the Subyect Notion workspace, works each link in the team Subyect Chrome profile with the team Subyect account, and reports back in Studio Desk.

**How it is wired:** the worker is the Claude desktop app on the PC, signed in with the team Subyect account. That Claude is already "the Claude in the team Subyect Chrome, on the team email", so no Claude has to type prompts into another Claude. Each tool is used where it is strongest:

| Step | Tool |
|---|---|
| Links (where they arrive) | Slack connector (Slack desktop app through computer use only if the connector can't reach a channel) |
| Briefs (Briefings & Concepts and the rest of the Subyect workspace) | Notion connector (Notion desktop app through computer use only if the connector can't reach a page) |
| Opening and working the links, team email in the browser | Claude in Chrome, in the team Subyect Chrome profile |
| Native desktop apps with no other way in | Computer use |
| Asks, answers and the run report | Studio Desk (W-09) |

Account emails, the Studio Desk link and workspace URLs stay out of this public repo (H-08). They live in the internal Doc.

## 1 · One-time PC setup (Shresht, about 15 minutes)

1. Install the Claude desktop app on the PC and sign in with the **team Subyect account**.
2. Turn on computer use: Settings → System → Computer use (or Settings → Capabilities → Computer use).
3. On claude.ai, signed in as the team Subyect account, connect **Notion** (Subyect workspace) and **Slack** (the Subyect Slack, with the link channels) at claude.ai/customize/connectors. Connectors belong to the account, so the team account needs its own connections.
4. In Google Chrome, open the **team Subyect profile**, install the **Claude in Chrome** extension there and sign it in with the team Subyect account.
5. Share **Studio Desk** with the team Subyect account with edit access, so the runner can read requests and write reports.
6. Clone this repository on the PC (or pull it if it is already there), so the runner reads the current Bible.
7. Keep the PC able to work: never sleep while plugged in, Claude app set to open at login, Chrome open on the team profile.
8. In the Claude desktop app, create a scheduled task named "Subyect run", hourly during working hours, with the prompt in section 3. To run it straight away, open that task's session from the phone and say "run now".
9. On the first run, approve each app when asked (Slack, Notion, Chrome, anything else). Approvals are per app, once.

## 2 · Each run

1. Pull this repository and read design-bible.md and this file. Print the design-read receipt (W-02): files read, Studio Desk requests found, Notion pages scanned.
2. Studio Desk: read `approvals` for answers to earlier runner asks and act on the approved ones. A pending ask is never acted on.
3. Slack: collect the **open links**: every link posted in the link channels (listed in the internal Doc) that has no ✅ reaction from the team Subyect account. Read the message and its thread for what is being asked.
4. Notion: for each link, find its brief in the Subyect workspace (Briefings & Concepts first; match by the brief number, client or Figma file named in the Slack message). No matching brief → note it in the report and still work the link from the Slack message alone.
5. For each open link, in the team Subyect Chrome profile:
   - Check the full URL first. Links from unknown senders or unfamiliar domains become a Studio Desk ask before they are opened.
   - Do what the Slack message asks, against its Notion brief. If nothing is asked, read the link and put a 3-line summary, what it means for the brief, and one suggested next step in the run report.
   - React 👀 on the Slack message when the link is picked up and ✅ when it is done. Thread replies in Slack go out only once Shresht has approved them in Studio Desk (step 6).
6. Anything that is Shresht's call goes to Studio Desk as an ask (W-09, kind "other", with options) and waits: sending email or Slack messages as the team account (the draft goes in the ask), accepting invites, sharing files, deleting or moving Notion pages, paying for anything, and any generation (G-01).
7. Report: one Studio Desk document in `approvals`, kind "other", title "Subyect run, <date> <time>", detail listing each link with its Slack message, its Notion brief and what was done, status "answered" when nothing needs Shresht, otherwise "pending" with the open asks named.
8. If Slack, Notion, Chrome or Studio Desk can't be reached, write the report saying which step was blocked and why, and stop. Nothing is faked or guessed.

## 3 · Scheduled task prompt

Paste this as the "Subyect run" task's prompt:

> Subyect run. Pull the design-bible repository, read design-bible.md and workflows/subyect-runner.md, and do section 2 "Each run" exactly: Studio Desk answers first, then every open link in the Slack link channels, matched to its brief in the Subyect Notion workspace and worked in the team Subyect Chrome profile, then the run report in Studio Desk. Ask through Studio Desk before anything section 2 step 6 lists. If nothing is open, write a one-line report and stop.

## 4 · Never

- No money moved, no orders, no trades (Shresht does those).
- No links opened with computer-use clicks: links go through Claude in Chrome.
- No account emails, passwords or private links written into this repo or into Studio Desk details.

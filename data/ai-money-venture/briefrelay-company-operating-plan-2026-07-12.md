# BriefRelay Company Operating Plan

Updated: 2026-08-03 15:45 MDT  
Owner: Jarvis  
Marketing owner: Mercury  
Design owner: Vega  
Public board: `https://getbriefrelay.github.io/briefrelay-status.html`

## Operating Mandate

Kevin expects BriefRelay to move without repeated prompting. Jarvis should review the company, decide the next useful work, execute it, and use the public board as the running status surface. Chat updates should not replace board updates.

## Current Company State

- Offer: missed-lead intake desk for local service businesses.
- Target buyer: local service operators where slow response loses revenue.
- Core pilot: one approved lead source, urgent lead flags, safe reply drafts for approval, follow-up tracking, daily owner brief.
- Price anchor: $750 pilot, with $300-$1,000/month expansion path.
- Public social: Instagram `@briefrelay`, 15 posts live as of 2026-08-03 15:45 MDT; August 3 Monday Lead Stack is newest at `https://www.instagram.com/briefrelay/p/DblRDE2kVJB/`. August 4 Draft With A Seatbelt was repaired and visually checked; August 5-9 are spot-check cleared.
- Public website/board: V1 static customer site and current status board are live on the branded free GitHub Pages URL `https://getbriefrelay.github.io/`; source repo is `https://github.com/getbriefrelay/getbriefrelay.github.io`. Kevin's admin-access Pages repo at `https://kevinpyles.github.io/briefrelay-site/briefrelay-status.html` remains a fallback mirror.
- Brand: Vega V4D / Lead Lift identity, fun-bold BriefRelay guide, buyer-safe humor.
- Marketing: Mercury owns the calendar, copy, content backlog, and email/social campaign improvement.
- Outreach: 84 outbound outreach emails sent as of 2026-08-03 09:27 MDT; July 31 recovery sent nine Batch 5/6 Follow-Up 2 close-loop emails and Gmail Sent verified `1-9 of 9`. August 3 Gmail browser checks found no human prospect replies, no new prospect delivery failures, and spam empty. Batch 8 replacement prospects are staged in `data/ai-money-venture/outreach/batch8_public_email_targets.csv` for approval; do not send until approved. `gws` Gmail OAuth now reaches Google but is blocked because the OAuth app is still in testing and `briefrelayops@gmail.com` is not an approved tester, so browser Gmail remains the operating path.
- Board: local source page is live, and the current public status page is published on the branded GitHub Pages repo using the stored `getbriefrelay` GitHub CLI config. Kevin's Pages repo remains a fallback mirror if branded auth fails.

## Audit Findings

1. **Marketing had a plan but not enough ready assets.**  
   The 30-day plan and captions existed, but only July 13 had a rendered post. Fixed by creating a July 14-19 asset batch.

2. **The old V3 brand builder is now unsafe to rerun.**  
   `scripts/build_briefrelay_brand_v3.js` contains stale V3 copy and can overwrite the approved V4D identity. Use `scripts/build_briefrelay_daily_assets.js` for current daily queue assets. Future cleanup should either archive or update the V3 builder.

3. **The board is the right update channel but was stale.**  
   It still showed an older as-of time and did not clearly list the current company projects. Update the board whenever work moves forward or blocks.

4. **Google/Gmail profile photo is updated.**  
   The V4D avatar was uploaded through the Google Account photo dialog and visually verified on the About Me profile page. Google warned it can take a day or two to propagate across services.

5. **Instagram posting has a working default path.**  
   Business Suite browser upload is unreliable and should not be retried as the primary route. Prepare the daily asset/caption, publish through the native Instagram web composer with CDP file-input targeting, and target only the create-post media input; the profile page also exposes hidden profile-photo file inputs.

## Active Projects

| Priority | Project | Owner | Next Action | Status |
|---|---|---|---|---|
| P0 | Daily Instagram execution | Jarvis + Mercury + Vega | Publish through native Instagram web composer using direct CDP against the create-post file input; use Business Suite only if CDP is unavailable | Active |
| P0 | Board as source of truth | Jarvis | Keep board current locally, publish to GitHub Pages after updates, and verify the hosted URL | Active |
| P1 | Email campaign V2 | Mercury + Jarvis | Check deliverability/replies, then send eligible outreach within mandate and caps | Active |
| P1 | Brand asset consistency | Vega + Jarvis | Keep V4D active across board, guide, Instagram; Google/Gmail photo sync is cosmetic/manual | Active |
| P1 | Brand-forward website URL | Jarvis | Keep `https://getbriefrelay.github.io/` verified for the website/board; keep Kevin's Pages repo as a fallback mirror | Active |
| P1 | Reusable content system | Vega + Mercury | Turn daily queue into repeatable templates | Active |
| P2 | Outreach pipeline expansion | Mercury + Jarvis | Review/approve staged Batch 8 public-email prospects before any new first-touch outreach | Ready for approval |
| P2 | Builder cleanup | Jarvis | Archive/update stale V3 generator to prevent accidental overwrite | Planned |

## Expected Daily Loop

- Check Gmail for human replies, bounces, spam, and account warnings before sending. Use managed-browser Gmail as the supported route while `gws` OAuth is invalid.
- Send eligible outreach emails within Kevin's approved BriefRelay mandate and caps; verify sends in Gmail Sent.
- Publish and verify one Instagram post while BriefRelay is in launch mode; use native Instagram CDP upload against the create-post file input as the default route.
- Update outreach logs, prospect tracker, Instagram launch log, board, memory, and Obsidian project note after material changes.
- Verify the public board URL after board updates and include the current timestamp, totals, post count, known bounces, and blockers.
- Report the outcome with evidence, or report an exact blocker and next owner/step.

## Operating Rules Going Forward

- Do not wait for Kevin to ask what is next.
- Treat expected daily BriefRelay work as execution: check replies/bounces, send eligible outreach emails, publish and verify the Instagram post, update logs/trackers, update the board, verify the public board URL, and report with evidence.
- Update the board when status changes and before sending internal status emails.
- Every board update must include an accurate "As of" date/time stamp with timezone plus current outreach totals, Instagram post count, known bounces, and blockers.
- Keep the local board healthy and use GitHub Pages as the public board path.
- Prepare at least one post per day while BriefRelay is in launch mode.
- Make humor useful: inbox chaos is the joke, not the owner or customer.
- Do not claim external updates are complete unless verified.
- For Instagram, do not let Business Suite upload failure stall the cadence: use the native Instagram web composer with direct CDP file-input targeting, then verify the live URL and avatar state.

## 2026-07-17 Instagram Recovery Note

- Published July 17 Hot Leads Up after the 08:00 Business Suite/native attempts failed. Working route: restart the managed browser if the composer is poisoned, open native Instagram `Create -> Post`, use CDP `DOM.setFileInputFiles` against the create-post input that accepts feed media, add Mercury's approved caption, share, and verify profile count/newest URL.
- Live URL: `https://www.instagram.com/briefrelay/p/Da5wEL2ER4C/`. Verification: `@briefrelay` shows 5 posts and V4D avatar restored.
- Caution: do not set all hidden `input[type=file]` nodes. One is a profile-photo input; it briefly replaced the avatar during troubleshooting and had to be restored through Edit Profile.

## 2026-07-17 Growth-Ops Note

- Gmail: managed browser remained logged in as `briefrelayops@gmail.com`; no human prospect replies, no last-day delivery/bounce matches, spam empty, and the recovery-phone warning remains.
- Outreach: no new prospect email sent at 10:20 because no Mercury-reviewed unsent batch was ready and July 17 had only 3 conservative sends remaining after the morning follow-ups.
- Pipeline: Batch 7 staged for Mercury review with Icon Roofing, Ryan Mechanical Company, Arid Valley Plumbing, Ground Zero Plumbing AC and Electrical, and Gold Star Plumbing & Drain.
- Next send rule: Mercury must review the 5-email batch; rotate at least three subject patterns; preserve "Nothing sends without approval"; log copy angle.

## 2026-07-18 Operator Note

- Coordination: BriefRelay group check-in was posted. Direct configured-agent pings to `BriefRelayMercuryBot` and `BriefRelayVeraBot` returned `agent not found`, so written Mercury/Vega handoffs were used.
- Gmail: managed browser was logged in as `briefrelayops@gmail.com`; no human prospect replies, no last-day delivery/bounce matches, spam empty, and the Google recovery-phone warning remains. Gmail Drafts still shows 3 leftover July 17 autosaves.
- Outreach: sent four eligible Batch 1 Follow-Up 2 close-loop emails to Sweet Dreams Plumbing, Harper's Roofing, Mesa Roofing LLC, and Stradling Roofing. Almeida was excluded because they replied not interested. Gmail Sent verified `1-4 of 4` for today's close-loop subject at 8:08-8:09 MDT.
- Instagram: July 18 Things Found In The Inbox is live at `https://www.instagram.com/briefrelay/p/Da793pakS8X/`; profile shows 6 posts and the V4D avatar still appears active. Business Suite still fails to attach media, and native Instagram's normal upload handoff did not attach; direct CDP against the create-post media input worked.
- Next action: monitor replies/bounces, keep Batch 7 waiting for Mercury review, and publish July 19 Sunday Desk Reset tomorrow.

## 2026-07-20 Operator Note

- Coordination: Direct configured-agent pings to `BriefRelayMercuryBot` and `BriefRelayVeraBot` still returned `agent not found`; Jarvis used written Mercury/Vega handoffs and the July 18 Vega memory note. No newer handoff/update files were found except Vega's July 18 brand/content check.
- Gmail: Managed browser was logged in as `briefrelayops@gmail.com`; `gws` Gmail auth still fails with `invalid_grant`. Search `after:2026/7/18 -in:sent -in:drafts` returned no messages, targeted `newer_than:3d` delivery/bounce search returned no messages, and spam was empty. Google recovery-phone warning remains visible.
- Outreach: Sent five Batch 7 first-touch emails to Icon Roofing, Ryan Mechanical Company, Arid Valley Plumbing, Ground Zero Plumbing AC and Electrical, and Gold Star Plumbing & Drain. Gmail Sent verified `1-5 of 5` at 8:08-8:10 MDT. Outreach total is now 56 emails and 35 unique public prospects contacted.
- Instagram: July 20 Roof Leak Next To Newsletter is live at `https://www.instagram.com/briefrelay/p/DbBHeD5kWag/`; profile shows 7 posts. Business Suite again returned `ok` without attaching media, and native Instagram's normal upload handoff stayed on `Select from computer`; direct CDP against the create-post media input worked.
- Content runway: Generated July 20-26 SVG/PNG assets in `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-20/`. July 19 Sunday Desk Reset was missed by the stale run and remains staged, not back-posted.

## 2026-07-21 Instagram Recovery Note

- Cause: the 08:00 daily operator cron fired but the isolated run ended with `AbortError: agent run aborted`, so the July 21 Instagram publish, checks, and board update did not complete on schedule.
- Recovery: Jarvis manually resumed the Instagram work at 15:52 MDT. The first clean browser restart triggered Instagram's human-confirmation checkpoint; after it cleared, normal upload handoffs still returned `ok` without attaching media. Direct CDP `DOM.setFileInputFiles` against only the native create-post feed-media input attached the converted JPEG and allowed publishing.
- Instagram: July 21 Missed Lead Confession #2 is live at `https://www.instagram.com/briefrelay/p/DbEhcacEWd6/`; profile shows 8 posts.
- Next action: tomorrow's operator should publish July 22 Follow-Up Did Not Ghost You from the ready queue and should treat an aborted run as a same-day recovery item, not a silent miss.

## 2026-07-22 Operator Note

- Coordination: BriefRelay group kickoff posted. Direct configured-agent pings to `BriefRelayMercuryBot` and `BriefRelayVeraBot` still returned `agent not found`, so written Mercury/Vega handoffs were used.
- Gmail: `gws` Gmail auth still fails with `invalid_grant`; managed browser remained logged in as `briefrelayops@gmail.com`. Search `newer_than:2d -in:sent -in:drafts` showed two Instagram account/security notices only, including July 21 "You're back on Instagram"; targeted delivery/bounce search returned no messages and spam was empty. No human prospect replies found.
- Outreach: Sent nine eligible Follow-Up 1 emails to AZ Roofing Works, Birdie Plumbing AZ, Streamline Plumbing AZ, Sunline Plumbing, Air Care, 911 Air Repair, Precise Air & Heating, Authorized AC, and Accurate Air. Guardian Contracting Group was excluded because it bounced. Gmail Sent verified `1-9 of 9` for today's 11:47 PM follow-up subject at 8:04-8:06 MDT. Outreach total is now 65 emails.
- Instagram: July 22 Follow-Up Did Not Ghost You is live at `https://www.instagram.com/briefrelay/p/DbGR2DZEY4q/`; profile shows 9 posts. Business Suite was blocked at the Meta login chooser; native Instagram normal upload handoff returned `ok` without attaching media; direct CDP against the feed-media input worked.
- Next action: monitor today's follow-ups for replies/bounces and publish July 23 Before/After Brief from the ready queue.

## 2026-07-23 Daily Operator Note

- Coordination: Direct configured-agent pings to `mercury` and `vega` succeeded. Mercury reported no overnight marketing changes and confirmed July 23 Before/After Brief was queued; Vega reported no new design changes and confirmed the July 23 asset remained V4D-aligned.
- Gmail: `gws` Gmail auth still fails with `invalid_grant`; managed browser remained logged in as `briefrelayops@gmail.com`. Broad non-sent search showed only the Instagram account-restored notice; targeted newer_than:3d delivery/bounce search returned no messages; spam was empty. No human prospect replies found.
- Outreach: Batch 7 Follow-Up 1 went to Icon Roofing, Ryan Mechanical Company, Arid Valley Plumbing, Ground Zero Plumbing AC and Electrical, and Gold Star Plumbing & Drain, but each recipient received the follow-up twice because a browser/session send path duplicated the queued compose recovery. Gmail Sent verified `1-10 of 10` for `in:sent after:2026/7/23 "The 11:47 PM estimate request"` at 8:03-8:13 MDT. Outreach total is now 75 emails and the July 23 outreach cap is consumed; no further Batch 7 follow-up unless a prospect replies.
- Instagram: July 23 Before/After Brief is live at `https://www.instagram.com/briefrelay/p/DbI3bzLEXBI/`; profile shows 10 posts. Business Suite remained blocked at the Meta login chooser; normal native upload handoff failed; direct CDP against only the create-post feed-media input worked. A duplicate July 23 post was briefly created at `https://www.instagram.com/briefrelay/p/DbI3aN3EfUn/` and the older duplicate was deleted.
- Next action: monitor Batch 7 for reply/bounce impact from the duplicate follow-up, keep July 24 No Autopilot Promises ready, and avoid leaving prefilled compose tabs open before future sends.

## 2026-07-24 Low-Token Recovery Note

- Daily operator status: the `briefrelay-8am-company-operator` cron retried around 08:00 MDT and failed before execution with the Codex subscription usage-limit error. Reset is reported as July 28, 2026 at 11:27 AM MDT.
- Board/status: public board remained reachable with HTTP 200, but it was stale from July 23 until this note/board update. Current durable counts remain 75 outreach emails and 10 live Instagram posts.
- Execution status: no July 24 Gmail browser check, outreach send, Instagram publish, or agent handoff was completed in this low-token recovery pass. July 24 No Autopilot Promises remains queued and should be handled by a lower-token route or after quota recovery.

## 2026-07-24 Recovery Completion Note

- Instagram: July 24 No Autopilot Promises is live at `https://www.instagram.com/briefrelay/p/DbMEZylGR5M/`. Generic upload failed and a JPEG retry hit Instagram's "Something went wrong" dialog; restarting the managed browser and using native Instagram CDP file-input targeting with the PNG worked. Profile verified at 11 posts with the July 24 post newest.
- Gmail/outreach: managed browser Gmail was logged in as `briefrelayops@gmail.com`; `newer_than:1d -in:sent -in:drafts` returned no messages, targeted delivery/bounce search returned no messages, and spam was empty. No outreach email sent because all apparent due contacts were monitor-only, Batch 7 was duplicated/over-contacted on July 23, and Batch 5/6 next normal follow-up window is July 28.

## 2026-07-27 Manual Recovery Completion Note

- Cause: the 8 AM `briefrelay-8am-company-operator` cron run aborted with `AbortError: agent run aborted`, so the daily operator path had to be recovered manually.
- Cron hardening: edited the daily cron to use light context, low thinking, a 3600-second timeout, and a shorter concrete recovery checklist so future runs are less likely to stop after a broad blocked report.
- Gmail/outreach: managed browser Gmail was logged in as `briefrelayops@gmail.com`. Broad search `newer_than:3d -in:sent -in:drafts` returned no messages; targeted 7-day delivery/bounce search returned no messages; spam `newer_than:7d` returned no messages. `gws` Gmail auth still fails with `invalid_grant`. No outreach email was sent because Batch 7 remains under the duplicate-send guard and Batch 5/6 next normal follow-up window is July 28.
- Instagram: July 25 HVAC Lead Aging Like Milk was recovered and published on July 27 via native Instagram CDP feed-media input targeting. Live URL: `https://www.instagram.com/briefrelay/p/DbTXhJgkRP6/`. `@briefrelay` verified at 12 posts with the no-cooling lead graphic newest.
- Remaining watch item: the cron history still shows the July 27 8 AM run as failed, but the business work from that blocked run has been manually recovered and the future cron configuration has been tightened.

## 2026-08-01 Operator Note

- Gmail/outreach: `gws` Gmail auth still fails with `invalid_grant`; managed browser remained logged in as `briefrelayops@gmail.com`. Search `in:anywhere newer_than:1d -in:sent -in:drafts` returned no messages, targeted delivery/bounce search showed only the internal Matt campaign-review thread, and spam was empty. No outreach email was sent because no tracker item is eligible today, Batch 5/6 have completed Follow-Up 2, and Batch 7 remains under duplicate-send guard.
- Instagram: Lead Archaeology was published with native Instagram CDP feed-media input targeting after normal upload returned `ok` without attaching media. Live URL: `https://www.instagram.com/briefrelay/p/DbgAzYokYTh/`; profile verified at 14 posts.
- Next action: build the next August Instagram queue/assets and research a replacement prospect batch before any new first-touch outreach.

## 2026-08-02 Operator Note

- Gmail/outreach: `gws` Gmail auth still fails with `invalid_grant`; managed browser remained logged in as `briefrelayops@gmail.com`. Broad non-sent last-day search returned no messages, targeted seven-day delivery/bounce search showed only the known internal Matt campaign-review thread, and spam was empty. No outreach email was sent because no tracker item is eligible today, Batch 5/6 have completed Follow-Up 2, and Batch 7 remains under duplicate-send guard.
- Instagram: no post published during the operator run because no approved current August asset queue existed at that time. `@briefrelay` was verified at 14 posts with August 1 Lead Archaeology still newest at `https://www.instagram.com/briefrelay/p/DbgAzYokYTh/`. Afterward, Mercury/Vega prepared the August 3-9 queue; August 3 Monday Lead Stack is cleared, August 4 Draft With A Seatbelt needs a clipping fix, and August 5-9 passed spot check.
- Next action: publish August 3 Monday Lead Stack in the next daily operator run, fix August 4 clipping before its post date, and research a replacement prospect batch before any new first-touch outreach.

## 2026-08-03 Manual Recovery Note

- Cron status: the 08:00 BriefRelay operator plus 08:23 Mercury and Vega cron sessions aborted with `AbortError: agent run aborted` and left no usable transcript closeout.
- Gmail/outreach: `gws` Gmail auth still fails with `invalid_grant`; managed browser remained logged in as `briefrelayops@gmail.com`. Search `in:anywhere newer_than:1d -in:sent -in:drafts` returned no messages, targeted seven-day delivery/bounce search showed only the known internal Matt campaign-review thread and no prospect delivery failure, and spam was empty. No outreach email was sent because no tracker item is eligible today, Batch 5/6 have completed Follow-Up 2, Batch 7 remains under duplicate-send guard, and no replacement prospect batch is approved.
- Instagram: August 3 Monday Lead Stack was published through native Instagram after PNG/JPEG normal upload attempts hit Instagram's "Something went wrong" dialog. Direct CDP `DOM.setFileInputFiles` against only the create-post feed-media input worked. A duplicate post at `https://www.instagram.com/briefrelay/p/DblKV3CEQfo/` was deleted; the kept live post is `https://www.instagram.com/briefrelay/p/DblRDE2kVJB/`. Profile verified at 15 posts with V4D avatar still active.
- Board: local board was updated and served HTTP 200. Branded GitHub Pages was refreshed through the stored `getbriefrelay` GitHub CLI config after Kevin's token proved read-only.
- 10:30 MDT blocker alternatives: pushed the current board to Kevin's admin-access Pages repo `kevinpyles/briefrelay-site`; verified `https://kevinpyles.github.io/briefrelay-site/briefrelay-status.html` serves the August 3 board. Repaired the August 4 Draft With A Seatbelt SVG/PNG clipping and visually checked the regenerated PNG. Reclassified `gws` Gmail `invalid_grant` as non-blocking because managed-browser Gmail is logged in and is the supported operational route until a fresh interactive OAuth login is completed. Reclassified Instagram upload fragility as a default-CDP procedure rather than a blocker.
- 15:45 MDT update: pushed the current board to the branded `getbriefrelay/getbriefrelay.github.io` repo using the stored `getbriefrelay` GitHub CLI config and verified `https://getbriefrelay.github.io/briefrelay-status.html` serves the current board. Updated Google/Gmail profile photo to the V4D avatar; Google accepted the save and the About Me page visually shows the new avatar, with Google's normal one-to-two-day propagation note. Retried `gws auth login --services gmail`; Google OAuth reached account selection, then blocked with `Error 403: access_denied` because the OAuth app named `Slide Deck` has not completed verification and the account is not an approved tester.
- Next action: approve or revise staged Batch 8, then send only within the 10/day cap after the next reply/bounce check.

## 2026-08-04 Operator Note

- Gmail/outreach: managed browser Gmail remained logged in as `briefrelayops@gmail.com`. Last-day non-sent search returned no messages, targeted seven-day delivery/bounce search showed only the known internal Matt campaign-review thread and no prospect delivery failure, and spam was empty. No outreach email was sent because Batch 5/6 are complete through Follow-Up 2, Batch 7 remains under duplicate-send guard, and no replacement prospect batch is approved.
- Instagram: August 4 Draft With A Seatbelt was published through native Instagram CDP feed-media input targeting after the normal upload handoff returned `ok` without attaching media. An older duplicate at `https://www.instagram.com/briefrelay/p/DbnvZ3Fkahc/` was deleted; the kept live post is `https://www.instagram.com/briefrelay/p/Dbnw9XAEa_q/`. Profile verified at 16 posts with the BriefRelay avatar still active.
- Next action: publish August 5 Follow-Up Lot from the prepared queue and approve or revise staged Batch 8 before any new first-touch outreach.

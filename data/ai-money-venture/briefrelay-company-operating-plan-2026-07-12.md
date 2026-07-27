# BriefRelay Company Operating Plan

Updated: 2026-07-27 10:16 MDT  
Owner: Jarvis  
Marketing owner: Mercury  
Design owner: Vega  
Public board: `/Users/jarvis/.openclaw/workspace/briefrelay-status.html`

## Operating Mandate

Kevin expects BriefRelay to move without repeated prompting. Jarvis should review the company, decide the next useful work, execute it, and use the public board as the running status surface. Chat updates should not replace board updates.

## Current Company State

- Offer: missed-lead intake desk for local service businesses.
- Target buyer: local service operators where slow response loses revenue.
- Core pilot: one approved lead source, urgent lead flags, safe reply drafts for approval, follow-up tracking, daily owner brief.
- Price anchor: $750 pilot, with $300-$1,000/month expansion path.
- Public social: Instagram `@briefrelay`, 12 posts live as of 2026-07-27 10:16 MDT; July 25 HVAC Lead Aging Like Milk was recovered and published July 27 at `https://www.instagram.com/briefrelay/p/DbTXhJgkRP6/` after native Instagram CDP feed-media input recovery.
- Public website: V1 static customer site is live on the branded free GitHub Pages URL `https://getbriefrelay.github.io/`; source repo is `https://github.com/getbriefrelay/getbriefrelay.github.io`.
- Brand: Vega V4D / Lead Lift identity, fun-bold BriefRelay guide, buyer-safe humor.
- Marketing: Mercury owns the calendar, copy, content backlog, and email/social campaign improvement.
- Outreach: 75 outbound outreach emails sent as of 2026-07-27 10:16 MDT; July 23 Batch 7 Follow-Up 1 duplicated during browser/session recovery, so five Batch 7 prospects received two follow-up copies and Gmail Sent verified `1-10 of 10`. July 27 Gmail browser checks found no human replies, no targeted bounce/delivery messages, and spam empty. No outreach email was sent because Batch 7 is under duplicate-send guard and the next normal Batch 5/6 follow-up window is July 28; `gws` Gmail auth still fails with `invalid_grant`.
- Board: local and public status page are live, with a 5-minute watchdog for the tunnel/server.

## Audit Findings

1. **Marketing had a plan but not enough ready assets.**  
   The 30-day plan and captions existed, but only July 13 had a rendered post. Fixed by creating a July 14-19 asset batch.

2. **The old V3 brand builder is now unsafe to rerun.**  
   `scripts/build_briefrelay_brand_v3.js` contains stale V3 copy and can overwrite the approved V4D identity. Use `scripts/build_briefrelay_daily_assets.js` for current daily queue assets. Future cleanup should either archive or update the V3 builder.

3. **The board is the right update channel but was stale.**  
   It still showed an older as-of time and did not clearly list the current company projects. Update the board whenever work moves forward or blocks.

4. **Google/Gmail profile photo remains externally blocked.**  
   The asset is ready. The blocker is Google's browser upload dialog not accepting the file handoff. Keep this visible; retry later with a fresh browser path or manual upload route.

5. **Instagram posting is the main execution risk.**  
   Business Suite browser upload is unreliable. The working recovery path is native Instagram web composer with CDP file-input targeting. Prepare the daily asset/caption, try Business Suite once, then use native Instagram CDP upload if Business Suite does not attach media. Target only the create-post media input; the profile page also exposes hidden profile-photo file inputs.

## Active Projects

| Priority | Project | Owner | Next Action | Status |
|---|---|---|---|---|
| P0 | Daily Instagram execution | Jarvis + Mercury + Vega | Use Meta Business Suite first; if upload does not attach, publish through native Instagram web composer using direct CDP against the create-post file input | Active |
| P0 | Board as source of truth | Jarvis | Keep board current; verify tunnel after updates | Active |
| P1 | Email campaign V2 | Mercury + Jarvis | Check deliverability/replies, then send eligible outreach within mandate and caps | Active |
| P1 | Brand asset consistency | Vega + Jarvis | Keep V4D active across board, guide, Instagram; retry Google/Gmail | Active |
| P1 | Brand-forward website URL | Jarvis | Keep `https://getbriefrelay.github.io/` verified and update outreach/CTA links to use it | Active |
| P1 | Reusable content system | Vega + Mercury | Turn daily queue into repeatable templates | Active |
| P2 | Outreach pipeline expansion | Mercury + Jarvis | Build next qualified prospect batch after reply check | Planned |
| P2 | Builder cleanup | Jarvis | Archive/update stale V3 generator to prevent accidental overwrite | Planned |

## Expected Daily Loop

- Check Gmail for human replies, bounces, spam, and account warnings before sending.
- Send eligible outreach emails within Kevin's approved BriefRelay mandate and caps; verify sends in Gmail Sent.
- Publish and verify one Instagram post while BriefRelay is in launch mode; use Meta Business Suite first, then native Instagram CDP upload against the create-post file input if the Business Suite browser handoff fails to attach media.
- Update outreach logs, prospect tracker, Instagram launch log, board, memory, and Obsidian project note after material changes.
- Verify the public board URL after board updates and include the current timestamp, totals, post count, known bounces, and blockers.
- Report the outcome with evidence, or report an exact blocker and next owner/step.

## Operating Rules Going Forward

- Do not wait for Kevin to ask what is next.
- Treat expected daily BriefRelay work as execution: check replies/bounces, send eligible outreach emails, publish and verify the Instagram post, update logs/trackers, update the board, verify the public board URL, and report with evidence.
- Update the board when status changes and before sending internal status emails.
- Every board update must include an accurate "As of" date/time stamp with timezone plus current outreach totals, Instagram post count, known bounces, and blockers.
- Keep the tunnel healthy and watchdog active.
- Prepare at least one post per day while BriefRelay is in launch mode.
- Make humor useful: inbox chaos is the joke, not the owner or customer.
- Do not claim external updates are complete unless verified.
- For Instagram, do not let Business Suite upload failure stall the cadence: after one failed Business Suite attach attempt, use the native Instagram web composer with direct CDP file-input targeting, then verify the live URL and avatar state.

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

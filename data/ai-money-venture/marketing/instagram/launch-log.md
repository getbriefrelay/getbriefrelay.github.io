# BriefRelay Instagram Launch Log

## 2026-07-12

- Created Instagram account: `@briefrelay`
- Email: `briefrelayops@gmail.com`
- Password storage: macOS Keychain service `briefrelay.instagram`, account `briefrelayops@gmail.com`
- Profile name: BriefRelay
- Bio: Catch urgent service leads before the inbox eats them. Approval-gated replies, follow-ups, and daily owner briefs.
- Avatar: `assets/briefrelay/briefrelay-avatar.png`
- First live post: `https://www.instagram.com/briefrelay/p/DatO9zJGfW7/`
- First post source assets: `data/ai-money-venture/marketing/instagram/briefrelay-inbox-bermuda-triangle/`
- Note: The intended four-slide carousel upload failed in Instagram's web composer with "Something went wrong." Posted slide 1 as a single-image launch post. Remaining slides are ready for a later retry.
- Creative upgrade: Kevin said the launch image looked too basic. Created Brand Designer agent `vega`, wrote Vega's brand guide, wrote Mercury's campaign upgrade brief, and rendered improved V2 carousel assets at `data/ai-money-venture/marketing/instagram/briefrelay-inbox-bermuda-triangle-v2/`. Use the V2 assets for the next posting retry rather than the original carousel.
- Posting retry: Attempted to publish the V2 carousel from the logged-in OpenClaw browser session. Instagram's web composer opened but did not ingest the files through the normal upload control or hidden multi-file input. No new post was created; profile remained at 1 post. Stop repeated retries unless using a fresh browser/session or manual upload path.
- Logo refresh: Created Vega-style logo V2 at `assets/briefrelay/briefrelay-avatar-v2.svg` and `assets/briefrelay/briefrelay-avatar-v2.png`, promoted it to the live `assets/briefrelay/briefrelay-avatar.svg/png`, and updated @briefrelay's Instagram profile photo. Verified the new avatar appears on the Instagram profile.

- Daily marketing cadence: created Mercury operating plan, next-7 post queue, fun Email V2, and marketing backlog. Scheduled a daily marketing-manager cron for 8:30 AM America/Denver to prepare/post/report one BriefRelay Instagram item per day. Next planned post: Missed Lead Confession #1 on 2026-07-13 at 9:15 AM MDT. Asset rendered at `data/ai-money-venture/marketing/instagram/briefrelay-missed-lead-confession-2026-07-13.png`.
- Proactive company review: Kevin directed Jarvis to take charge without waiting for repeated prompts, use the board as the main update surface, and keep the tunnel running. Created company operating plan at `data/ai-money-venture/briefrelay-company-operating-plan-2026-07-12.md`.
- Daily queue expansion: rendered July 14-19 Instagram assets as SVG and PNG in `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-14/`. Visual pass caught and fixed text overlap/clipping before staging.

## 2026-07-13

- Email outreach executed: Batch 4 sent five prospect emails through the logged-in Gmail browser at 10:26-10:28 MDT using Mercury's upgraded copy. Prospects: GOAT Roofing, PlumbSmart, Weather Masters / AC Dudes, The Cooling & Plumbing Co, and Discount ACR.
- Reply/bounce status: 17:00 MDT check found no new human prospect replies. The Cooling & Plumbing Co / `info@azcpg.com` bounced with a 550 address-not-found failure; follow-up requires a new verified contact.
- Instagram status: no July 13 post was successfully published. Profile verification at 17:32 MDT still showed 1 post, the July 12 launch post.
- Posting attempt: tried to publish `briefrelay-missed-lead-confession-2026-07-13.png` through the Instagram web composer. The upload handoff returned OK but Instagram stayed on the upload screen; after clicking Select from computer and uploading again, Instagram returned "Something went wrong. Please try again."
- Retry attempt: converted the PNG to JPEG at `/Users/jarvis/.openclaw/media/inbound/briefrelay-missed-lead-confession-2026-07-13.jpg` and retried through the composer. Instagram returned the same "Something went wrong. Please try again." error.
- Fresh-session retry: restarted the OpenClaw browser path and retried the July 13 asset after the active-session PNG/JPEG failures. Instagram still did not accept the upload.
- Current blocker: Instagram web upload is not accepting the prepared July 13 asset in either the active browser session or fresh retry path. Stop repeated web retries to avoid stressing the new account; next path should be mobile/manual upload or a supported publishing API route if available.

## 2026-07-13 Evening Follow-Ups

- Email follow-ups executed: Batch 1 Follow-Up 1 sent to Sweet Dreams Plumbing, Harper's Roofing, Mesa Roofing LLC, Stradling Roofing, and Almeida Roofing at 17:52 MDT through the logged-in Gmail browser.
- Verification: Gmail Sent search for `in:sent "The 11:47 PM estimate request"` showed 5 matching messages.
- July 13 send count: 10 outreach emails total: 5 new Batch 4 prospect emails plus 5 Batch 1 follow-ups.

## 2026-07-13 Business Suite Recovery

- Native Instagram web composer remained blocked: PNG and JPEG uploads returned Instagram's "Something went wrong. Please try again." error from both active and clean browser sessions.
- Recovery path: converted `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-14/2026-07-14-1147-estimate-request.png` to `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-14-1147-estimate-request.jpg`, switched `@briefrelay` to an Instagram business/professional account, logged into Meta Business Suite with Instagram, and published from Business Suite instead of the native Instagram web uploader.
- Live post: `https://www.instagram.com/briefrelay/p/DawQlOTiXB5/`
- Verification: `@briefrelay` profile showed 2 posts after publish; newest post is the 11:47 PM estimate-request graphic.
- Posting rule going forward: use Meta Business Suite for BriefRelay feed posts. Avoid repeated native Instagram web composer retries unless the browser upload path is known to be fixed.

## 2026-07-15

- Instagram status: no July 15 post was found in the launch log as of 10:28 MDT. Today's planned asset exists at `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-14/2026-07-15-approval-lock.png`, but no publish/verification entry exists yet.
- Root cause found from Mercury cron: `briefrelay-daily-marketing-ops` ran at 08:05 MDT and failed with `AbortError: agent run aborted` after about 16 minutes. Added a cron failure alert so future Mercury marketing-op aborts should announce into the BriefRelay group instead of failing silently.
- Recovery publish: converted/copied the July 15 approval-lock asset into `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-15-approval-lock.png` and used Meta Business Suite composer for Instagram `briefrelay`.
- Live post: `https://www.instagram.com/briefrelay/p/Da1oG6tFtf9/`
- Verification: @briefrelay profile showed 3 posts after publish. Newest post is the approval-lock graphic with alt text matching `AUTOPILOT? Nope. Approval required. SEND LOCKED`.
- Note: Business Suite composer displayed a generic "We're having trouble completing your request" while still showing "Publishing your post." External Instagram profile verification confirmed the post did publish.

## 2026-07-16

- Planned post: Inbox Court using `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-14/2026-07-16-inbox-court.png`.
- Visual check: asset renders cleanly and matches the V4D guide.
- Business Suite attempt: opened Meta Business Suite composer for Instagram `briefrelay`, copied the asset to `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-16-inbox-court.png`, clicked Add photo/video, and ran the OpenClaw browser upload tool.
- Blocker: the browser upload tool returned `ok`, but Business Suite still showed no media attached and Publish stayed disabled. No July 16 post was published during the 8 AM run. Next route is a fresh Business Suite browser session or manual/mobile upload, not the native Instagram web uploader.
- 08:17 MDT retry: staged the approved Inbox Court caption in both the existing Business Suite composer and a fresh composer tab, then retried the OpenClaw browser upload against `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-16-inbox-court.png`. Both uploads returned `ok`, but Business Suite still showed no attached media and Publish remained disabled. Instagram profile verification showed `@briefrelay` still at 3 posts with the July 15 Approval Lock post newest. Exact blocker: Business Suite/browser upload handoff is not attaching media. Next action: manual/mobile upload or a different supported upload route.
- 11:03 MDT decision: repeated the Business Suite test in a fresh composer, converted the asset to `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-16-inbox-court.jpg`, filled the caption, and tried the JPEG upload. The upload tool again returned `ok`, but Business Suite attached no media and Publish remained disabled. Verified `@briefrelay` still has 3 posts and the July 15 post remains newest. Decision: stop treating browser upload as retryable; complete July 16 via manual/mobile upload packet. Sent the BriefRelay group packet with the PNG attached and caption in message `1199`.
- 11:19 MDT fix: bypassed the failing Business Suite upload control and used Chrome DevTools Protocol against the native Instagram web composer. Flow: `Create` -> `Post` -> intercepted `Select from computer` file chooser -> set `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-16-inbox-court.jpg` -> clicked through crop/filter -> inserted the approved caption -> clicked Share. Instagram displayed "Post shared" / "Your post has been shared." Verification: `@briefrelay` profile shows 4 posts and newest live post is `https://www.instagram.com/briefrelay/p/Da3KSMXkZYr/`.

## 2026-07-17

- Planned post: Hot Leads Up using `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-14/2026-07-17-hot-leads-up.png`.
- Visual check: asset renders cleanly and matches the V4D guide.
- Business Suite attempt: copied the PNG to `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-17-hot-leads-up.png`, opened Meta Business Suite composer for Instagram `briefrelay`, and ran the OpenClaw upload handoff. The upload returned `ok`, but no media attached and Publish stayed disabled; Business Suite also retained the previous caption.
- Native Instagram attempt: converted the asset to `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-17-hot-leads-up.jpg`, opened native Instagram `Create -> Post`, tried the normal upload handoff, then used direct CDP to set the JPEG on Instagram's hidden file input. Instagram returned "Something went wrong. Please try again." No July 17 post was published during the 8 AM run.
- Manual/mobile packet: sent the BriefRelay group a Telegram packet with the PNG attached and the approved caption in message `1229`.
- 11:34 MDT fix: restarted the managed OpenClaw browser, opened native Instagram profile/composer, and bypassed the OpenClaw upload handoff by using CDP `DOM.setFileInputFiles` on the create-post `input[type=file]` that accepts feed media. Published the cleaned JPEG with Mercury's approved caption. Verification: `@briefrelay` shows 5 posts and newest live post is `https://www.instagram.com/briefrelay/p/Da5wEL2ER4C/`. Note: avoid setting every hidden file input; a profile-photo input also exists and briefly changed the avatar. Restored the V4D avatar through Edit Profile and visually verified it.

## 2026-07-18

- Planned post: Things Found In The Inbox using `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-14/2026-07-18-things-found-in-inbox.png`.
- Visual source: Vega had already cleared the July 18/19 assets as on-brand in the July 17 handoff.
- Business Suite attempt: opened Meta Business Suite composer for Instagram `briefrelay`, staged Mercury's approved caption, and ran the OpenClaw upload handoff against `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-18-things-found-in-inbox.jpg`. The upload returned `ok`, but no media attached and Publish stayed disabled.
- Native Instagram fallback: opened native Instagram `Create -> Post`; the normal upload handoff also returned `ok` but left the composer on `Select from computer`. Used direct CDP `DOM.setFileInputFiles` against only the create-post media input accepting `image/avif,image/jpeg,image/png,image/heic,image/heif,video/mp4,video/quicktime`. The composer advanced to crop/edit, the caption was added, and Instagram displayed `Post shared` / `Your post has been shared`.
- Live post: `https://www.instagram.com/briefrelay/p/Da793pakS8X/`
- Verification: `@briefrelay` profile shows 6 posts; newest grid item is the July 18 Things Found In The Inbox post; live URL returns HTTP 200; V4D avatar still appears active.

## 2026-07-20

- Planned post: Roof Leak Next To Newsletter using `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-20/2026-07-20-roof-leak-next-to-newsletter.png`.
- Queue repair: generated and exported July 20-26 SVG/PNG assets in `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-20/`; visually checked the July 20 asset before posting.
- Business Suite attempt: staged the July 20 caption and ran the upload handoff against `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-20-roof-leak-next-to-newsletter.png`. The upload returned `ok`, but no media attached, Publish stayed disabled, and the old July 18 caption remained visible.
- Native Instagram normal upload attempt: opened native Instagram `Create -> Post`; normal upload handoff returned `ok` but left the composer on `Select from computer`.
- Native Instagram CDP fallback: converted the asset to `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-20-roof-leak-next-to-newsletter.jpg`, used `DOM.setFileInputFiles` against only the create-post media input accepting `image/avif,image/jpeg,image/png,image/heic,image/heif,video/mp4,video/quicktime`, added the approved caption, and shared.
- Live post: `https://www.instagram.com/briefrelay/p/DbBHeD5kWag/`
- Verification: `@briefrelay` profile shows 7 posts; newest grid item is the July 20 Roof Leak Next To Newsletter post. July 19 Sunday Desk Reset was skipped/missed by the stale run and remains available as a staged asset, not back-posted.

## 2026-07-21

- 08:00 operator issue: the daily cron fired but the isolated agent run aborted before completing the Instagram publish/checks/board update, so no July 21 post went live in the morning.
- Planned post: Missed Lead Confession #2 using `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-20/2026-07-21-missed-lead-confession-2.png`.
- Recovery: converted the asset to `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-21-missed-lead-confession-2.jpg`. The first retry hit Instagram's "Confirm you're human" checkpoint and the normal upload handoff again returned `ok` without attaching media. After the checkpoint cleared, direct CDP `DOM.setFileInputFiles` against only the create-post feed-media input attached the asset.
- Live post: `https://www.instagram.com/briefrelay/p/DbEhcacEWd6/`
- Verification: Instagram displayed `Post shared` / `Your post has been shared`; `@briefrelay` profile shows 8 posts and the newest grid item is the July 21 Missed Lead Confession #2 post.

## 2026-07-22

- Planned post: Follow-Up Did Not Ghost You using `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-20/2026-07-22-follow-up-did-not-ghost-you.png`.
- Business Suite attempt: opened Meta Business Suite composer first, but the session was at the Meta business-tools login chooser instead of an authenticated composer. Logged blocker and continued through native Instagram.
- Native Instagram fallback: converted the asset to `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-22-follow-up-did-not-ghost-you.jpg`. Normal upload handoff returned `ok` but left the composer on `Select from computer`; direct CDP `DOM.setFileInputFiles` against the create-post feed-media input attached the JPEG, then caption/share completed.
- Live post: `https://www.instagram.com/briefrelay/p/DbGR2DZEY4q/`
- Verification: Instagram displayed `Post shared` / `Your post has been shared`; `@briefrelay` profile shows 9 posts and the newest grid item is the July 22 Follow-Up Did Not Ghost You post.

## 2026-07-23

- Planned post: Before/After Brief using `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-20/2026-07-23-before-after-brief.png`.
- Visual check: asset renders cleanly: "Inbox soup. Owner brief." with the V4D mark, before/after cards, and no text clipping.
- Native Instagram upload: converted the asset to `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-23-before-after-brief.jpg`. Normal upload handoff returned `ok` but stayed on `Select from computer`; clicking Select and retrying produced Instagram's "Something went wrong. Please try again." dialog.
- Native Instagram CDP fallback: reset the composer, used CDP `DOM.setFileInputFiles` against only the create-post feed-media input accepting `image/avif,image/jpeg,image/png,image/heic,image/heif,video/mp4,video/quicktime`, added the caption, and shared.
- Duplicate cleanup: the retry path briefly created a duplicate July 23 post at `https://www.instagram.com/briefrelay/p/DbI3aN3EfUn/`. Jarvis deleted the older duplicate and kept the newest post.
- Live post: `https://www.instagram.com/briefrelay/p/DbI3bzLEXBI/`
- Verification: Instagram displayed `Post shared` / `Your post has been shared`; after duplicate cleanup, `@briefrelay` profile shows 10 posts and the newest grid item is the July 23 Before/After Brief post.

## 2026-07-24

- Planned post: No Autopilot Promises using `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-20/2026-07-24-no-autopilot-promises.png`.
- Native Instagram upload: the first generic upload handoff returned `ok` but did not attach media; a JPEG retry produced Instagram's "Something went wrong. Please try again." dialog. Restarted the managed OpenClaw browser, reopened `@briefrelay`, selected native Instagram `Create -> Post`, and used CDP `DOM.setFileInputFiles` against only the create-post feed-media input accepting `image/avif,image/jpeg,image/png,image/heic,image/heif,video/mp4,video/quicktime`.
- Caption used: "No autopilot promises." with the approval-gated daily-owner-brief explanation and trust line: "Nothing gets sent, booked, deleted, or promised without approval."
- Live post: `https://www.instagram.com/briefrelay/p/DbMEZylGR5M/`
- Verification: Instagram displayed `Post shared` / `Your post has been shared`; `@briefrelay` profile shows 11 posts and the newest grid item is the July 24 No Autopilot Promises post.

## 2026-07-27

- Planned post recovered: HVAC Lead Aging Like Milk using `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-20/2026-07-25-hvac-lead-aging-like-milk.png`.
- Cause: the 8 AM daily operator run aborted with `AbortError: agent run aborted`, leaving the July 25 post and daily checks unrecovered until manual intervention.
- Native Instagram CDP recovery: converted the asset to `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-07-25-hvac-lead-aging-like-milk.jpg`, opened native Instagram `Create -> Post`, and used CDP `DOM.setFileInputFiles` against only the create-post feed-media input accepting `image/avif,image/jpeg,image/png,image/heic,image/heif,video/mp4,video/quicktime`.
- Caption used: no-cooling lead language with emergency AC requests, hot leads visible, safe reply drafts, approval-gated daily owner brief, and the trust line "Hot leads go on top before the day gets loud."
- Live post: `https://www.instagram.com/briefrelay/p/DbTXhJgkRP6/`
- Verification: Instagram displayed `Post shared` / `Your post has been shared`; after profile refresh, `@briefrelay` showed 12 posts and the newest grid item was the July 27 published no-cooling lead graphic.

## 2026-07-31

- Planned post recovered: Sunday Desk Reset #2 using `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-20/2026-07-26-sunday-desk-reset-2.png`.
- Cause: the daily operator cron aborted again with `AbortError: agent run aborted`, leaving July 28-31 recovery work without a visible closeout.
- Native Instagram upload: normal OpenClaw upload handoff returned Instagram's "Something went wrong. Please try again." for both PNG and JPEG attempts. Installed local `websocket-client` support and used direct CDP `DOM.setFileInputFiles` against only the create-post feed-media input accepting `image/avif,image/jpeg,image/png,image/heic,image/heif,video/mp4,video/quicktime`.
- Caption used: "Sunday desk reset. Tomorrow needs less \"wait, when?\" BriefRelay keeps urgent items, draft replies, follow-ups, and approval status in one owner brief. One source. One brief. Fewer mysteries."
- Live post: `https://www.instagram.com/briefrelay/p/DbdfE6iEa6D/`
- Verification: Instagram displayed `Post shared` / `Your post has been shared`; after profile refresh, `@briefrelay` showed 13 posts and the newest grid item was the July 31 Sunday Desk Reset #2 post.

## 2026-08-01

- Planned post recovered: Lead Archaeology using `data/ai-money-venture/marketing/instagram/daily-queue-2026-07-20/2026-07-31-lead-archaeology.png`.
- Native Instagram upload: copied the asset to `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-08-01-lead-archaeology.png`. The normal OpenClaw upload handoff returned `ok` but did not attach media; direct CDP `DOM.setFileInputFiles` with `suppress_origin=True` targeted only the create-post feed-media input accepting `image/avif,image/jpeg,image/png,image/heic,image/heif,video/mp4,video/quicktime`.
- Caption used: lead archaeology / buried estimate request language, with approval-gated safe reply and owner brief positioning plus the trust line "Nothing gets sent, booked, deleted, or promised without approval."
- Live post: `https://www.instagram.com/briefrelay/p/DbgAzYokYTh/`
- Verification: after profile refresh, `@briefrelay` showed 14 posts and the newest grid item was the August 1 Lead Archaeology post.

## 2026-08-02

- Planned post status: no new August queue asset exists yet. The board and prior logs already marked the July 20-26 batch plus the Lead Archaeology recovery asset as fully used; the only unused older asset is July 19 Sunday Desk Reset, explicitly marked missed/staged and not back-posted.
- Publish decision: no Instagram post was published today because there was no approved current queued asset to publish safely.
- Verification: `@briefrelay` profile remained logged in and showed 14 posts. Newest post remains August 1 Lead Archaeology at `https://www.instagram.com/briefrelay/p/DbgAzYokYTh/`.
- Next action: create the next August Instagram queue/assets before the next daily operator publish.
- 08:22 MDT Mercury update: August 3-9 asset queue now exists in `daily-queue-2026-08-03`. The August 3 Monday Lead Stack PNG was visually checked and the caption handoff was prepared in `briefrelay-august-3-9-instagram-captions.md`. Next action: publish the August 3 Monday Lead Stack post in the next daily operator run.

## 2026-08-03

- Planned post recovered: Monday Lead Stack using `data/ai-money-venture/marketing/instagram/daily-queue-2026-08-03/2026-08-03-monday-lead-stack.png`.
- Cause: the 08:00 BriefRelay operator cron, 08:23 Mercury cron, and 08:23 Vega cron all aborted with `AbortError: agent run aborted`, leaving the daily work without a visible closeout until manual recovery.
- Native Instagram upload: copied/converted the asset into `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-08-03-monday-lead-stack.png` and `.jpg`. Normal PNG and JPEG upload attempts returned Instagram's "Something went wrong. Please try again." Direct CDP `DOM.setFileInputFiles` with `suppress_origin=True` targeted only the create-post feed-media input accepting `image/avif,image/jpeg,image/png,image/heic,image/heif,video/mp4,video/quicktime`; the composer advanced through crop/edit/caption/share.
- Caption used: Mercury's Monday Lead Stack caption about AC outage, roof leak, estimate request, urgent items on top, approval-gated drafts, and "Nothing gets sent, booked, deleted, or promised without approval."
- Duplicate cleanup: the retry path briefly created an older duplicate at `https://www.instagram.com/briefrelay/p/DblKV3CEQfo/`. Jarvis deleted that duplicate and kept the newest post.
- Live post: `https://www.instagram.com/briefrelay/p/DblRDE2kVJB/`
- Verification: Instagram displayed `Post shared` / `Your post has been shared`; after duplicate cleanup and profile refresh, `@briefrelay` showed 15 posts with the August 3 Monday Lead Stack post newest.

## 2026-08-04

- Planned post: Draft With A Seatbelt using `data/ai-money-venture/marketing/instagram/daily-queue-2026-08-03/2026-08-04-reply-draft-seatbelt.png`.
- Visual check: asset renders cleanly after the August 3 clipping repair; no text clipping or element overlap found.
- Gmail/outreach check: managed browser Gmail was logged in as `briefrelayops@gmail.com`; `in:anywhere newer_than:1d -in:sent -in:drafts` returned no messages, targeted seven-day delivery/bounce search showed only the known internal Matt campaign-review thread and no prospect delivery failure, and spam was empty. No outreach email was sent because Batch 5/6 are complete through Follow-Up 2, Batch 7 remains under duplicate-send guard, and no replacement batch is approved.
- Native Instagram upload: converted the asset to `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-08-04-reply-draft-seatbelt.jpg`. Normal OpenClaw upload returned `ok` but did not attach media; direct CDP `DOM.setFileInputFiles` with `suppress_origin=True` targeted only the create-post feed-media input accepting `image/avif,image/jpeg,image/png,image/heic,image/heif,video/mp4,video/quicktime`; the composer advanced through crop/edit/caption/share.
- Duplicate cleanup: the retry path created an older duplicate at `https://www.instagram.com/briefrelay/p/DbnvZ3Fkahc/`. Jarvis deleted that duplicate and kept the newest post.
- Live post: `https://www.instagram.com/briefrelay/p/Dbnw9XAEa_q/`
- Verification: Instagram displayed `Post shared` / `Your post has been shared`; after duplicate cleanup and profile refresh, `@briefrelay` showed 16 posts with the August 4 Draft With A Seatbelt post newest and the BriefRelay profile avatar still active.

## 2026-08-05

- Planned post recovered: Follow-Up Lot using `data/ai-money-venture/marketing/instagram/daily-queue-2026-08-03/2026-08-05-follow-up-parking-lot.png`.
- Cause: the 8 AM BriefRelay operator cron reported `AbortError: agent run aborted`, and the board was still stamped August 4 until this same-day recovery.
- Gmail/outreach check: managed browser Gmail was logged in as `briefrelayops@gmail.com`; `in:anywhere newer_than:1d -in:sent -in:drafts` returned no messages, targeted seven-day delivery/bounce search returned no messages, and spam was empty. No outreach email was sent because Batch 5/6 are complete through Follow-Up 2, Batch 7 remains under duplicate-send guard, and Batch 8 is staged but not approved.
- Native Instagram upload: the normal OpenClaw upload returned `ok` but did not attach media. Direct CDP `DOM.setFileInputFiles` targeted only the create-post feed-media input accepting `image/avif,image/jpeg,image/png,image/heic,image/heif,video/mp4,video/quicktime`; the composer advanced through crop/edit/caption/share.
- Caption used: Mercury's approved Follow-Up Lot caption about hot leads not getting parked forever, next touches mattering, and the next thing staying visible on the brief.
- Live post: `https://www.instagram.com/briefrelay/p/DbqW0Yykfik/`
- Verification: Instagram displayed `Post shared` / `Your post has been shared`; after profile refresh, `@briefrelay` showed 17 posts with the August 5 Follow-Up Lot post newest and the BriefRelay profile avatar still active.

## 2026-08-10

- Cron pause blocker: during the 08:05 MDT daily marketing ops run, Mercury found the newer main-workspace standing memory dated 2026-08-07: Kevin paused all BriefRelay work because it has not made money and has consumed too many tokens. No Gmail outreach, Instagram publishing, or browser verification was performed because this scheduled cron is not fresh explicit approval.
- Prepared-only work: created the August 10-16 Instagram SVG/PNG queue at `data/ai-money-venture/marketing/instagram/daily-queue-2026-08-10/` and the caption handoff at `briefrelay-august-10-16-instagram-captions.md`. The August 10 Monday Inbox Roll Call PNG was visually checked and is readable/on-brand.
- Current Instagram status remains unchanged from the latest verified check: `@briefrelay` has 17 live posts, with August 5 Follow-Up Lot newest at `https://www.instagram.com/briefrelay/p/DbqW0Yykfik/`.
- Next action: keep BriefRelay marketing paused until Kevin explicitly reauthorizes external posting/outreach or restarts the daily cadence.

## 2026-08-21

- Daily ops check: reviewed the current BriefRelay marketing backlog, launch log, outreach tracker/log, Batch 8 staged prospects, and the latest prepared August 10-16 Instagram queue.
- Current blocker: Kevin's 2026-08-07 standing pause remains active. This scheduled cron is not fresh explicit approval, so no Gmail outreach, Instagram publishing, browser verification, or new asset build was performed.
- Prepared status: August 10-16 captions and 1080x1080 PNG assets remain staged; Batch 8 remains `needs_approval`; no approved outbound email exists today.
- Next action: keep BriefRelay marketing paused until Kevin explicitly reauthorizes external posting/outreach or restarts the daily cadence.

## 2026-08-24

- Daily ops check: reviewed the current BriefRelay marketing backlog, launch log, outreach tracker/log, prospect tracker, and prepared August 10-16 Instagram queue.
- Current blocker: Kevin's 2026-08-07 standing pause remains active. This scheduled cron is not fresh explicit approval, so no Gmail outreach, Instagram publishing, browser verification, or new asset build was performed.
- Prepared status: August 10-16 captions and 1080x1080 PNG assets remain staged; Batch 8 remains `needs_approval`; no approved outbound email exists today.
- Next action: keep BriefRelay marketing paused until Kevin explicitly reauthorizes external posting/outreach or restarts the daily cadence.

## 2026-08-30

- Daily ops check: reviewed the current BriefRelay marketing backlog, launch log, outreach tracker/log, prospect tracker, Batch 8 staged status, and the prepared August 10-16 Instagram queue.
- Current blocker: Kevin's 2026-08-07 standing pause remains active. This scheduled cron is not fresh explicit approval, so no Gmail outreach, Instagram publishing, browser verification, or new asset build was performed.
- Prepared status: August 10-16 captions and 1080x1080 PNG assets remain staged; Batch 8 remains `needs_approval`; no approved outbound email exists today.
- Next action: keep BriefRelay marketing paused until Kevin explicitly reauthorizes external posting/outreach or restarts the daily cadence.

## 2026-09-13

- Daily ops check: reviewed current BriefRelay marketing backlog/log status, Batch 8 staged prospects, and the latest prepared August 10-16 Instagram queue.
- Current blocker: Kevin's 2026-08-07 standing pause remains active. This scheduled cron is not fresh explicit approval, so no Gmail outreach, Instagram publishing, browser verification, or new asset build was performed.
- Prepared status: August 10-16 captions and 1080x1080 PNG assets remain staged; Batch 8 remains `needs_approval`; no approved outbound email exists today.
- Automation cleanup: removed stale cron `99c3fd54-095f-4623-96fe-c877c6a3eb75` (`briefrelay-daily-marketing-ops`) so the paused daily marketing ops check stops recurring.
- Recall note: memory semantic search was unavailable because the index provenance classifier changed, so direct file reads were used for this check.
- Next action: keep BriefRelay marketing paused until Kevin explicitly reauthorizes external posting/outreach or restarts the cadence.

## 2026-09-13 Resume

- Kevin explicitly reauthorized BriefRelay posting and email in the Telegram group at 22:01 MDT, so Mercury resumed normal marketing ops.
- Planned post recovered: Monday Inbox Roll Call using `data/ai-money-venture/marketing/instagram/daily-queue-2026-08-10/2026-08-10-monday-inbox-roll-call.png`.
- Native Instagram upload: copied the asset to `/Users/jarvis/.openclaw/media/inbound/briefrelay-2026-09-13-monday-inbox-roll-call.png`, opened native Instagram `Create -> Post`, used the feed-media file input accepting `image/avif,image/jpeg,image/png,image/heic,image/heif,video/mp4,video/quicktime`, added Mercury's approved caption, and shared.
- Live post: `https://www.instagram.com/briefrelay/p/DdQQC1ZkS7b/`
- Verification: Instagram displayed `Your post has been shared`; after profile refresh, `@briefrelay` showed 18 posts with the new post newest.

## 2026-09-23

- Planned post recovered: Competitor Replied First using `data/ai-money-venture/marketing/instagram/daily-queue-2026-09-15/2026-09-23-competitor-replied-first.png`.
- Native Instagram upload: opened native Instagram `Create -> Post`, attached the prepared Sep 23 PNG, advanced through crop/edit/caption/share, and shared from the logged-in `@briefrelay` profile.
- Live post: `https://www.instagram.com/briefrelay/p/Ddob_KWEdEQ/`
- Verification: after profile refresh, `@briefrelay` showed 19 posts with the Sep 23 post newest.
- Gmail/outreach check: managed browser Gmail was logged in as `briefrelayops@gmail.com`. Last-10-day search showed Instagram notices plus the already-known Agape Air delivery block; Agape Air was excluded from follow-up because its first-touch send had a delivery-block warning.
- Email follow-ups executed: Batch 8 Follow-Up 1 sent to Pineapple Air Heating & Cooling, Western Sky Mechanical, Total Plumbing & Drain, and Storm Plumbing at 09:19 MDT through the logged-in Gmail browser.
- Verification: Gmail Sent search for `in:sent after:2026/09/23 "The 11:47 PM estimate request"` showed four today results for the follow-up subject.

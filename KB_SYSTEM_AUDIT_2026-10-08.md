---
type: report
title: "KB + Skills + CRM + Video System Audit — 8 October 2026"
description: "Deep audit of the whole operating system: structure, learning loop, routing clarity, private-vs-show separation, the 44_Gigs CRM, the creative and video pipeline, the skill layer, routines and plans. Run from a cloud session reading Drive via the connector; four parallel agents covered 44_Gigs, 05_Creative + hans-video, folders 00–08 + 90, and 80_project_files + Claude code + 99_Skills."
tags: [audit, kb, skills, crm, video, meta]
visibility: internal
updated: 2026-10-08
---

# KB + Skills + CRM + Video System Audit — 8 Oct 2026

**How to read this.** Section 1 is the verdict. Section 2 answers Hans's direct questions. Section 3 is the scorecard. Section 4 is the evidence per area. Section 5 is the ordered to-do list. Section 6 is what could not be verified. Everything here was read, not assumed; items marked UNVERIFIED were not reachable from Drive.

**Method.** Read from a claude.ai cloud session via the Google Drive connector (read-only). Roughly 250 Markdown files read in full, every folder fully listed, plus the 37 skills installed in the claude.ai account (local to the session). Previous audit for comparison: `_archive/KB_SYSTEM_AUDIT_2026-07-06.md`.

---

## 1. Verdict

The design is right and unusually mature for a one-person business: a canon layer (North Star → priorities → plan), a KB with one-home-per-fact rules, skills as the operating layer, a file-based CRM with a follow-up queue, scheduled routines judged by their artifacts, and a decisions log. The July audit's conclusion ("no restructure needed") still holds. **Confidence: high.**

The problem is not structure. It is three things:

1. **The learning does not travel.** Rules get added on the Mac (skills, CRM README, hans-video LEARNINGS) but the skills installed in the claude.ai account, which cloud, web and phone sessions run, are the **June 2026 versions**. `hans-copywriting` here is v1.0 without the 6 July "Offer & Pitch Lab"; `anti-ai-writing` lacks the July REWRITE mode; `hans-training` is frozen at 22 June with "recalibrate after the 2 July lab test" still pending. Meanwhile 29 of 35 skill mirrors in `99_Skills/` predate September. This, plus skills that fetch their brain from a Mac-only path, is why the assistant is "sometimes missing info" off the Mac.
2. **The system generates more than it prunes.** The gigs ledger was reformatted on 4 Aug because it was unreadable at 30 KB; it is 165 KB today. The reference files that skills must read are 145–350 KB and now contain daily "0 KEPT" digest logs. The ⏰ queue holds ~55 rows, roughly half of them closed. Hans deleted 10 of the last 13 sweep-generated drafts. The decisions log took ~200 entries in 5.5 weeks.
3. **Private data has leaked into business files**, and two live credentials sit in the KB in plaintext.

Nothing here is broken. All eight Claude routines that write to Drive are alive as of this morning. The CRM caught a new lead today. The video pipeline shipped a teaser (v11) and three showreels in the last four days. The fix is maintenance and propagation, not a rebuild.

---

## 2. Hans's questions, answered

### "Is it set up the best way?"
Yes, for the structure. The three-layer split (canon / KB facts / skills for process) matches what every serious practitioner recommends and what the previous audit confirmed. What is not best-in-class: the skill layer is split between "fat" skills that carry their own knowledge (write-like-hans 98 KB, hans-training, hans-website, hans-copywriting) and "thin loader" skills that are 40–60 lines pointing at a Mac path (`hans-show`, `hans-ai-systems`, `hans-marketing`, `magic-consult`). Off the Mac, the thin ones are nearly empty. That is an inconsistent design, and it costs you exactly where you noticed it. Confidence: high.

### "Is it learning?"
Partly, and in the right places. Real learning, with evidence:
- `44_Gigs/README.md` rules 7–18 are each dated to a mistake (missed loss for 3 days → rule 7; scheduled sends mistaken for deleted drafts → rule 9; your "if I delete a draft it's because I don't think it's needed" → rule 18, 5 Oct).
- `hans-video/LEARNINGS.md`: 15 dated rule blocks in five days, mostly your words.
- `write-like-hans`: every correction extracted as a dated rule (12 Jul, 28 Jul, 4 Aug entries).
- Decisions log: appended through 8 Oct.

Not learning, or learning into the void:
- The external-input loop has collapsed. Creator digests run daily (116 files, 7 Jun → 8 Oct) but the keep-rate went from 13 kept in August to 1 in October, and the zero-days are logged *into* the reference files. `90_Learning/CATALOG.md` last entry 21 Jun; `Hans_Nuggets.md` entries only 21–29 Jun. Whether the Nugget Inbox note has had anything to sort since June: UNVERIFIED (Apple Notes not reachable). Either the inbox is empty or the sorter stopped. Check the artifact.
- The learning stays on the Mac (see §1).

### "Is it clear where things belong and how it runs?"
The rules are clear and written down (`_START_HERE`, `_KB_STANDARDS`, the three-way routing test in `update-knowledge-base`, the routines registry). Practice has drifted:
- Four running orders exist for the Season 5 show (BML_2026_Show_Script, Routine_Database, Clever_Hans_Script_Drafts, two archive scripts), none marked "as performed".
- Two chatbot sources of truth (`01_BML/Chatbot_KB.md` says it is canonical; `08_Resources/Bot_Knowledge/bml.md` is what the bot uses).
- Three deposit/invoice policies for Norway across Pricing_Master, Proposal_Template and Contracts/_README (the Contracts one, 24 Aug, is the real standard).
- `Pricing_Master.md` claims single source of truth but omits julebord, team-building and villa add-ons, and `Pricing_Tiers.md` contradicts it on four numbers.
- READMEs for 01, 03, 04, 06, 07 are out of date; 06 says "empty" (holds two invoices), 07 says "none yet" (holds ~13 items).
- `_INBOX/` has 10 files, some used 3–4 Oct and never filed, oldest from 2018.
- `ACTION_PRIORITIES.md`, the declared canonical hub, has no September or October block. Its live block is "AUGUST STACK"; it still says BML is off-season and Norway ads are paused. Season 6 went on sale 1 Oct and Norway ads have run since 16 Jul.

### "Does it understand the difference between private and show work?"
The rule exists (07_Personal is private; family off public bios; visibility frontmatter). Enforcement is leaky:
- The twins (unannounced, due Feb/Mar 2027) appear in ~6 creative files, the O2 residency file, two client files, the ledger, and `01_BML/Schedule_and_Season.md`, which is tagged **public-ok**.
- `44_Gigs/clients/sakine-blakseth.md` carries Nikki's travel dates; `tromso-kommune.md` records where you sleep privately in Tromsø. Sweep reports list your personal purchases (Apple, Strava, Hertz, SAS booking refs) under "not gigs".
- `05_Creative/Footage_Library/MAC_INDEX.md` lists folder paths for IVF, Tessa medical, school, will and codicil, marriage certificate. `Claude code/catalog/inbox_2026-10/` holds a 17,071-row private photo sort log and a 1 MB OCR dump of 11,453 personal photos (contents UNVERIFIED). Family first names are hard-coded in `catalog_drive.py` and replicated in 13+ archive snapshots.
- Visibility enum is inconsistent (`public-draft`, `internal-secret`, `private` all in use); `Race_and_PB_History` is `internal`, not private; `Chatbot_KB` frontmatter says internal, body says PUBLIC.
- Unresolved contradiction: hans-video QC gate says "family never on screen in public content", while its own performance data names the dad-joke reels with Nikki and Granny as the best-held format. Needs one ruling from you.

Family material in `05_Creative` as show clay is fine and by your rule. The index files and catalogue logs are not show clay.

### "Is the CRM set up properly? Does it log contacts and prompt future work?"
**Design: yes.** Ledger dashboard (⚡ WAITING ON HANS ≤10 rows, ⏰ queue with Prompt ≈ Send − 1 month, pipeline/won/lost), one file per client with exact offers and why-lost, 2 scheduled touches per gig (day-of well-wish via Gmail Schedule Send; win-back at the earlier of contact+10 months / gig+9 months), ghostbuster ladder, invoice-timing rule, 44 client files, 5 templates. Running: `CRM_RUN_LOG` shows 05:15–05:31 full and 13:12 quick runs every day since 5 Oct; ledger and client files modified today.

**Logging:** strong on email (thread IDs, timestamps, quotes). Weak on phone and Cal.com calls: Lilia 14 Sep, Osloguide, Anastasia, Deme — outcome never logged. Three client files contradict the ledger (`gabrielle-wadman` "open" vs lost 7 Jul; `hunton` header "open" vs lost 15 Sep; Sakine invoice "paid 8 Oct" in one table, "not registered paid" in two others, same file). O2 show date 16 Nov in the ledger's recurring table, 9 Nov everywhere else.

**Prompting future work:** the mechanism works and has produced results (31 Aug win-back batch → 4 clean no's with named owners; the Cisco tier-2 mail "shook the answer loose in two hours after five months"). ~55 ⏰ rows with win-backs dated Jan–Aug 2027. But the 10-month rule has never fired yet (earliest 2027), the 17 Sep review found 0 of 13 lost dated gigs had day-of rows (three missed for good), and you deleted 10 of the last 13 generated drafts. The engine over-produces relative to what you will send.

**Overdue on your side today (≈130k NOK):** Tromsø kommune contract/invoice (Siv quiet since 8 Sep, deadline 1 Oct), Sjøentreprenøren 43k invoice "planned 25 Sep, not seen sent", Deme Offshore offer (budget approved 9 Sep, deadline 25 Sep, not written). Plus Repstad signed 8 Sep, still awaiting your "ok" to move to Confirmed.

### "Grok bots, one job per bot, talking like a team — are we set up wrong?"
It is a false choice, and you are already using both models.

- **Skills = hats on one agent.** Right for interactive work: one context, one voice, the whole KB in reach. Cost: one context window, so if the hat points at a 350 KB file the agent skims and misses things.
- **Separate agents = separate context windows.** Claude Code has this: subagents (this audit ran four in parallel, each reading a different part of Drive), custom agent definitions in `.claude/agents/`, and scheduled tasks. Your `crm`, `kb-intake`, `weekly-ads`, `weekly-website` tasks *are* one-job bots. The accounting plan written today adds an accountant.
- **"They talk to each other like a human team"** is mostly theatre. What actually makes a bot team work is shared memory, and that is your KB. The CRM writes the ledger; `/status` reads it; the heartbeat checks artifacts. That is the team talking. The weak point is the same as above: bots write into shared files and nobody prunes.

So: no, you are not set up worse than the one-bot-per-job model. You are set up like it for routines and like a single assistant with hats for live work, which is the right split. The two real gaps are (a) the hats are stale off the Mac and (b) no bot owns pruning. Confidence: high on the architecture point; moderate on how Grok's product actually behaves (I have not used it and will not claim specifics).

### "Why are you sometimes missing info?"
Three concrete mechanisms, all verified:
1. **Stale installed skills** (June versions in the claude.ai account; live edits only on the Mac). Evidence: `manifest.json` dates; v1.0 header and no Pitch Lab in the installed hans-copywriting; `99_Skills` mirror dates.
2. **Thin skills fetch their brain from `/Users/Macbook/...`.** Off the Mac that path does not exist and the Drive-ID fallback is forbidden by the skill text itself ("do NOT rely on Google Drive file IDs"). `hans-show` without `Show_Reference.md` + `Comedy_Writing.md` is a 56-line rule list.
3. **Duplicated facts with different values** (discount codes in 6 files with 3 different percentages; four running orders; two chatbot masters). Which one gets read is luck.

### "Video cataloguing and editing: is it functioning? Have you learnt all you need?"
**Functioning, and fast.** Evidence from 4–8 Oct: 1,882 videos / 397 h / 4.7 TB indexed (`FOOTAGE_INDEX.md` + 4 CSVs); 119 BML shows laugh-scanned, 542 moment clips cut; 70 at-risk shows transcribed (`batch.log` ends "ALL DONE") and 344 reaction clips cut by cue-line regex; teaser v1→v11 published 5 Oct to IG, FB, YouTube, TikTok and the BML homepage; two S6 clips scheduled 6 Oct; three showreels v1 rendered 7 Oct (v2 waiting on you and a licensed voice). Tooling is free and on the Mac: ffmpeg 9, faster-whisper, custom `laughscan.py`, `cut_moments.py`, `cut_reactions.py`, `reelcut.py`, `transcribe.py`, showreel engine, QC gate with consent and loudness rules.

**No new skill is needed.** `hans-video` already has a taste model (15 LEARNINGS rules + teardown of your 156 past reels + photo taste model), clip-selection criteria, consent rules, a music licence log and the backup plan. What is missing is four reference files and some housekeeping:
1. **A clip-level register in Drive.** The only index of 886 clips is two CSVs (`_moments.csv`, `_reactions.csv`) on the HG-4TB disk, which has 27 GB free and no second copy. Columns needed: routine, season, volunteer-visible, consent, tier, used-in.
2. **A routine cue-line bank** per season, mined from the 47 archived scripts. Cue regexes were improvised per session; 16 of 70 nights produced zero reaction clips because no cues existed for their routines.
3. **A consent register with evidence** (night, volunteer, asked by whom; a photo of the door notice; the Fienta line). Clips with volunteers are already scheduled; the rules exist, the record does not. Norway: Åndsverkloven § 104 clause per gig.
4. **A show-night capture SOP** as one checklist (4K, clean mic feed, a phone on the audience's faces). Every benchmark in your own files says faces are the product; the archive camera sits behind the audience.

Tooling gaps, honestly stated: the agent cannot watch video. No scene detection, no face or pose tracking, no visual-quality scoring for video (the photo cataloguer has blur and brightness; the video one does not). Norwegian transcription (nb-whisper) is researched but not installed, so Lean Konferansen (18.5 GB) has no transcript. These are medium-to-large and only worth it after the four files above.

Also stale: `FOOTAGE_INDEX.md` not regenerated since 4 Oct although 9 shows were deleted and 58 are being shrunk; `_STATUS.md` still shows v8–v10 "waiting on notes" after v11 shipped; `02_Villa_Shows/Video_Pipeline.md` (June, "for your video guy") is superseded and not cross-linked.

### "What is the best way to organise my work, now and for the future?"
Keep the structure. Change three habits and one piece of plumbing.

**Habits**
1. **Prune is a job, not a hope.** Give one routine (the heartbeat, or a new `weekly-prune` Sunday task) explicit pruning rules: closed ⏰ rows → client file; sweep reports → `CRM_RUN_LOG`; "0 KEPT" digest days → `_digest_archive` roll-up; reference files capped at ~60 KB with the overflow in a dated appendix. Without this the September pattern repeats every two months.
2. **Monthly stack, written.** `ACTION_PRIORITIES.md` gets a dated block on the 1st, and the contradicted lines get struck the same day. Today it is two months stale and says the opposite of reality on two money levers.
3. **One ruling per contradiction, logged.** The audit found ~15 (list in §4). Each needs one line from you, then the losing copies become pointers.

**Plumbing: make the KB reachable off the Mac.** Everything that goes wrong off the Mac traces to the KB being a Mac path. Two options, in order of my preference:
- **(a) Mirror the KB text to a private GitHub repo, nightly, from the Mac.** One scheduled task: `rsync` the `.md`/`.csv`/`.json` (no media, no `99_Skills` zips) into a repo and push. Cloud and phone sessions then read the whole KB natively, can search it, and can propose edits as commits that the Mac pulls in the morning. Drive stays the home; the repo is a read mirror plus an inbox for off-Mac edits. Effort: medium (one script, one routine, one registry row). Risk: a credential on the Mac for the push; keep media out. Confidence that this fixes the off-Mac gap: high.
- **(b) Make the thin skills fat.** Fold `Show_Reference` + `Comedy_Writing` into `hans-show`; fold the TJ Robertson summary into `hans-ai-systems` or retire that skill; give `magic-consult` the library index inline. Then re-upload every custom skill once, and add "re-upload after edit" to the skill update protocol. Effort: medium, and it has to be repeated on every edit. Do this for `hans-show` regardless; it is the one that matters most and it is 56 lines today.

For the future (twins Feb/Mar 2027, less time): the system should run on artifacts you glance at, not drafts you delete. Shrink what it produces (one monthly win-back list to pick from, not 9 drafts; day-of only for corporate), keep the heartbeat honest, and let the accounting bot and the CRM bot be the two things that run unattended.

---

## 3. Scorecard

| Area | Score | One line |
|---|---|---|
| Structure / folder design | 9/10 | Right model; no restructure. |
| Routing clarity (where things belong) | 6/10 | Rules clear; ~15 live contradictions; 5 stale READMEs. |
| Learning loop | 5/10 | Learns well in skills/CRM rules; external intake collapsed; learning does not reach cloud/phone. |
| Private vs show separation | 4/10 | Rule exists; twins in a public-ok file; IVF/medical/will paths and 17k private photo rows inside the KB; two plaintext tokens. |
| CRM design | 9/10 | Best part of the system. |
| CRM hygiene | 5/10 | Ledger 5× its August size; closed rows retained; 3 contradictions; phone outcomes unlogged. |
| CRM output vs what Hans sends | 4/10 | 10 of last 13 drafts deleted; 3 money items overdue on Hans. |
| Creative KB | 6/10 | Current, but 4 running orders, S6 naming split, README omits 8 subfolders. |
| Video pipeline | 8/10 | Working and fast; one disk, no backup of the clip index; 4 reference files missing. |
| Skills (content) | 8/10 | Strong, well-gated. |
| Skills (propagation) | 3/10 | June versions everywhere except the Mac; 29/35 mirrors pre-September. |
| Routines | 7/10 | 8/8 Drive-writing routines alive; heartbeat prompt likely still watching retired artifacts (UNVERIFIED); 3 unregistered overnight jobs. |
| Plans / priorities | 4/10 | Hub two months stale; annual plan not reviewed Q3; revenue vs $145k tracked nowhere. |

---

## 4. Evidence by area

### 4.1 Skill layer (installed in the claude.ai account, 37 skills)
- Custom skills and install dates: hans-ai-systems, hans-copywriting, hans-show **11 Jun**; bml-seating-chart 14 Jun; magic-consult 16 Jun; hans-training 22 Jun; kelly-swanson, magic-council, mccabe, nate, paul-harris, tommy-wonder 23 Jun; anti-ai-writing 5 Jul; hans-marketing, hans-social, hans-website, update-knowledge-base 20 Aug; write-like-hans 4 Sep; barry, gerard, jonah-babins, rory 2 Oct.
- `hans-video` is **not installed** in the account at all (lives only in `99_Skills/` and on the Mac). Fine while video is Mac-only; note it.
- Local-path dependencies (`/Users/Macbook/...`): 10 of the custom skills. Thin loaders: hans-show (56 lines), hans-ai-systems (42), magic-consult (91), hans-marketing (100, but also inlines its rules).
- `magic-council` carries copies of the 7 avatars; **gerard and rory copies differ** from the standalone skills (38 and 24 changed lines). The maintenance note says to re-copy; it was not done after the 2 Oct updates.
- `magic-consult` (One Ahead, Meltzer, Birbiglia, Swiss, McCabe) overlaps `magic-council` (rory = One Ahead, mccabe) and the Drive-only comedy-* skills (birbiglia, meltzer, taylor-tomlinson, comedy-council, hans-comedy, pete-holmes exist in `99_Skills` but are neither installed nor in the backup script's MINE list). Decide one front door for craft questions.
- Stale headers: `hans-copywriting` "Version 1.0"; `hans-training` "Status (Jun 2026): ad-hoc through mid-July… recalibration ~15 Jul" in the installed copy (the `99_Skills` mirror is 3 Sep; whether zones were rebuilt there: UNVERIFIED).
- `backup_skill.sh` MINE list: 35 names; not in it: jonah-babins, birbiglia, meltzer, taylor-tomlinson, comedy-*, pete-holmes, hans-comedy, `_mobile`, and the planned hans-accounting. `_archive` has no snapshots for kelly-swanson, mccabe, nate, paul-harris, tommy-wonder, hans-social.

### 4.2 Routines (registry in `_START_HERE` § What runs on its own)
Alive with Drive proof: crm (today 05:31), kb-intake digest half (today 09:46), weekly-ads (5 Oct), weekly-gbp (5 Oct), weekly-website (5 and 7 Oct), weekly-expense-sweep (4 Oct, but ledger frozen since 7 Sep, last receipt 6 Sep, four empty sweeps). No Drive artifact: flight-travel-blocks, the three launchd social queues (logs on the Mac only), systems-heartbeat (by design). The archived pre-rebuild heartbeat prompt checks retired artifacts (`SITE_AUDIT_*`, `castaways-google-post`, `skjema-vaktpost`); the 5 Oct rebuild entry lists five rewritten tasks and heartbeat is not among them. **Verify the live heartbeat prompt**; if unchanged it alarms on the wrong things and misses `weekly-*`. Unregistered unattended jobs: `shrink_night.sh` (starts when both drives mount), `batch_transcribe.py`, `cut_reactions.py`; the storage plan's step 11 proposes a monthly routine; the accounting plan implies a weekly Ask-Hans queue. Registry rule says register on creation.

### 4.3 Business folders (00–08, 90)
- **Secrets in the KB:** `01_BML/BML_MailerLite_API_token.md` (live, full-scope, unindexed); `ACCOUNTING_BUILD_PLAN.md` proposes storing `.fiken_token` inside the Drive-synced KB; `ig_pipeline/config.json` stores the Bright Data key; bank account on 06 invoice PDFs; TIN/NIS in `Tax_and_Compliance`.
- **BML Season 5 facts in public-ok files** that S6 copy will be generated from: REPEAT26 20% / LOCAL26 10% (`Pricing_and_Tickets`), LOCAL26 = 15% and = 10% in two sections of `Chatbot_KB`, "fifth production", "season extended through June 21 2026", "No refunds. No rescheduling" (vs the 29 Sep FINAL 48-hour ladder). `Discount_Codes.md` (5 Oct) is correct: S6 = FOUNDHIM only, LOCAL15. Show count 55 / 56 / 57 across three files.
- **Pricing:** `Pricing_Master` (21 Jun) vs `Pricing_Tiers` (15 Jun): Tier 3 "USD 5,000+" vs "$5,000–15,000"; Tier 1 "BBD 2,000–4,000" vs "~$500 USD floor"; Gerard benchmark $15–25k vs $10–20k. Norway floor for Barbados-travel gigs: 80–100k (`03 README`) vs 60–80k (`Pricing_and_Rates`) vs 40–80k (city pages); 2026 reality: 30k, 40k+travel, 60k, 75k. Mingle add-on "+10,000 fixed" in three places, "moving to ~15,000, do not publish as fixed" in a fourth. FX 1:10 vs 50k≈$4,500.
- **Clients/testimonials:** `Full_Client_List` (15 Jun) has no 2026 clients, lists Health Directorate twice, lacks Google/BCG/Hilton. Skatteetaten quote attributed three different ways. `Approved_Quotes_Register` is the de-facto master (CLAUDE.md says so) but `00_Brand_Voice/_README` does not list it and six quotes exist only there.
- **Learning loop:** digests daily to 8 Oct; transcription broke 5–7 Oct (Linux binaries after the Mac migration), fixed 8 Oct. Marketing_reference daily log: KEPT 2 / 13 / 3 / 1 for Jul / Aug / Sep / Oct; ai_systems: 3 / 10 / 3 / 0. `geo_reference` is 350 KB. CATALOG last 21 Jun; nuggets last 29 Jun.
- **Castaways split:** a separate Castaways KB exists; `06_Castaways/_README` does not point to it and says the folder is empty (holds 2 invoices). `08_Resources/Bot_Knowledge/castaways.md` is a second full fact sheet that will drift.
- **_INBOX:** 10 unfiled files, 2018–Oct 2026.

### 4.4 CRM (44_Gigs) — detail
59 files + 1 PDF. Ledger 29.6 KB (4 Aug) → 97 KB (16 Sep) → 165 KB (8 Oct), 442 lines, longest row 4,714 chars; top ~1,800 words are ten dated "Sveip" chat reports despite rule 2. ~Half the ⏰ rows closed but retained. `gigs/` dead (template untouched since 29 Jun; O2 file contradicted by the ledger). `_SWEEP_CARD_PROMPT.md` retired but present. README rule numbers duplicated (two 16s; 10 after 18). Duplication: Capsol in six places; Ahlsell in four; win-back pool in four. Channels with no next action: Island Villas (39 days), Scenorama, OK Collective, Festus, DCP. Missing why-lost or price: Tieto, Osloguide, Nordea, Serit, Autodesk, Abacus, JSG (the ledger names these gaps itself, which is good). Tool truncation: the ledger's final Lost rows could not be read; UNVERIFIED.

### 4.5 Creative (05_Creative)
Current: Show_Reference (28 Jul), Comedy_Writing (17 Aug), Story_Bank (13 Aug), Season6 BUILDOUT (68 KB, 23 Sep), five S6 drafts, Leankonferansen script. Problems: `BML_2026_Show_Script.md` still says "IN DEVELOPMENT… title undecided" for a show that ran Dec 2025–May 2026; S6 title split ("Have You Seen This Man?" vs tarot backs "WHO ARE / YOU?"); BUILDOUT §7 says the bookend is carried by the box, §5 says the box is OUT; open questions answered but not struck; "only the 30 Jul call exists on the calendar" for six Rory sessions; show opens 18 Dec with "NOTHING IS LOCKED". Seat count 30 / 26 / 50 in three files. `_README` (23 Jul) omits Footage_Library, Video_Edits, Show_Transcripts, Season6_Tarot_Cards, Impossible_Bottle, Business_Card, Maps, Keynote and seven S6 drafts. Business material inside creative: Business_Card RFQs, tarot pricing, Research_Sources marketing scrapes.

### 4.6 Plans and project files
`ACTION_PRIORITIES` frontmatter 20 Jul, modified 8 Sep, live block 4 Aug. `HANS_2026_PLAN` "last updated 22 Jun", quarterly review missed, O2 "dates pending", milestones unmarked; $145k target tracked nowhere (`Wins_Log` has one example row). `80_project_files/_README` (2 Oct) omits four new files and two weekly logs, names a retired routine, lists `Wins_Log` and `MONTHLY_MARKETING_SESSION` as live; eight June/July leftovers at top level; the 6.4 MB `.mhtml` flagged in July is still there (now in `_assets/`). `audits/` uses three naming schemes. Decisions log: ~200 entries 1 Sep–8 Oct; "append at bottom" violated (a 5 Oct entry after 7 Oct); mixed NO/EN formats; the storage plan's progress log duplicates it. Contradicted-by-files decisions: `/morning`, `/next`, `/done` retired 4 Aug but still in `Claude code/.claude/commands/`; "monthly-ads-loop" still named in `_README`; brand-term pause review (21 Sep) never done; "7 creators" vs "5 accounts".

---

## 5. What to do, in order

Effort: S = under an hour, M = a session, L = multi-session or needs Hans's hands.

**Today (risk)**
1. **Rotate and remove the two tokens** (MailerLite file; Bright Data key in `ig_pipeline/config.json`); fix the accounting plan to keep `.fiken_token` outside the KB. Add `secret` to the visibility rule and a "never in the KB" line to `_KB_STANDARDS`. S.
2. **Clear the three overdue money items** (Tromsø contract/invoice, Sjøentreprenøren 43k invoice, Deme offer) and ok Repstad into Confirmed. S, Hans.
3. **Copy `_moments.csv` + `_reactions.csv` from the 4TB into `05_Creative/Footage_Library/`.** The only clip index is on a disk at 27 GB free with no backup. S.
4. **Strip the twins and family travel from business files**: `Schedule_and_Season.md` (public-ok), the two client files, the ledger rows, O2 file; move `MAC_INDEX.md`, the privat/mac CSVs and `catalog/inbox_2026-10/` logs to `07_Personal` or delete after the sort is verified; move the private-folder regex out of `catalog_drive.py`. S–M.

**This week (propagation and the hub)**
5. **Write the OCTOBER stack in `ACTION_PRIORITIES.md`** and strike the contradicted lines (BML off-season, NO ads paused). S.
6. **Re-upload the edited skills to the claude.ai account** (hans-copywriting, anti-ai-writing, hans-training at minimum; then all custom ones) and add "re-upload after edit" to the skill protocol in `_KB_STANDARDS`. Run `backup_skill.sh --mine`; add the missing names to MINE. Re-copy gerard and rory into magic-council. S–M.
7. **Verify the live `systems-heartbeat` prompt** matches the 5 Oct routine names and artifacts; register the overnight shrink/transcribe jobs or mark them one-off with an end date; give flight-travel-blocks and the social queues a Drive artifact (one appended line). S–M.
8. **S6 fact sweep of 01_BML public-ok files** (codes, "fifth production", June extension, refund wording, 55/56/57). S.

**This month (structure hygiene)**
9. **Split the ledger**: WAITING + ⏰ (future rows only) + pipeline/won/lost; sweep reports → `CRM_RUN_LOG`; strategy blocks → `03_Norway/Julebord_Tour_2026_Nov_Dec.md`; closed ⏰ rows → client sweep logs on close; delete `gigs/` and `_SWEEP_CARD_PROMPT.md`; fix rule numbering; archive naming `GIGS_LEDGER_YYYY-MM-DD.md` monthly. M.
10. **Reduce generated drafts**: no auto day-of for referred/private leads; win-backs as one monthly pick-list; a one-line "call outcome?" prompt after every Cal.com booking; signed contract = Confirmed without a second ok; a frontmatter-vs-ledger status check in the sweep. M.
11. **Make `Pricing_Master` the real master** (julebord ladder, mingle status, team-building, villa add-ons, one deposit policy, "verified on" per line); `Pricing_Tiers` → pointer. M.
12. **One testimonial/client source**: declare `Approved_Quotes_Register` canonical in `00_Brand_Voice/_README`; the three curated review files and both Track_Records → pointers; add 2026 clients to `Full_Client_List`. M.
13. **Stop the digest bloat**: keep only KEPT items in reference files; "0 KEPT" days → monthly roll-up in `_digest_archive`; cap reference files (~60 KB) with dated appendices; shrink `geo_reference`. Check whether the nugget sorter has had input since June; if not, say so in `90_Learning/_README` or retire it. M.
14. **hans-video reference files**: clip register schema, consent register + door-notice photo, routine cue-line bank (then re-run `cut_reactions` on the 16 empty nights before 4K originals go), capture SOP; close the two open taste rulings; fold LEARNINGS into SKILL; regenerate `FOOTAGE_INDEX` with a "verified on" header; fix `_STATUS`; point `Video_Pipeline.md` at hans-video. M.
15. **Creative housekeeping**: mark `BML_2026_Show_Script.md` "S5 as performed" and point the other three running orders at it; one S6 title; strike answered BUILDOUT questions; update `_README`; move Business_Card and Research_Sources out. M.
16. **READMEs**: 01, 03, 04 (+Corporate_Caribbean), 06 (point to Castaways KB, move invoices), 07, 80. Clear `_INBOX`. Delete the 50-byte stray file and retired commands in `Claude code/`. S.
17. **Q3 review of `HANS_2026_PLAN`** with one "revenue vs target" table fed from the ledger and Fienta. M.
18. **Decide the expense sweep**: four empty weeks; fold into the accounting plan's receipt flow or retire the Sunday task. S decision, M merge.

**Next quarter (plumbing)**
19. **Nightly KB-text mirror to a private GitHub repo** from the Mac, so cloud/phone sessions read the real KB and can hand edits back as commits. M.
20. **Fatten `hans-show`** (inline Show_Reference + Comedy_Writing essentials) and decide one front door for craft questions (magic-council vs magic-consult vs the uninstalled comedy-* set). M.
21. **Second copy of originals**: verify the 1080p shrink, buy the 5 TB, mirror. L, Hans.
22. Optional tooling after 14: nb-whisper for Norwegian; scene detection and pose-based reframe. M–L.

---

## 6. Not verified (could not reach from Drive)
- Whether the Nugget Inbox Apple Note has had entries since 29 Jun (so whether the sorter is dead or idle).
- The live `systems-heartbeat` and `flight-travel-blocks` prompts on the Mac.
- Content of the three launchd `publish_log.txt` files.
- Whether the Mac's live skill copies differ from the `99_Skills` mirrors (only the mirrors and the installed account copies were compared).
- The final Lost rows of `GIGS_LEDGER.md` (tool truncation) and the 97 KB September ledger backup.
- Contents of `ocr_rows.json` and the `07_Personal/Expenses` ledger (listed, not read).
- `geo_reference.md` (350 KB) and `Hans_Templates.md` (107 KB) were probed structurally, not read line by line.
- Which legal entity name is correct in the 6 Oct YouTube audit entry ("HG Entertainment AS" vs the two entities in the accounting plan).

*Written 8 Oct 2026 from a cloud session. File it under `80_project_files/` and add it to `_README.md`; the July audit lives in `_archive/`.*

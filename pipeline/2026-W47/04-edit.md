# Edit: 2026-W47 (rewrite 2, tool comparison)

Piece: "Don't wait for the company rollout: run a capped, four-week opt-in." Jon held the publish again. Wade rewrote on top of fe58e26's `04-final.md` at 259c061, adding Rhett's Addendum 3 (635a84d, Grok Bot vs enterprise AI tools) and Jon's citation and wording notes. This file replaces the edit log for fe58e26. Inputs: `03-outline.md` and `03-draft.md` at 259c061, `02-brief.md` with addenda 1 to 3, `style/jon-academic-voice.md`. Governing files are unchanged since fe58e26 and were re-read.

## Fact-check
Every vendor page in the tables, the appendix and the cost sections was opened live on Fri Nov 20, 2026, and each quote was matched against the page text. The research sources from fe58e26 (Bick et al., Pew, Gallup, GOV.UK, DBT, Puthal et al., lstack) are unchanged in the text and were verified in that round.

| Claim | Source | Verified |
|---|---|---|
| Grok Bot prices: Plus $8, Premium $30, Super $100, Ultra $200 a month; team seats $30 / $100 / $200; Teams "$30+/user/month"; tax excluded; "Prices subject to change"; Cursor third-party line; 24-hour cancel line | x.ai/pricing, docs pricing | ✅ unchanged |
| Grok Bot cap, seats, cancel, boundary, Enterprise-only controls, rollout checklist | docs caps (updated Nov 17), teams (Nov 17), team plans, cancel, usage limits | ✅ all quotes still verbatim after the Nov 17 updates |
| Meetings "on Team, Enterprise, Ultra, and Super plans"; joins "Google Meet, Zoom, or Microsoft Teams calls"; "listens, takes notes, answers questions in the meeting chat" | docs meetings (updated Nov 17) | ✅ verbatim fragments of "A Bot can join your Google Meet, Zoom, or Microsoft Teams calls. It listens, takes notes, answers questions in the meeting chat..." The 1.0 post still says "Team, Enterprise, and Ultra"; the newer meetings doc adds Super, and that's what is cited |
| Team Bots share quote; routines trigger list; persistent computer; "Connect apps"; MCP server outside the catalog; MCP policy "applies in full"; Privacy Mode training line; SCIM | docs team bots, routines, computer and apps, teams | ✅ |
| ChatGPT: Standard seat "access to ChatGPT, ChatGPT Work, and Codex"; $25 monthly / $20 annual; Premium $125 / $100; "OpenAI won't train on your workspace's data" | OpenAI Help Center, Business overview (updated about Nov 19) | ✅ |
| Workspace agents share quote; off by default for Enterprise | Help Center, workspace agents | ✅ |
| Team tasks "run on a schedule or supported trigger, using approved company tools"; "configure app connections for teams"; custom GPT creation disabled, "Use Plugin Creator" | Enterprise and Edu release notes | ✅ but these are Enterprise release notes, so both cells now say "Enterprise" |
| Record macOS only; "Calendar auto-join currently supports Google Meet links only"; Zoom and Teams started manually | Help Center, Record | ✅ |
| Dots cloud toggles ("Cloud browser use", "Cloud network access", "Cloud computer use") | Help Center, managing dots | ✅ Enterprise, Edu and Healthcare only, so labeled "Enterprise" |
| Codex description; Codex Cloud "runs coding tasks on OpenAI-managed computers"; included across ChatGPT plans | Help Center, Using Codex | ✅ |
| Codex pricing: Business "$20/ user / month*" ("*2+ users, billed annually"), "$25 per user per month when billed monthly", Enterprise "Contact sales", "SCIM, EKM ... RBAC ... Audit logs", "Data retention and data residency controls" | developers.openai.com Codex pricing | ⚠️ the draft quoted "$20 / user / month", which isn't verbatim. Now unquoted plain words, with the Business overview cited too. Rest ✅ |
| Slack @ChatGPT to Codex Cloud; scheduled tasks; plugins "can include skills and MCP servers"; Computer Use on macOS and Windows | developers.openai.com | ✅ |
| Copilot: add-on "$30.00 user/month, paid yearly"; "a qualifying Microsoft 365 plan"; Agent Builder and Copilot Studio; "Researcher, Analyst, and Facilitator"; connectors; metered agents | microsoft.com Copilot Enterprise pricing | ✅ The draft's "Standard Enterprise add-on" isn't a Microsoft product name (the page says "Microsoft 365 Copilot (add-on)"), so "Standard" was cut |
| Copilot Business promo: "Originally starting from $21.00 now starting from $18.00"; promotional terms; EDP line; usage-based billing | microsoft.com Copilot business pricing | ✅ promo still live. Offer terms on the page: "available between July 1, 2026, and December 31, 2026", annual commitment, "promotional pricing applies to the first year only" |
| Facilitator answers in chat; scheduled meetings only | Microsoft Support | ✅ |
| Scheduled prompts across Teams, Office.com, Outlook; "up to 10 active and 50 total schedules per user"; compliance boundary; Power Platform retirement Dec 31, 2026 | Microsoft Learn (updated Nov 11) | ✅ |
| Copilot Studio computer use and five Copilot Credits; custom connectors "to connect to any publicly available API" | Microsoft Learn | ✅ |
| Workspace: Starter $7, Standard $14, Plus $22 per user per month; "Gemini AI assistant"; Enterprise "Contact sales" | workspace.google.com/pricing | ✅ figures match. Static text shows "All plans billed monthly" and "Price is per user/month and does not include tax", but the Annual/Flexible toggle state still can't be read from the static page, so no billing term is added. The page also runs a new-customer "50% off" offer; the table rightly shows standard prices |
| Gems quotes | Workspace Updates blog, Sep 18, 2025 | ✅ fixed to verbatim (see check 4) |
| Meet notes "emailed to the organizer"; Business Standard and up | Workspace Admin Help (updated Nov 10, 2026) | ✅ |
| Gemini schedules "up to 10 active schedules at a time"; connected-app requirement | Gemini Apps Help | ✅ |
| Workspace Studio starters | Workspace Studio Help | ⚠️ the source reads "You can choose an event, schedule, or create a trigger manually." The draft's ellipsis ("an event, schedule, or ... manually") changed the meaning. Now quoted in full. "Gmail, Sheets, and Drive, as well as other common apps" ✅ |
| Chrome auto browse; "off by default for managed users" | Chrome Enterprise Help | ✅ |
| Work-account chats not used to improve models | Gemini Apps Help | ✅ |
| UNVERIFIED items from Addendum 3 | addendum 3 | ✅ none appear as fact in the draft |
| Overclaims ("better", "best", "beats", "unique"), em dashes, tools Jon doesn't use, Jon's surname or address | standing rules | ✅ none |

No new sources. No numbers beyond the brief and addenda.

## Wade's checks
1. **Live re-check.**
   - All product pages were opened today. The two Nov 17 pages (spending caps, teams) still match word for word, and so does the meetings doc, also updated Nov 17.
   - The Copilot Business promo is still running. Its offer terms run to Dec 31, 2026, first year only.
   - Fixes from the re-check: the non-verbatim OpenAI $20 quote, the Workspace Studio ellipsis, "Standard" removed from the Copilot add-on name, and "Enterprise" labels on team tasks, app connections and the dots toggles.
2. **Vendor lettering.** Rebuilt from each page's own date.
   - Grok Bot: n.d. (x.ai/pricing), then 2026a to k. Every docs page shows "Last updated" in 2026. The letters are correct and alphabetical.
   - OpenAI: Help Center articles show "Updated: [n] days ago", all within 2026, so they're dated: 2026a Business overview, 2026b release notes, 2026c Record, 2026d workspace agents, 2026e dots, 2026f Using Codex. The developers.openai.com pages show no date: n.d.-a Computer Use, n.d.-b Plugins, n.d.-c Pricing, n.d.-d Scheduled tasks, n.d.-e Slack.
   - Microsoft: the two pricing pages and the Support page show no date: n.d.-a Facilitator, n.d.-b AI for business, n.d.-c Enterprise. The Learn pages show "Last updated on": 2026a computer use, 2026b scheduled prompts, 2026c connectors.
   - Google: the Help pages and the pricing page show no date: n.d.-a pricing, n.d.-b Chrome, n.d.-c Workspace Studio, n.d.-d Schedules, n.d.-e work account. The Admin Help Meet page shows "Last updated 2026-11-10": Google (2026).
   - Order: "Google Workspace (2025)" now sits after all "Google" entries. In-text lists put n.d. before dated works.
   - Every in-text cite was remapped by script and cross-checked. Each one matches an entry, and every entry is cited.
3. **Author.** "SpaceX Super Intelligence", consistently. Every docs.x.ai page names it as the organization author in its metadata, and x.ai's footer reads "© 2026 SpaceX Super Intelligence LLC". Only the 1.0 post's metadata still says xAI, which looks stale. Addendum 3's "xAI" isn't used.
4. **Shortened quotes.**
   - Gems: the draft quoted "you can share ... with other users", with the ellipsis dropping the object. Now verbatim: "you can share Gems with other users in your organization and beyond".
   - Grok Bot meetings: both fragments are verbatim and accurate. The plan list sits outside the quotes.
   - Also fixed: Workspace Studio (meaning changed by the ellipsis) and OpenAI $20 (not verbatim).
5. **Our own words.**
   - "previously $21.00" now quotes the page: "Originally starting from $21.00".
   - The bundling opener ("Bundling may matter more to a cost-minded exec than any single feature") is unsourced and ranks bundling above features, so it was cut. "For this reason" was cut from the follow-on sentence.
6. **Length.**
   - Cuts: the bundling opener, a duplicate "Codex is included" clause, the publisher clause repeated in the cost section, "One gap remains", the "Two terms carry this argument" signpost, the table-scope sentence, and a tightened lead-in to the "fits when" list.
   - The body before the appendix is still about 3,440 words. Further cuts would drop sourced points or the comparison section Jon asked for.
   - Concise is scored 2. The remaining length is structural: the voice guide's paragraph shape, full author names at first mention, and a new comparison section. That's for Chet and the look-back.
7. **Fairness.**
   - No "better", "best" or "beats". Each "fits when" is framed as fit.
   - One unfair implication was cut. The test-the-difference examples listed "event-triggered routines, or a persistent bot computer". ChatGPT Enterprise has webhook-triggered tasks and dot cloud computers, and Workspace Studio has event starters, so those aren't sourced differences. The example list now keeps only the documented one: joining Meet, Zoom and Teams calls.
   - The tone stays tool-agnostic. Nothing implies which tools Jon or lstack use.

Other fix: "The GDS Service Manual" is now "The GOV.UK Service Manual", which matches the reference.

**Not changed, flagged for Chet:** Jon's "name every source in full at first mention" note led Wade to list all authors in narrative cites, e.g. "Puthal, Mishra, Mohanty, Longo and Yeun (2025)". The voice guide says "et al." for three or more authors (APA 7). I left Wade's version because it follows Jon's newer note. If Jon meant naming the publication or organization, switching to "et al." saves about 25 words.

**Repeat mistake:** this is the third W47 round with a non-verbatim or meaning-shifting shortened quote. Per AGREEMENTS.md, that calls for a `SKILL.md` check, for example: "diff every quoted fragment, and every ellipsis, against the live page text." That's for the Reviewer to propose and Chet to approve.

## Scores
| Principle | Score | Note |
|---|---|---|
| Useful | 5 | Five-item ask plus a fit table an exec can use to frame "why not the tool we already have" |
| Clear | 4 | Defined terms, plain glosses, four-row table. Wide tables and a long appendix are dense on X |
| Credible | 5 | After fixes, every quote is verbatim and every cell traces to a live official page. UNVERIFIED items stay out, counterpoints are named, and the comparison makes no performance claims |
| Concise | 2 | About 3,440 words before the appendix. Readers will skim the comparison and the cost detail. Structural, not fixable by cuts alone |
| Iterative | 4 | Jon's hold notes applied (comparison section, Super for Meetings, article wording, $30 Copilot in the table). But shortened-quote errors recurred for a third round |
| **Average** | **4.0** | |

## Send-backs
0 of 1 used. The angle is sound: a sanctioned, bounded pilot that tests what an existing tool doesn't cover, with no claim that Grok Bot beats competitors or that opt-in beats a mandate. The issues were quote fidelity, citation dates and a few unsourced phrases, fixed here as cuts and clarifications.

**Pre-publish:** re-check x.ai/pricing, the docs.x.ai pricing, spending caps, team plans, teams and meetings pages, the Microsoft Copilot business page (promo ends Dec 31, 2026), workspace.google.com/pricing, and the ChatGPT Business overview. Several of these change weekly.

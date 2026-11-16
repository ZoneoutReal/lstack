# Edit: 2026-W47

Piece: "Don't wait for the company rollout: run a capped, four-week opt-in." The earlier W47 piece is shelved in `shelved/2026-W47-boring-checks/`; this file replaces its edit log.

## Fact-check
| Claim | Brief # | Verified |
|---|---|---|
| Individual prices and the tax line ("Prices subject to change") | 1 | ✅ x.ai/pricing and docs.x.ai pricing, re-checked Nov 16, 2026: Free $0, Plus $8, Premium $30, Super $100, Ultra $200 a month; prices exclude tax; "Prices subject to change" |
| Third-party models billed separately | 1 | ✅ but the draft broadened it. Source: "Third Party model usage in Cursor is not included in the monthly prices shown and must be purchased separately." Every vendor page scopes this to Cursor. Now quoted verbatim with a short gloss, so it isn't read as covering all bot usage |
| Grok Bot on Premium, Super and Ultra, not Plus; bot usage "draws from that seat's shared weekly usage pool, not a separate additive pool"; no official size in hours, tasks or dollars | 2 | ✅ docs.x.ai pricing and usage limits |
| Team seat prices $30 / $100 / $200; same usage as the matching tier; "three Premium seats and one Super seat"; "Plus isn't available for teams"; "Seats do not share weekly pools"; Enterprise for "invoicing, pooled usage, or advanced security" | 3 | ✅ all on docs.x.ai pricing, docs.x.ai usage limits and x.ai/pricing. cursor.com link dropped from [3] |
| Team Bots on Team and Enterprise; Meetings on Team, Enterprise and Ultra | 4 | ✅ x.ai Grok Bot 1.0 post (Nov 2) and docs.x.ai teams page |
| Gloss: Team Bots are shared bots | 4 | ✅ kept, trimmed to the 1.0 post's wording ("everyone on a team can work with the same AI teammate") |
| Monthly additional usage limit; Additional Usage stops at an empty balance or the cap; "Alerts do not stop usage..."; Auto Top-up "off unless you turn it on"; no Grok Bot-only cap | 5 | ✅ docs.x.ai spending caps and teams FAQ |
| Gloss: what Additional Usage is | 5 | ✅ corrected. docs.x.ai usage limits: "any third-party model usage in Cursor, plus any first-party usage beyond your included weekly usage." The draft's "paid usage beyond what the seats include" left out the third-party part; now trimmed to match |
| Per-member limits ("a default monthly limit per member and per-member overrides") | 5 | ⚠️ only on cursor.com. docs.x.ai says self-serve admins set "one monthly additional usage limit for the whole team, either a fixed amount or an amount per seat." Sentence cut, and the cursor.com link dropped from [5] |
| Joining is prorated; removed members lose access, seat stays until Reduce seats, comes off at period end; canceled seat active to period end; cancel 24 hours before renewal | 6 | ✅ docs.x.ai team plans and cancel pages; x.ai/pricing |
| Teams plan: Grok Bot on by default, "no switch to turn it off"; Enterprise-only controls; "People can belong to more than one workspace" | 7 | ✅ docs.x.ai teams page and team plans |
| UK trial 30 Sep to 31 Dec 2024, 20,000 employees; earlier pilots "limited to 300 licences at most"; DBT 1,000 licences, 3 months | 8 | ✅ GOV.UK findings report; DBT evaluation PDF |
| GOV.UK Service Manual: cost vs improvement; stopping is not a failure; "around 4 to 8 weeks is typical" | 9 | ✅ verbatim |
| 26 minutes a day, self-reported | 10 | ✅ findings report and press release |
| DBT: small savings; no evidence of improved productivity; Excel slower and worse | 11 | ✅ verbatim |
| DBT ~70% volunteers, ~30% random, stratified | 12 | ✅ verbatim |
| Denmark 41% / 7%; Microsoft and LinkedIn 78% BYOAI (31,000 people, 31 countries); Gallup 40% and "only 22%" | 13 | ✅ NBER w33777 (revised); Work Trend Index; Gallup |
| NBER take-up 76% / 57% / 69%; 93% and 28%; "consistently associated with..."; framed as associations | 14 | ✅ verbatim |
| DBT peers and line managers; self-led training; Gallup 68% vs 13% | 15 | ✅. The 13% figure is people who "believed it would" help, not people who said it did. Clarified |
| Gallup "three times" and "2.6 times" | 16 | ✅ verbatim |
| PNAS: 16-point gender gap; 12 points within workplace and tasks; "employer restrictions and a perceived need for training" | 17 | ✅ PubMed abstract; 12 points confirmed in the full text (PMC11725873) |
| NBER "precise null effects on earnings and recorded hours", ruling out more than 2% | 18 | ✅ |
| AI Playbook principles and the high-risk validation line; Grok Bot rollout checklist (TLS proxy, sign-in, inherited policies) | 19 | ✅ GOV.UK Playbook; docs.x.ai teams page |
| UK trial limitations quote | counterpoint 5 | ✅ but misquoted. Source: "Limitations were observed when dealing with complex, nuanced, or data-heavy aspects of work." Now quoted from "when dealing" |
| DBT hallucinations | counterpoint 5 | ✅ in the DBT PDF [11], not the cross-government report [C1]. Citation fixed |
| lstack structure quotes ("Files are the handoff", human approves every publish, send back once, researcher KR1) | 20 | ✅ AGREEMENTS.md and roles/researcher.md on main. Structure only; no hours, spend or results |
| No usage multiples (4x / 15x / 50x or 3.5x / 12x) | open question | ✅ absent; the sources still disagree (x.ai/bot shows 3.5x and 12x Premium usage) |
| No opt-in vs mandate causal claim | corrections | ✅ the draft says no study compares them. One line read as causal ("employer backing changes how many people use them and how it goes") and now reads "goes with more use and better reported results"; "Peers and managers shape uptake" softened to "matter as well" (DBT calls it anecdotal) |
| Dropped items (unofficial dollar figures, DTA, Annie Duke, earlier NBER figures, "nearly 2 weeks", lstack results) | dropped | ✅ absent |
| All six counterpoints | counterpoints | ✅ all used, including both required ones (some work stays off the bot; the cap and stop rule must be real) |
| Tools Jon doesn't use; Jon's surname or address | n/a | ✅ absent. Cursor appears once, inside the vendor's own pricing quote |
| Overclaiming words in our voice ("impossible", "deterministic"); em dashes | W47 lessons | ✅ none |

No invented sources or numbers. Every figure traces to the brief and was checked at the original source on Nov 16, 2026.

**Pre-publish:** prices, plan gates and billing wording come from vendor pages that say "Prices subject to change." Re-check x.ai/pricing and docs.x.ai pricing, spending caps and team plans right before publish.

## Cuts and clarifications in 04-final.md
1. Third-party pricing line is now the vendor's verbatim, Cursor-scoped wording, with a short gloss.
2. Additional Usage gloss now matches docs.x.ai.
3. Per-member limit sentence cut (cursor.com only, and docs.x.ai describes it differently); cursor.com links dropped from [3] and [5].
4. Team Bots gloss trimmed to the 1.0 post's wording.
5. Causal phrasing softened in the "why" section.
6. UK trial limitations quote made verbatim; hallucinations citation moved to [11]; Gallup 13% clarified.

## Scores
| Principle | Score | Note |
|---|---|---|
| Useful | 5 | A five-item ask the reader can take to an exec today, with a spend formula, stop steps and an off-limits list |
| Clear | 4 | Plain structure; billing terms are glossed. A few quoted terms ("extensive-margin take-up") stay dense |
| Credible | 5 | Every figure matches its source; both sides of the opt-in evidence are shown; the one misquote, one wrong citation and two loose glosses are fixed |
| Concise | 4 | Long for a one-page plan, but each section carries a decision |
| Iterative | 5 | W47 lessons applied: verbatim quotes, no multiples, no overclaims, no em dashes; all six counterpoints used |
| **Average** | **4.6** | |

## Send-backs
0 of 1 used. Angle is sound: a sanctioned, capped opt-in beats waiting, with no claim that it beats a mandate. Minor clarifications only; see `04-final.md`.

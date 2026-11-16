# Edit: 2026-W47

## Fact-check
| Claim | Brief # | Verified |
|---|---|---|
| 10,926 merged PRs in Oct 2026, up from 809 in June; counts all contributors to the Grok Bot team's code (about 227 people, many "casual or drive-by"); explicitly "not an agent-only number"; team-reported, unaudited | 11, 13 | ✅ slide image in Tan's Nov 4 post ("809 → 10,926 merged PRs a month", "PRs that touch the grok bot team's code"); her reply "all PRs to grok bot, not just mine"; talk captions |
| Share of commits reverted 0.98% (Jun) to 0.47% (Oct); quoted as "% of commits reverted"; never called an error rate or quality score | 12 | ✅ revert slide in the official clip; talk: "steady at about half a percent"; no "error rate" anywhere in the piece |
| PR vs commit mismatch and no revert definition or window disclosed | 12 | ✅ slide says commits, speech says PRs |
| DORA 2024: 7.2% stability reduction per 25% rise in AI adoption | 16 | ✅ 2024 PDF. Draft quoted it as "a 7.2% reduction"; source reads "an estimated 7.2% reduction". Quote corrected |
| DORA 2025: AI as "an amplifier, magnifying an organization's existing strengths and weaknesses" | 17 | ✅ dora.dev 2025 page |
| Tan's thesis and "not blind trust" quote | 1 | ✅ captions, about 1:15 |
| Inverse pyramid: code and static checks first, "constrain what agents can do...", verification next, prose last for "things that require judgment" | 2 | ✅ captions, about 2:03 to 2:30 |
| Written pyramid: human review at the bottom, "the hardest to scale..." | 3 | ✅ Tan's Oct 16 post, verbatim |
| Turn corrections into checks; "less things to look out for in code review" | 4 | ✅ captions, about 3:12 and 9:28 |
| Codebase flaws are copied; "as pristine as possible" | 5 | ✅ captions, about 4:37 |
| "The same checks serve people and agents alike" sourced to Tan's Oct 12 posts, not the talk | 6, corrections | ✅ both posts verbatim ("there is no difference when agents write the code instead..."; "anyone, even randoms and non-technical colleagues, can write good PRs") |
| Banned a hard-to-use React API ("categorically eliminated"); imports across a boundary "forbidden or banned by our dependency graph analyzer and some lint rules" | 7 | ✅ captions (useEffect; Electron main and renderer) |
| "ban 99% of comments", "not enforceable", lint errors "to fix the root cause" | 8 | ✅ captions, about 8:22; Oct 15 post supports |
| Lint rule to "stop the bleed", then rewrite old patterns | 9 | ✅ Oct 14 reply, verbatim from "create" |
| Runtime verification; review "shrunk into looking at verification artifacts"; formal methods "certainly not a silver bullet" | 10 | ✅ captions, about 9:53 and 11:25 |
| 49 people with exactly one PR in October | 13 | ✅ contributor slide in the clip (Oct: 1 / 22 / 77 / 78 / 49) |
| Cold launch 2,669 to 1,831 ms (31% down); long-chat median typing 11.6 to 4.5 ms (61% down); May vs the Nov 4 slide | 14 | ✅ second slide image in Tan's Nov 4 post |
| Release pace: 15 desktop releases in Oct, median 28 hours apart; no "daily releases" | 14, corrections | ✅ releases slide in the clip (7 / 19 / 15; 44 / 25 / 28 hours). Clip caption's "daily stable releases" not used |
| Order of operations ("before you jump into building out a software factory", "verification story", "produces more slop"); "six months" | 15 | ✅ captions, about 15:25 and 1:43 |
| DORA change fail rate (rollback or "hotfix"); "having one metric to rule them all" | 18 | ✅ dora.dev four-keys guide |
| Fuzzing run opens fix PRs and auto-merges; labeled our inference that fixes may arrive as new PRs | C1 | ✅ captions, about 16:26; the product named in the talk is left out |
| "most of the volume of PRs i land are refactoring" | C2 | ✅ Oct 11 reply |
| "it isn't perfect of course and we do make mistakes" | C3 | ✅ Oct 27 post |
| "mission critical 'hard' (eg embedded) software" exemption | C4 | ✅ Oct 11 post |
| "most product code that we land no longer really requires deep human review", framed as her team, not a recommendation | C5 | ✅ captions, about 16:51 |
| Quotes only from Tan's talk, her posts and her slides (plus DORA's own documents); AI Engineer's clip caption not quoted | corrections | ✅ |
| No causal claim: "coincided with the checks, not that the checks caused them" | corrections | ✅ |
| Tool-agnostic: no product pitch from the talk's "outer loop", no tool or workflow attributed to Jon; React and LSPs appear only as Tan's examples | corrections | ✅ |
| All five counterpoints used (revert, PR count, one team / self-reported, judgment, DORA baseline) | counterpoints | ✅ all five on the page; none dropped |
| Dropped items ("30x'd", "70% of daily tokens", "mostly written by agents", "3,000 of them", "at least once a day", METR 19%) | dropped | ✅ absent |
| Sources list uses only links from the brief, and each resolves to what it is cited for | all | ✅ every URL appears in the brief; X posts read by id; YouTube time stamps land in the right section of the captions; DORA pages return 200 |
| Jon's surname or address; Claude, Hermes or OpenClaw attributed to Jon | n/a | ✅ absent |
| Em dashes (new skill check) | n/a | ✅ none in the draft or the final |

No invented sources, numbers or results. Every figure traces to the brief and was checked against the original source.

## Cuts and clarifications in 04-final.md
1. DORA 2024 quote made verbatim ("an estimated 7.2% reduction...").
2. Takeaway: "faster usually means less stable" changed to "more AI adoption usually means less stable delivery". DORA measured AI adoption, not speed, and says speed and stability are not tradeoffs.
3. Plain test, question 4: "most teams see stability fall" changed to "stability tends to fall as AI adoption rises" (DORA reports an average estimate, not a share of teams).
4. Sources: cut "(from the brief)" and the "(brief counterpoint N)" notes, which are pipeline labels, not reader-facing.

## Scores
| Principle | Score | Note |
|---|---|---|
| Useful | 5 | Five numbered checks, a four-question test, and two things to do this week |
| Clear | 4 | Plain structure and short sections. A few terms (LSPs, fuzzing, fix forward) go unexplained, but the reader is engineering managers |
| Credible | 5 | Every figure matches the slides, captions, posts or DORA; scope, team-reported status and the commits vs PRs mismatch are all stated; the one loose quote and two DORA overreaches are fixed |
| Concise | 4 | Each check earns its place; Check 3 is thin but short |
| Iterative | 5 | W45 lesson met: all five brief counterpoints used. Every one of Rhett's corrections to the pitch was followed |
| **Average** | **4.6** | |

## Send-backs
0 of 1 used. Angle is sound: one team's boring checks set against DORA's baseline, with the limits of the numbers spelled out. Minor clarifications only; see `04-final.md`.

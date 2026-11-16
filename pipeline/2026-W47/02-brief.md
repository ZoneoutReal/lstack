# Brief — Put the boring checks in before you scale agent volume

## Reader and promise
Engineering managers and tech leads whose teams are speeding up with coding agents and are tempted to take the volume as proof the process is fine. Promise: a numbered list of boring, deterministic checks (architecture, lint, tests, verification) that apply to every pull request no matter who or what wrote it, plus a plain test for whether those checks are in place before you let volume rise. Source spine: Lauren Tan's AI Engineer CODE talk "All Code Is Slop (Except Mine)" (given Nov 11, 2026; video posted Nov 14) and her own posts, with DORA research for the outside view and the counterpoints.

Notes on sources:
- The talk video is the official upload on the AI Engineer YouTube channel, which Tan linked from her own account. Talk quotes come from the video's captions. The figures in claims 11 to 14 were also checked against the official AI Engineer clip, both by transcribing its audio and by reading the slides on screen.
- YouTube links carry approximate start times taken from the captions. The X clip has no verified clock marks, so describe the moment rather than citing a time.
- All Grok Bot team figures are team-reported by Tan. None are audited.

## Key claims
| # | Claim | Source (link) |
|---|---|---|
| 1 | Tan's thesis: "the job of the software engineer ... is figuring out how to maintain or even improve the quality of your code while massively increasing your productivity." She frames it as trust: "Not blind trust but investing in your agents environment so you can trust that your agents are going to do the right thing." | https://www.youtube.com/watch?v=O_zcc6Xl12g&t=68s |
| 2 | Her "inverse pyramid" says where to spend effort. First come two deterministic layers: the code itself (API design, architecture, refactoring) and static checks (lint rules, type systems, compilers, testing). These "constrain what agents can do and force them to do the right thing by default." Runtime and formal verification come next. Prose (rules, skills, AGENTS.md) comes last, for "things that require judgment." | https://www.youtube.com/watch?v=O_zcc6Xl12g&t=123s |
| 3 | In her written version of the same pyramid, human review is the bottom layer: "the hardest to scale. at the rate agents land code, it's pretty much impossible to thoroughly review every PR, so spend that effort on the highest leverage point, designing an environment where agents do the right thing by default." | https://x.com/poteto/status/2111133080526495985 |
| 4 | Turn corrections into checks. "Whenever you're correcting your agent, think about how you can make that a deterministic check instead of adding another line to your rules ... it's far more reproducible when it's in code." Do it often enough and "you'll find that you have just less things to look out for in code review." | https://www.youtube.com/watch?v=O_zcc6Xl12g&t=192s ; https://www.youtube.com/watch?v=O_zcc6Xl12g&t=550s |
| 5 | The codebase is the agent's biggest input, so its flaws spread. Workarounds, anti-patterns, deprecated code and tech debt are "now likely to be just copied by the next agent since it looks like the established pattern." Her advice: keep the codebase "as pristine as possible so that agents are always copying the good stuff." | https://www.youtube.com/watch?v=O_zcc6Xl12g&t=264s |
| 6 | The checks are the same ones human code has always needed (Tan's post, not the talk): "we have always had lint rules, compilers with good diagnostics and strong type systems, LSPs, etc to help us write better code. there is no difference when agents write the code instead, you just need more of them, and stronger ones." In a follow-up: "maintainers can adjust their codebase so that anyone, even randoms and non-technical colleagues, can write good PRs." | https://x.com/poteto/status/2109699980248408574 ; https://x.com/poteto/status/2109761952696483905 |
| 7 | Architecture checks remove whole classes of mistakes. Her team banned a hard-to-use React API (useEffect) in product code, so the problem was "categorically eliminated, and we never need to catch that during code review again." Imports between the app's main-process and renderer directories are "forbidden or banned by our dependency graph analyzer and some lint rules." | https://www.youtube.com/watch?v=O_zcc6Xl12g&t=326s |
| 8 | Comments are not checks. Agents used code comments to justify quick fixes. The team "decided to just ban 99% of comments" because "they're not enforceable." They replaced them with lint rules whose error messages tell the agent "to fix the root cause." | https://www.youtube.com/watch?v=O_zcc6Xl12g&t=500s ; https://x.com/poteto/status/2110758788525621282 |
| 9 | A pattern for retiring a bad habit: "i would create a lint rule to block new usages of the old pattern to stop the bleed, then open PRs to rewrite all previous patterns to the new one." The talk's closing gives the same order: a lint rule to prevent new occurrences, then clean up the old ones. | https://x.com/poteto/status/2110161793331208527 ; https://www.youtube.com/watch?v=O_zcc6Xl12g&t=911s |
| 10 | Verification is the layer above static checks. Runtime verification means "giving your agent a way to run the code for itself." Review has "really shrunk into looking at verification artifacts instead," such as videos, screenshots, diagrams and formal verification. Formal methods have found bugs, but Tan says they are "certainly not a silver bullet." | https://www.youtube.com/watch?v=O_zcc6Xl12g&t=580s |
| 11 | **The 11,000 figure (confirmed, with context).** Spoken: "last month, our team shipped a ridiculous 11,000 pull requests to production." The slide is titled "grok bot team merged 11k PRs in oct" and shows 10,926 for October, up from 809 in June (23,370 total for Jun to Oct). On her own X account, the same chart is labeled "PRs that touch the grok bot team's code," and she adds that it "is all PRs to grok bot, not just mine." So: about 11,000 (10,926) merged PRs in October 2026, from all contributors to Grok Bot, team-reported. | https://www.youtube.com/watch?v=O_zcc6Xl12g&t=812s ; https://x.com/aiDotEngineer/status/2121981562824564960 ; https://x.com/poteto/status/2118017093677494706 ; https://x.com/poteto/status/2118051545468301479 |
| 12 | **The ~0.5% figure (confirmed, with context).** Spoken: "the number of PRs that get reverted has actually gotten lower on a relative basis and is steady at about half a percent." The slide on screen is titled "revert rate," with the axis label "% of commits reverted": Jun 0.98%, Jul 0.61%, Aug 0.47%, Sep 0.48%, Oct 0.47%. Note the mismatch: the speech says PRs, the slide says commits. Neither says what counts as a revert or how long after merge it is counted. | https://www.youtube.com/watch?v=O_zcc6Xl12g&t=854s ; https://x.com/aiDotEngineer/status/2121981562824564960 |
| 13 | Who was contributing: "in October, we had about 227 people who contributed at least one pull request." Many were "casual or drive-by contributors who don't always have a lot of context." The October slide breaks the 227 down by PRs each: 1 person at 1,000+, 22 at 100 to 999 ("core"), 77 at 10 to 99 ("casual"), 78 at 2 to 9 and 49 at 1 PR ("drive by"). Tan's Oct 27 post says engineers, designers and PMs all contribute. | https://www.youtube.com/watch?v=O_zcc6Xl12g&t=835s ; https://x.com/aiDotEngineer/status/2121981562824564960 ; https://x.com/poteto/status/2115133011352240581 |
| 14 | Quality signals beyond reverts, all team-reported. Speed: Tan says startup, typing, opening new chats and switching chats "has gotten faster" than at launch. Her slide compares May with "now" (the slide was posted Nov 4): cold launch went from 2,669 ms to 1,831 ms (−31%), and median typing latency in a long chat went from 11.6 ms to 4.5 ms (−61%). Releases: spoken "we cut a new stable version about once a day." The slide shows desktop app releases of 7 (Aug, from launch), 19 (Sep) and 15 (Oct), with median times between releases of 44, 25 and 28 hours. | https://www.youtube.com/watch?v=O_zcc6Xl12g&t=870s ; https://x.com/poteto/status/2118017093677494706 ; https://x.com/aiDotEngineer/status/2121981562824564960 |
| 15 | Order of operations, in her words: "before you jump into building out a software factory ... whenever you correct your agent, try and do it by improving your codebase first ... make sure that your verification story is really strong. A lot of this work is a prerequisite to automation anyway. And if your inner coding loop produces slop, then automating that loop just produces more slop." Getting there took her "six months." | https://www.youtube.com/watch?v=O_zcc6Xl12g&t=911s ; https://www.youtube.com/watch?v=O_zcc6Xl12g&t=100s |
| 16 | The industry baseline is the opposite of Tan's result. DORA's 2024 report: "an estimated 1.5% reduction [in delivery throughput] for every 25% increase in AI adoption" and "an estimated 7.2% reduction [in delivery stability] for every 25% increase in AI adoption." Its reading: "improving the development process does not automatically improve software delivery—at least not without proper adherence to the basics of successful software delivery, like small batch sizes and robust testing mechanisms." | https://dora.dev/research/2024/dora-report/2024-dora-accelerate-state-of-devops-report.pdf |
| 17 | DORA's 2025 report describes AI's "primary role" as "an amplifier, magnifying an organization's existing strengths and weaknesses." | https://dora.dev/research/2025/dora-report/ |
| 18 | Measure stability alongside volume, not volume alone. DORA pairs throughput metrics with instability metrics. One of those is "change fail rate," defined as deployments needing immediate intervention, "likely resulting in a rollback of the changes or a 'hotfix'." Pitfalls DORA lists include "having one metric to rule them all" and ignoring Goodhart's law, which "increases the likelihood that teams will try to game the metrics." | https://dora.dev/guides/dora-metrics-four-keys/ |

## Counterpoints
- **A low revert rate does not prove the code is good, only that it was not rolled back.** The topic requires this counterpoint; it is already circulating (https://x.com/SahilExec/status/2122293348983542189). The definitions back it up. Tan's slide measures "% of commits reverted" (claim 12). DORA's change fail rate counts rollbacks *and* hotfixes (claim 18), so a team that fixes forward can have a low revert rate and still ship failures. Tan also says her team's fuzzing run opens fix PRs and auto-merges them (https://www.youtube.com/watch?v=O_zcc6Xl12g&t=981s), which means some fixes arrive as new PRs rather than reverts. That is our inference, not her claim.
- **PR count is not a quality measure, and it doesn't compare across teams.** PR size varies. Tan says "most of the volume of PRs i land are refactoring" (https://x.com/poteto/status/2109361189071499640), and DORA pushes small batch sizes (claim 16), so many small PRs can be a deliberate choice. Treating volume as the proof is DORA's "one metric to rule them all" pitfall (claim 18).
- **One team, self-reported, after a big investment.** The numbers come from Tan, are not audited, and show that results coincided with the checks, not that the checks caused them. Her team built its own client framework, and she says it took her "six months" to get there (claim 15). She also writes, "it isn't perfect of course and we do make mistakes" (https://x.com/poteto/status/2115133011352240581).
- **Checks do not replace judgment, and some code needs more than this.** Tan keeps prose for "things that require judgment" (claim 2), calls formal verification "not a silver bullet" (claim 10), and moves human effort to designing the environment rather than removing it (claim 3). By her own definition, agent-assisted code "won't be Good Code (that is still expensive)." She exempts "mission critical 'hard' (eg embedded) software" from the usual tolerance for imperfect code (https://x.com/poteto/status/2109110547824378140). Her line that "most product code that we land no longer really requires deep human review" (https://www.youtube.com/watch?v=O_zcc6Xl12g&t=1004s) describes her team after these investments. It is not a general recommendation.
- **Without the basics, faster usually means less stable.** DORA's 2024 numbers (claim 16) show the common outcome of more AI adoption is lower stability. Tan's result is the exception the piece explains, not the default a reader should expect.

## Examples / data
Raw material for the numbered checks and the plain test. Each item traces to a claim above; Wade picks and orders.

Candidate checks (generic; Tan's tool names are examples only):
1. Architecture that makes the wrong thing impossible, such as banning a risky API in product code or forbidding imports across a boundary (claims 2 and 7).
2. Lint rules with error messages that point at the root cause (claims 8 and 9).
3. Type systems, compilers and tests (claim 2).
4. Runtime verification: the agent runs the code and shows evidence such as screenshots or video (claim 10).
5. Every repeated review comment becomes a check, and old instances get cleaned up (claims 4 and 9).

Candidate inputs for the "plain test" (the test itself is ours, not Tan's; build it from these):
- Does correcting an agent end in a new check rather than a new line of prose (claim 4)?
- Can a low-context contributor land a good PR (claims 6 and 13)?
- Are reverts *and* hotfixes or fix-forwards tracked alongside volume (claims 12 and 18)?
- Are stability and performance holding as volume rises (claims 14 and 16)?

Key figures, exact:

| Figure | What it is | Source |
|---|---|---|
| 10,926 ("11k", "11,000") | merged PRs touching the Grok Bot team's code, Oct 2026 | claim 11 |
| 809 → 10,926 | Jun to Oct 2026 monthly merged PRs (23,370 total) | claim 11 |
| 0.47% | Oct 2026 "% of commits reverted" (Jun 0.98%) | claim 12 |
| about 227 | people with at least one PR in Oct 2026 | claim 13 |
| 15 releases, median 28 hours | Oct 2026 desktop app releases | claim 14 |
| −31% cold launch, −61% long-chat median typing | May vs "now" (slide posted Nov 4) | claim 14 |
| −7.2% stability / −1.5% throughput | DORA 2024 estimate per 25% rise in AI adoption | claim 16 |

Quotable scale image: "I remember going into work in 2024 and reviewing the three pull requests that my colleagues wrote ... And today, that number is more like 300." She gives no unit or time window, so don't add one. https://www.youtube.com/watch?v=O_zcc6Xl12g&t=211s

Clip: the official AI Engineer clip (https://x.com/aiDotEngineer/status/2121981562824564960, about 91 seconds) covers exactly the results section: PRs, releases, contributors, revert rate and speed. Its caption, "11,000 pull requests in one month. A revert rate around 0.5%.", is AI Engineer's wording, not Tan's spoken words.

## Open questions
- What counts as a "revert" on Tan's slide: a revert commit, within what window after merge, and why does the slide say commits while the talk says PRs?
- What share of the 10,926 PRs were written mostly by agents versus by people? No source gives one.
- Are the 3,000 PRs Tan says she shipped "last month" part of the 10,926? She doesn't say. The October contributor slide shows one person at 1,000+ PRs, but it doesn't name them.
- What are the team's hotfix, fix-forward or change-fail rates? Only reverts are disclosed.
- Is "about once a day" a fair summary of 15 October releases with a median of 28 hours between them? Should the piece use the slide numbers instead?
- For a team without its own framework, what is the smallest first set of checks, and how long does it take? Tan says six months for her and "much less time" for others. That is her estimate, not data.
- Does any public source show a team scaling agent volume *without* these checks and what happened? DORA's survey-level finding (claim 16) is the closest; no named case was found.

## Dropped as unverifiable
- **"30x'd"** (Tan's Nov 4 post, "ship crazy amounts of code (30x'd) without reading it"). It gives no baseline or unit, and it doesn't match the chart in the same post (809 → 10,926). Don't use it.
- **"70% of her daily tokens go into verification."** Tan relays this from a post by "Cindy." The original post was not located or checked, so it's secondhand.
- **"mostly written by agents."** This is a recap's claim about the 11,000 PRs (SahilExec); no primary source gives an agent share.
- **"lauren tan did 3,000 of them herself."** The 3,000 figure is Tan's own ("I shipped 3,000 pull requests to production"), but "of them" (inside the 11,000) is the recap's inference.
- **"at least once a day."** Tan's Nov 7 post says this about releases, but it conflicts with the October slide (15 releases, median 28 hours). Use the talk's "about once a day" with the slide numbers.
- **METR's 2025 "19% slower" study.** Not used; METR itself labels those results out of date.
- Third-party talk recaps (pjfp.com, btbytes, potibo) were not used as sources for any claim.

## Corrections to the pitch (for the writer)
- "11,000 pull requests in one month" is right in substance, but say what it is: about 11,000 (10,926 on the slide) **merged** PRs in **October 2026**, counting **all contributors** to Grok Bot (about 227 people, including drive-by contributors), team-reported. It is not an agent-only count.
- "A revert rate around 0.5%": the slide measures **"% of commits reverted"** (0.47% in October, down from 0.98% in June). Tan says it "is steady at about half a percent." Don't call it an error rate or a quality score, and keep the revert counterpoint in.
- The clip's caption is AI Engineer's wording. Quote Tan's spoken words or her slides, not the caption.
- Don't write "daily stable releases" as fact. Use her "about once a day" or the slide numbers (15 releases in October, median 28 hours apart).
- "Apply equally to human and agent work": source this to Tan's Oct 12 posts (claim 6), not the talk. The talk shows the checks applying to every contributor's PR but doesn't make that statement.
- The talk ends by pitching specific products as the "outer loop" (Grok Bot routines, Cursor cloud agents and projects). Leave that out. Keep the checks generic and tool-agnostic, and don't attribute any tool or workflow to Jon.
- Tan's evidence shows the checks came before the volume and the two coincided. Don't claim the checks are proven to cause low reverts.
- Last week's lesson (W45 look-back): numbered checks drove read-through, and every brief counterpoint must be used or explicitly dropped in the outline.

# Package: Put the boring checks in before you scale agent volume

## Title options (pick 1)
1. **Put the boring checks in before you scale agent volume** ← pick
2. More agent volume is not proof your process works
3. Five boring checks before you let agent volume rise

## Hooks (3)
1. More volume is not proof the process is fine. It mostly makes the process louder. *(the piece's own line)*
2. Lauren Tan's team reports 10,926 merged PRs in October from all contributors, and 0.47% of commits reverted. Team-reported, unaudited, one team. Here are the boring checks her team leans on, and what those numbers do not prove. *(number, with its limits)*
3. Take the last review comment you wrote twice and turn it into a check. That is one of five boring checks to put in before you let agent volume rise. *(action)*

## Format note
This week's X version is one long-form X Article plus a short teaser post, not a thread, as 01-topic.md sets out ("a single X Article on @JonLotti, saved as a draft only, plus a short teaser post. No thread."). The template's "Thread version" section is replaced by the Article on purpose. The X Article draft on @JonLotti is `2122386087586750464` (unpublished), built from the 0b8726f final. Jon approves publish Friday. Draft `2122383968922124288` (built from the earlier ac33e9a final) is stale and should be deleted by hand in X's editor, because the connector can't delete drafts. The connector cannot read drafts back, so open the draft in X's editor and check the layout before approving. In the draft, each bracketed source marker such as [11] links to that source's first URL, and the Sources list at the end links every URL. After the Article is live, put its permalink in the teaser where `ARTICLE_URL` appears (X counts that URL as 23 characters). The teaser below is counted with that slot included (263 / 280).

Packaging notes followed: the clip caption's wording ("11,000 pull requests in one month," "revert rate around 0.5%," "daily stable releases") is kept out of the teaser, hooks and clip takes; figures are framed as team-reported and unaudited; the commits vs PRs mismatch stays in; the fuzzing example's product stays unnamed; no causal claim and no tool names in the teaser or hooks; the Grok Bot 1.0 trailer is a clip take only, not the hook.

## Article
### Title
Put the boring checks in before you scale agent volume

### Body
Same text as `04-final.md` at 0b8726f (after Edie's Pass 2), unchanged, sources list included.

Lauren Tan's team reports 10,926 merged pull requests in October 2026, up from 809 in June [11]. That count covers everyone who contributed to the Grok Bot team's code, about 227 people, many of them "casual or drive-by contributors who don't always have a lot of context" [11][13]. It is not an agent-only number. Over the same months, the share of commits reverted fell from 0.98% in June to 0.47% in October [12]. All of these figures are team-reported and unaudited.

Most teams should not expect that result. DORA's 2024 report put it at "an estimated 7.2% reduction [in delivery stability] for every 25% increase in AI adoption" [16]. Its 2025 report calls AI "an amplifier, magnifying an organization's existing strengths and weaknesses" [17]. More volume is not proof the process is fine. It mostly makes the process louder.

Here are five boring checks that apply to every pull request no matter who or what wrote it (three that tooling enforces, one that asks for evidence, and one habit that keeps adding to the first three), plus a four-question test for whether they are in place before you let volume rise.

## Why the boring checks come first
Tan frames the job this way: "figuring out how to maintain or even improve the quality of your code while massively increasing your productivity." The trust she wants is "not blind trust but investing in your agents environment so you can trust that your agents are going to do the right thing" [1].

Her "inverse pyramid" says where that investment goes. In her words, "the first two layers are deterministic": the code itself (API design, architecture, refactoring) and "lint rules, type systems, compilers, or you know, different kinds of testing." They come first, because they "constrain what agents can do and force them to do the right thing by default." Runtime and formal verification come next. Prose rules for the agent come last, for "things that require judgment" [2].

In her written version, human review sits at the bottom: "at the rate agents land code, it's pretty much impossible to thoroughly review every PR, so spend that effort on the highest leverage point, designing an environment where agents do the right thing by default" [3].

None of this is new. In Tan's words: "we have always had lint rules, compilers with good diagnostics and strong type systems, LSPs, etc to help us write better code. there is no difference when agents write the code instead, you just need more of them, and stronger ones" [6]. The same checks serve people and agents alike.

## Check 1. Make the wrong thing hard
The codebase is the agent's biggest input, so its flaws spread. Workarounds and tech debt are "now likely to be just copied by the next agent since it looks like the established pattern." Tan's advice is to keep the codebase "as pristine as possible so that agents are always copying the good stuff" [5].

Architecture rules do the most work here. Her team banned a hard-to-use React API in product code, so that class of problem was "categorically eliminated, and we never need to catch that during code review again." Imports across one internal boundary are "forbidden or banned by our dependency graph analyzer and some lint rules" [7]. Pick the one mistake your reviewers catch most, and ask whether a rule could make it hard to repeat.

## Check 2. Lint rules that point at the root cause, not comments
Comments are not checks. Tan's agents used code comments to justify quick fixes, so the team "decided to just ban 99% of comments" (not all of them) because "they're not enforceable." They replaced them with lint rules whose error messages tell the agent "to fix the root cause" [8]. A good error message is an instruction the agent is far less likely to skip.

## Check 3. Types, compilers and tests
These are the oldest checks on the list and still part of the base of Tan's pyramid [2]. If they are weak, every later layer has less to stand on. Tan's point is that you need "more of them, and stronger ones" when agents write the code [6].

## Check 4. Let the agent run the code and show evidence
Runtime verification means "giving your agent a way to run the code for itself." Tan says review has "really shrunk into looking at verification artifacts instead," such as videos, screenshots and diagrams. Formal verification is a separate tool: her team uses it for "model checking of major user flows." It has found bugs, but she calls it "certainly not a silver bullet" [10]. Ask for evidence that the change works, not just a diff.

## Check 5. Turn every repeated correction into a check
"Whenever you're correcting your agent, think about how you can make that a deterministic check instead of adding another line to your rules ... it's far more reproducible when it's in code." Do it often enough and "you'll find that you have just less things to look out for in code review" [4].

To retire a bad habit, Tan gives an order: "create a lint rule to block new usages of the old pattern to stop the bleed, then open PRs to rewrite all previous patterns to the new one" [9]. Stop new cases first, then clean up old ones.

## The plain test: four questions before you let volume rise
This test is ours, built from Tan's examples and DORA's metrics. If any answer is no, fix that before you add more agents.

1. When someone corrects an agent, does it end in a new check rather than a new line of prose [4]?
2. Can a low-context contributor land a good PR? Tan's team had 49 people with exactly one PR in October [13], and she writes that maintainers "can adjust their codebase so that anyone, even randoms and non-technical colleagues, can write good PRs" [6].
3. Are you tracking reverts and hotfixes next to volume? DORA pairs throughput with instability metrics, including change fail rate: deployments needing immediate intervention, "likely resulting in a rollback of the changes or a 'hotfix'" [18].
4. Are stability and performance holding as volume rises? For stability, use DORA's terms: change fail rate (question 3) and deployment rework rate, "deployments that are unplanned but happen as a result of an incident in production" [18]. DORA's baseline is that delivery stability tends to fall as AI adoption rises [16]. For performance, Tan's team reports cold launch down 31% (2,669 ms to 1,831 ms) and median typing latency in a long chat down 61% (11.6 ms to 4.5 ms) from May to the slide's Nov 4 posting, while shipping 15 desktop releases in October with a median of 28 hours between them [14].

## What the numbers do not prove
A low revert rate does not prove the code is good, only that it was not rolled back. Tan's slide measures "% of commits reverted," while she says aloud that "the number of PRs that get reverted ... is steady at about half a percent." Neither says what counts as a revert or how long after merge it is counted [12]. DORA's change fail rate counts hotfixes as well as rollbacks [18], so a team that fixes forward can keep reverts low and still ship failures. Tan also says her team's fuzzing run opens fix PRs and auto-merges them [C1]. Our inference, not her claim: some fixes may arrive as new PRs rather than reverts.

PR count is not a quality measure, and it does not compare across teams. PR size varies, and Tan writes that "most of the volume of PRs i land are refactoring" [C2]. DORA favors small batches [16], so many small PRs can be a deliberate choice. Treating volume as the proof is the pitfall DORA calls "having one metric to rule them all" [18].

This is one team, self-reported, after a big investment. The numbers show that results coincided with the checks, not that the checks caused them. Tan says getting there took her "six months" [15], and she writes, "it isn't perfect of course and we do make mistakes" [C3].

Checks do not replace judgment. Tan keeps prose for "things that require judgment" [2], calls formal verification "not a silver bullet" [10], and moves human effort to designing the environment rather than removing it [3]. She exempts "mission critical 'hard' (eg embedded) software" from the usual tolerance for imperfect code [C4]. Her line that "most product code that we land no longer really requires deep human review" [C5] describes her team after these investments. It is not a general recommendation.

## Takeaway
Order matters. Tan's advice "before you jump into building out a software factory": improve the codebase whenever you correct your agent, and "make sure that your verification story is really strong ... if your inner coding loop produces slop, then automating that loop just produces more slop" [15]. Without the basics, DORA's data says more AI adoption usually means less stable delivery [16].

Two things you can do this week: take the last review comment you wrote twice and turn it into a check [4], and put reverts and hotfixes on the same dashboard as PR volume [18].

## Sources
- [1] https://www.youtube.com/watch?v=O_zcc6Xl12g&t=68s
- [2] https://www.youtube.com/watch?v=O_zcc6Xl12g&t=123s
- [3] https://x.com/poteto/status/2111133080526495985
- [4] https://www.youtube.com/watch?v=O_zcc6Xl12g&t=192s ; https://www.youtube.com/watch?v=O_zcc6Xl12g&t=550s
- [5] https://www.youtube.com/watch?v=O_zcc6Xl12g&t=264s
- [6] https://x.com/poteto/status/2109699980248408574 ; https://x.com/poteto/status/2109761952696483905
- [7] https://www.youtube.com/watch?v=O_zcc6Xl12g&t=326s
- [8] https://www.youtube.com/watch?v=O_zcc6Xl12g&t=500s ; https://x.com/poteto/status/2110758788525621282
- [9] https://x.com/poteto/status/2110161793331208527 ; https://www.youtube.com/watch?v=O_zcc6Xl12g&t=911s
- [10] https://www.youtube.com/watch?v=O_zcc6Xl12g&t=580s
- [11] https://www.youtube.com/watch?v=O_zcc6Xl12g&t=812s ; https://x.com/poteto/status/2118017093677494706 ; https://x.com/poteto/status/2118051545468301479
- [12] https://www.youtube.com/watch?v=O_zcc6Xl12g&t=854s ; https://x.com/aiDotEngineer/status/2121981562824564960
- [13] https://www.youtube.com/watch?v=O_zcc6Xl12g&t=835s ; https://x.com/poteto/status/2115133011352240581
- [14] https://www.youtube.com/watch?v=O_zcc6Xl12g&t=870s ; https://x.com/poteto/status/2118017093677494706 ; https://x.com/aiDotEngineer/status/2121981562824564960
- [15] https://www.youtube.com/watch?v=O_zcc6Xl12g&t=911s ; https://www.youtube.com/watch?v=O_zcc6Xl12g&t=100s
- [16] https://dora.dev/research/2024/dora-report/2024-dora-accelerate-state-of-devops-report.pdf
- [17] https://dora.dev/research/2025/dora-report/
- [18] https://dora.dev/guides/dora-metrics-four-keys/
- [C1] https://www.youtube.com/watch?v=O_zcc6Xl12g&t=981s
- [C2] https://x.com/poteto/status/2109361189071499640
- [C3] https://x.com/poteto/status/2115133011352240581
- [C4] https://x.com/poteto/status/2109110547824378140
- [C5] https://www.youtube.com/watch?v=O_zcc6Xl12g&t=1004s

## Teaser post
Each URL counts as 23 characters. Replace `ARTICLE_URL` with the Article permalink after publish. Counted length: 263 / 280.

```
Lauren Tan's team reports 10,926 merged PRs in October from all contributors, and 0.47% of commits reverted. Team-reported, one team.

Volume is not proof your process works. Here are five boring checks to put in before agent volume rises:
ARTICLE_URL
```

## Images
| File | Alt text |
|---|---|
| assets/lotti-pose-laptop-circle.jpg | Lotti, a man with curly dark hair and a mustache, wearing an orange hoodie, typing on a laptop at a wooden desk, a steaming white coffee mug beside him, inside an orange circle. |
| assets/lotti-pose-thinking.jpg | Lotti in an orange hoodie, chin in hand, looking up at a glowing lightbulb against an orange circle. |
| assets/lotti-pose-cheer.jpg | Lotti in an orange hoodie with both arms raised and a big smile, confetti falling around him, against an orange circle. |

Suggested pairing: laptop pose at the top of the Article, thinking pose near the four-question test, cheer pose near "Two things you can do this week."

## Channel versions
### X (launch channel)
Publish the Article first, then the teaser with the Article permalink. X is the only launch channel this week. Do not publish until both approval boxes below are checked. An unpublished draft is already saved on @JonLotti (see format note). Do not publish, post the teaser, or edit or delete other drafts.

### Later (not yet active): TikTok, LinkedIn, YouTube Shorts
Not active yet.

## Clip takes
For each clip the lead kept in `01-topic.md`. Jon clips and posts after approval; we do not post. X Clipping credits and links the original video. Timestamps are not verified, so the takes describe the moment rather than citing a clock mark.

### Clip 1
- **Source post URL:** https://x.com/aiDotEngineer/status/2121981562824564960 (official AI Engineer CODE summit clip, about 91 seconds, Tan's results section)
- **Take (247 / 280):** Lauren Tan's team reports 10,926 merged PRs in October from all contributors, with 0.47% of commits reverted. Team-reported, and her slide says commits while she says PRs. A low revert rate shows what wasn't rolled back, not that the code is good.

### Clip 2 (optional standalone, not the hook)
- **Source post URL:** https://x.com/bot/status/2120582957782200586 (official Grok Bot 1.0 trailer, about 79 seconds)
- **Take (175 / 280):** The Grok Bot 1.0 trailer frames bots as teammates you can share and invite to meetings. If they're teammates, their work should pass the same boring checks as everyone else's.

## Approval
- [ ] Lead approved
- [ ] Human approved publish

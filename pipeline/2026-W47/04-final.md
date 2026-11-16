# Put the boring checks in before you scale agent volume

Lauren Tan's team reports 10,926 merged pull requests in October 2026, up from 809 in June [11]. That count covers everyone who contributed to the Grok Bot team's code, about 227 people, many of them "casual or drive-by contributors who don't always have a lot of context" [11][13]. It is not an agent-only number. Over the same months, the share of commits reverted fell from 0.98% in June to 0.47% in October [12]. All of these figures are team-reported and unaudited.

Most teams should not expect that result. DORA's 2024 report put it at "an estimated 7.2% reduction [in delivery stability] for every 25% increase in AI adoption" [16]. Its 2025 report calls AI "an amplifier, magnifying an organization's existing strengths and weaknesses" [17]. More volume is not proof the process is fine. It mostly makes the process louder.

Here are five boring, deterministic checks that apply to every pull request no matter who or what wrote it, plus a four-question test for whether they are in place before you let volume rise.

## Why the boring checks come first
Tan frames the job this way: "figuring out how to maintain or even improve the quality of your code while massively increasing your productivity." The trust she wants is "not blind trust but investing in your agents environment so you can trust that your agents are going to do the right thing" [1].

Her "inverse pyramid" says where that investment goes. The code itself (API design, architecture, refactoring) and static checks (lint rules, type systems, compilers, testing) come first, because they "constrain what agents can do and force them to do the right thing by default." Runtime and formal verification come next. Prose rules for the agent come last, for "things that require judgment" [2].

In her written version, human review sits at the bottom: "at the rate agents land code, it's pretty much impossible to thoroughly review every PR, so spend that effort on the highest leverage point, designing an environment where agents do the right thing by default" [3].

None of this is new. In Tan's words: "we have always had lint rules, compilers with good diagnostics and strong type systems, LSPs, etc to help us write better code. there is no difference when agents write the code instead, you just need more of them, and stronger ones" [6]. The same checks serve people and agents alike.

## Check 1. Make the wrong thing impossible
The codebase is the agent's biggest input, so its flaws spread. Workarounds and tech debt are "now likely to be just copied by the next agent since it looks like the established pattern." Tan's advice is to keep the codebase "as pristine as possible so that agents are always copying the good stuff" [5].

Architecture rules do the most work here. Her team banned a hard-to-use React API in product code, so that class of problem was "categorically eliminated, and we never need to catch that during code review again." Imports across one internal boundary are "forbidden or banned by our dependency graph analyzer and some lint rules" [7]. Pick the one mistake your reviewers catch most, and ask whether a rule could make it impossible.

## Check 2. Lint rules that point at the root cause, not comments
Comments are not checks. Tan's agents used code comments to justify quick fixes, so the team "decided to just ban 99% of comments" because "they're not enforceable." They replaced them with lint rules whose error messages tell the agent "to fix the root cause" [8]. A good error message is an instruction the agent cannot skip.

## Check 3. Types, compilers and tests
These are the oldest checks on the list and still part of the deterministic base of the pyramid [2]. If they are weak, every later layer has less to stand on. Tan's point is that you need "more of them, and stronger ones" when agents write the code [6].

## Check 4. Let the agent run the code and show evidence
Runtime verification means "giving your agent a way to run the code for itself." Tan says review has "really shrunk into looking at verification artifacts instead," such as videos, screenshots, diagrams and formal verification. Formal methods have found bugs, but she calls them "certainly not a silver bullet" [10]. Ask for evidence that the change works, not just a diff.

## Check 5. Turn every repeated correction into a check
"Whenever you're correcting your agent, think about how you can make that a deterministic check instead of adding another line to your rules ... it's far more reproducible when it's in code." Do it often enough and "you'll find that you have just less things to look out for in code review" [4].

To retire a bad habit, Tan gives an order: "create a lint rule to block new usages of the old pattern to stop the bleed, then open PRs to rewrite all previous patterns to the new one" [9]. Stop new cases first, then clean up old ones.

## The plain test: four questions before you let volume rise
This test is ours, built from Tan's examples and DORA's metrics. If any answer is no, fix that before you add more agents.

1. When someone corrects an agent, does it end in a new check rather than a new line of prose [4]?
2. Can a low-context contributor land a good PR? Tan's team had 49 people with exactly one PR in October [13], and she writes that maintainers "can adjust their codebase so that anyone, even randoms and non-technical colleagues, can write good PRs" [6].
3. Are you tracking reverts and hotfixes next to volume? DORA pairs throughput with instability metrics, including change fail rate: deployments needing immediate intervention, "likely resulting in a rollback of the changes or a 'hotfix'" [18].
4. Are stability and speed holding as volume rises? Tan's team reports cold launch down 31% (2,669 ms to 1,831 ms) and median typing latency in a long chat down 61% (11.6 ms to 4.5 ms) from May to the slide's Nov 4 posting, and 15 desktop releases in October with a median of 28 hours between them [14]. DORA's baseline is that stability tends to fall as AI adoption rises [16].

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

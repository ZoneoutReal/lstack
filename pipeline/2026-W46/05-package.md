# Package — Fix the harness before you switch models

## Title options (pick 1)
1. **Fix the harness before you switch models** ← pick
2. Audit the harness before you pay for a model swap
3. Four checks before you switch coding models

## Hooks (3)
1. Swapping the model when a coding agent disappoints is like replacing the engine when the problem is the dashboard, the checklist, and the toolbox. *(analogy; used as the Article opener and teaser lead)*
2. A 4-part harness audit you can run in about an hour: context, verification, state, and tools.
3. Seven harnesses, same model, same 20 tasks: pass rates 71.3% to 78.8%. Every planned head-to-head came back "can't tell apart." What moved was cost and speed.

## Format note
This week's X version is one long-form X Article plus a short teaser post, not a 21-post thread. The skill template still has a "Thread version" section; this replaces it on purpose. The aim is that an engineer or tech lead can read one clean piece and leave with the four-check harness audit and a reason to try it this week. Publish nothing until both approval boxes are checked. After the Article is live, put its permalink in the teaser where `ARTICLE_URL` appears (X counts that URL as 23 characters). The teaser below is counted with that slot included (246 / 280).

Revision (Nov 10): added the "Doesn't Claude just run best in Claude Code?" section, which answers Jon's objection, and checked it with Edie. The current X Article draft on @JonLotti is `2120019786893570048` (unpublished). The connector can't edit or delete drafts, so the earlier draft `2120000068115738624` is out of date and should be deleted in X's editor.

## Article
### Title
Fix the harness before you switch models

### Body

When a coding agent disappoints, the first move is often to swap the model. That's like replacing the engine when the problem is the dashboard, the checklist, and the toolbox.

A coding agent is the model plus a harness: the prompts, tools, context policies, hooks, sandboxes, subagents, feedback loops and recovery paths wrapped around it. A raw model is not an agent until that scaffolding gives it state, tool execution, feedback and constraints. [Addy Osmani writes about that scaffolding here](https://addyosmani.com/blog/agent-harness-engineering/).

Here's a four-part audit you can run on your own setup in about an hour: context, verification, state and progress files, and tools. It will tell you whether to change the harness or the model. That's the check I would run before paying for a swap.

Don't expect a harness swap to lift pass rate on its own. In [Garry Tan's evaluation](https://github.com/garrytan/g-harness-evals/blob/1c26ae409de0c90c32f5becd33a2aa7c311e7ef7/docs/benchmarks/2026-11-04-matrix-mu/report.md), holding the model and the tasks fixed, seven harness cells on 20 public multi-user tasks posted pass rates from 71.3% to 78.8%. All six planned head-to-head comparisons came back "can't tell apart." The observed gaps were 0 to 3.9 points, below the run's 7.7 to 14.2 point minimum detectable difference. Fourteen of those 20 tasks scored the same in every cell: 11 passed on every repetition in every harness, and 3 never passed in any cell. Those three were all corrections tasks. The report's verdict is to raise the ceiling and rerun on harder tasks, because "the tasks, not the harness, decide most of the score." The model still sets that ceiling.

What moved in Tan's run was cost and speed. On the same Opus 5.5 model, his report posted cost per solved task of about $0.19 for QM, $0.22 for Claude Code, $0.24 for Hermes Agent and $0.44 for OpenClaw, roughly twice as much for OpenClaw. Median time per trial ran from 40.1 seconds (Claude Code and QM) to 99.4 seconds (OpenClaw). On GPT-6.1 Sol, the Codex, OpenClaw and Hermes cells ran $0.17 to $0.22 per solved task (a descriptive range, with no cost test). "Fix the harness before you switch models" is not a promise that your pass rate will jump. On that set, it is a way to stop paying extra time and money for the same result.

Those figures are labeled dev results on public tasks at pinned versions, not held-out confirmation. Claude Code and Codex were never compared with each other, because each can run only its own model. In that evaluation, two OpenClaw cells were incomplete, and QM ran on a different Docker network, so its pairs were not tested. Tan discloses that he runs the evaluation and related projects, that QM is a Y Combinator project, and that Y Combinator is an investor in Hermes.

## "Doesn't Claude just run best in Claude Code?"

That's the first objection an expert will raise, and it's a fair one. The short answer is: not by default, and not because of the logo.

On Terminal-Bench 2.0, a harder, re-verified set of 89 container tasks scored as agent-model pairs, the same Claude Opus 4.6 model scored 58.0% in Claude Code and 62.9% in Terminus 2, the benchmark's reference harness. The same GPT-5.3-Codex model did better in its own lab's harness: 73.3% with Codex CLI against 64.7% with Terminus 2. Then [Terminal-Bench 2.1](https://www.tbench.ai/news/terminal-bench-2-1) fixed issues in 28 of the 89 tasks, and Claude Code with Opus 4.6 moved from 58.0% to 70.1% while Terminus 2 with Opus 4.6 moved from 62.9% to 63.8%. The lead flipped without changing the model, so some of what looks like a harness win is a benchmark artifact. Leaderboard rows can also differ in date, token budget and reasoning effort; they are not a randomized swap of the harness alone.

Claude Code's own layers can be load-bearing, and you can inspect which ones. In Tan's results on harder v0.4 tasks, removing Claude Code's memory-and-skills text and tool-description advice together took its pass rate from 60.4% to 0.0% (more on that under Context below). Anthropic describes tuning its harness to what each model can't yet do on its own, and taking pieces out as models improve. A lab's own harness includes layers like those, and they're the same layers the four checks below have you inspect. You can build them into your own setup instead of hoping a model swap does it for you.

## 1. Context

What is injected every turn: the system prompt, files like `AGENTS.md` or `CLAUDE.md`, tool schemas, memory files? How large is it? Are huge tool outputs re-sent in full?

Osmani describes context rot, models getting worse as the window fills, and the usual countermeasures: compaction, offloading large tool results to disk, and loading skills only when needed. In [a separate cost run Tan published on the same 20 tasks](https://github.com/garrytan/g-harness-evals/blob/1c26ae409de0c90c32f5becd33a2aa7c311e7ef7/findings/harness-cost/README.md), Claude Code cost $0.165 less per trial than OpenClaw on Opus 5.5, at the same 80% pass rate. About 81% of that gap was cache writes: in that run, OpenClaw re-sends a much bigger system prompt and bigger tool results. A heavier harness can cost much more for the same measured pass rate.

Trimming is not free, though. On harder v0.4 tasks, [Tan found](https://github.com/garrytan/g-harness-evals/blob/1c26ae409de0c90c32f5becd33a2aa7c311e7ef7/findings/prompt-cuts/README.md) that removing Claude Code's memory-and-skills text and tool-description advice together dropped its pass rate from 60.4% to 0.0%. The two layers were cut together, so the loss cannot be pinned on one of them. The full prompt wrote auto-memory files in 37 of 48 trials, and every one of its 29 passes had them; the cut arms wrote none in 96 trials.

Also check where a must-follow rule actually lives. In [Tan's rule-placement results](https://github.com/garrytan/g-harness-evals/blob/1c26ae409de0c90c32f5becd33a2aa7c311e7ef7/findings/rule-placement/README.md), a rule the agent sees every turn (a per-turn hook, the system prompt, or the startup file) was followed in 30 of 30 member turns on Codex, Hermes Agent and OpenClaw running GPT-6.1 Sol. A rule given once faded: 2 of 10 later turns on Hermes, and 4 of 10 on OpenClaw. These rule-placement figures are dev results on 10 public tasks, one repetition.

## 2. Verification

What, other than the builder, is allowed to call the work done?

When agents evaluate work they have just produced, they tend to praise it even when the quality is mediocre. [Anthropic separated a planner, a generator and a standalone evaluator](https://www.anthropic.com/research/harness-design-long-running-apps) so the builder was not the only judge. They also [saw agents mark features complete after unit tests or `curl` checks](https://www.anthropic.com/research/effective-harnesses-for-long-running-agents) without confirming the product worked end-to-end.

Look for hooks that run typecheck, lint or tests and feed failures back; a done-list that starts as failing; and, if you have it, a separate evaluator with no write access to the code it is grading.

A heavier setup is not automatically the right call. In one Opus 4.5 comparison from Anthropic's harness-design write-up, a solo run took 20 minutes and $9 and produced a retro game maker whose play mode did not respond to input; the full harness took 6 hours and $200 and produced a playable game, though the physics were still rough. Cost is part of the decision, not just the headline score.

## 3. State and progress files

Can a fresh session reconstruct where the last one stopped without guessing? Each new agent session starts with no memory of what came before.

[Anthropic's working pattern](https://www.anthropic.com/research/effective-harnesses-for-long-running-agents) is a progress file, a feature list that starts with every item marked failing, git history with descriptive commits, and a startup script. An initializer agent sets up an `init.sh` script, a `claude-progress.txt` log, that failing feature list, and an initial git commit; later coding agents read those artifacts, do one feature at a time, then leave a commit and a progress update. Compaction alone was not enough: even Opus 4.5 on the Claude Agent SDK fell short of building a production-quality web app from a high-level prompt. If your agent "finishes" a multi-hour job in one context window, or leaves half-written work undocumented, this layer is missing.

The useful harness space moves as models improve, rather than shrinking. In [their later write-up on harness design](https://www.anthropic.com/research/harness-design-long-running-apps), Anthropic dropped context resets after Opus 4.5 largely removed the "context anxiety" that had made resets essential for Sonnet 4.5, and later removed the sprint decomposition Opus 4.5 had needed once Opus 4.6 could run coherently for more than two hours without it. Every component encodes an assumption about what the model cannot do on its own. When that assumption no longer holds, the scaffolding should come out.

## 4. Tools

How many tools are on the menu, and does the agent actually use the ones you rely on?

In Tan's rule-placement work, an unmentioned skill sat unread on Claude Code and on Hermes, 0 opens in 30 turns, until the prompt named it, which got Claude Code to follow the rule in 30 of 30 turns. Anthropic saw better bug-finding once the agent had browser tools and was told to test as a user would. Prefer a short, named tool list over a pile of overlapping MCP servers.

## Takeaway

Run the four checks on your own setup before you pay for a model swap. If the same hard tasks fail in every harness, as three corrections tasks did across Tan's matrix, on Opus 5.5 and on GPT-6.1 Sol, I would not reach for another wrapper first. The next move may be a stronger model, a better verifier, or a different task breakdown.

Treat public leaderboard gaps with care, for the Terminal-Bench reasons above: some of what looks like a harness win is a benchmark artifact.

The measurement I would try this week is simple: ten of your own recent tickets, with and without your current progress-file and test-hook setup.

## Teaser post
Each URL counts as 23 characters. Replace `ARTICLE_URL` with the Article permalink after publish. Counted length: 246 / 280.

```
When a coding agent disappoints, swapping the model is like replacing the engine when the problem is the dashboard, the checklist, and the toolbox.

I wrote up a 4-part harness audit you can run in about an hour this week.
ARTICLE_URL
```

## Images
| File | Alt text |
|---|---|
| assets/lotti-pose-thinking.jpg | Lotti, a man with curly dark hair and a mustache, wearing an orange hoodie, chin in hand, looking up at a glowing lightbulb against an orange circle. |
| assets/lotti-pose-laptop.jpg | Lotti in an orange hoodie typing on a laptop at a wooden desk, a steaming white coffee mug beside him, against an orange circle. |
| assets/lotti-pose-thumbsup.jpg | Lotti in an orange hoodie giving a thumbs-up and a slight smile, against an orange circle. |

Suggested pairing: thinking pose at the top of the Article, laptop pose near the four checks, thumbs-up near the takeaway.

## Channel versions
### X (launch channel)
Publish the Article first, then the teaser with the Article permalink. X is the only launch channel this week. Do not publish until both approval boxes below are checked. Do not create an X draft from this file until a human asks.

### Later (not yet active): TikTok, LinkedIn, YouTube Shorts
Not active yet.

## Approval
- [ ] Lead approved
- [ ] Human approved publish

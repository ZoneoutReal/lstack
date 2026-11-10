# Fix the harness before you switch models

When a coding agent disappoints, the first move is often to swap the model. That is like replacing the engine when the problem is the dashboard, the checklist, and the toolbox. A coding agent is the model plus a harness: the prompts, tools, context policies, hooks, sandboxes, subagents, feedback loops and recovery paths wrapped around it. A raw model is not an agent until that scaffolding gives it state, tool execution, feedback and constraints [1].

Here is a four-part audit — context, verification, state and progress files, and tools — you can run on your own setup in about an hour. It will tell you whether to change the harness or the model.

Do not expect a harness swap to lift pass rate on its own. Holding the model and the tasks fixed, seven harness cells on 20 public multi-user tasks posted pass rates from 71.3% to 78.8%. All six planned head-to-head comparisons came back “can’t tell apart.” The observed gaps were 0 to 3.9 points, below the run’s 7.7 to 14.2 point minimum detectable difference [2]. Fourteen of those 20 tasks scored the same in every cell: 11 passed on every repetition in every harness, and 3 never passed in any cell. Those three were all corrections tasks. The report’s verdict is to raise the ceiling and rerun on harder tasks, because “the tasks, not the harness, decide most of the score” [4]. The model still sets that ceiling.

What did move was cost and speed. On the same Opus 5.5 model, cost per solved task was about $0.19 for QM, $0.22 for Claude Code, $0.24 for Hermes Agent and $0.44 for OpenClaw — roughly twice as much for OpenClaw. Median time per trial ran from 40.1 seconds (Claude Code and QM) to 99.4 seconds (OpenClaw). On GPT-6.1 Sol, Codex, OpenClaw and Hermes ran $0.17 to $0.22 per solved task (a descriptive range, with no cost test) [3]. “Fix the harness before you switch models” is not a promise that your pass rate will jump. On this set, it is a way to stop paying extra time and money for the same result.

Those figures are labeled dev results on public tasks at pinned versions, not held-out confirmation. Claude Code and Codex were never compared with each other, because each can run only its own model. Two OpenClaw cells were incomplete, and QM ran on a different Docker network, so its pairs were not tested. Tan discloses that he runs the evaluation and related projects, that QM is a Y Combinator project, and that Y Combinator is an investor in Hermes.

## 1. Context
What is injected every turn — the system prompt, files like `AGENTS.md` or `CLAUDE.md`, tool schemas, memory files? How large is it? Are huge tool outputs re-sent in full?

Osmani describes context rot and the usual countermeasures: compaction, offloading large tool results to disk, and loading skills only when needed [1]. In a separate cost run on the same 20 tasks, Claude Code cost $0.165 less per trial than OpenClaw on Opus 5.5, at the same 80% pass rate. About 81% of that gap was cache writes: OpenClaw re-sends a much bigger system prompt and bigger tool results [6]. A heavier harness can cost much more for the same measured pass rate.

Trimming is not free, though. On harder tasks, removing Claude Code’s memory-and-skills text and tool-description advice together dropped its pass rate from 60.4% to 0.0%. The two layers were cut together, so the loss cannot be pinned on one of them. The full prompt wrote auto-memory files in 37 of 48 trials, and every one of its 29 passes had them; the cut arms wrote none in 96 trials [5].

Also check where a must-follow rule actually lives. A rule the agent sees every turn — a per-turn hook, the system prompt, or the startup file — was followed in 30 of 30 member turns on Codex, Hermes Agent and OpenClaw running GPT-6.1 Sol. A rule given once faded: 2 of 10 later turns on Hermes, and 4 of 10 on OpenClaw. These rule-placement figures are dev results on 10 public tasks, one repetition [12].

## 2. Verification
What, other than the builder, is allowed to call the work done?

When agents evaluate work they have just produced, they tend to praise it even when the quality is mediocre. Anthropic separated a planner, a generator and a standalone evaluator so the builder was not the only judge [10]. They also saw agents mark features complete after unit tests or `curl` checks without confirming the product worked end-to-end [9].

Look for hooks that run typecheck, lint or tests and feed failures back; a done-list that starts as failing; and, if you have it, a separate evaluator with no write access to the code it is grading.

A heavier setup is not automatically the right call. In one Opus 4.5 comparison, a solo run took 20 minutes and $9 and produced a retro game maker whose play mode did not respond to input; the full harness took 6 hours and $200 and produced a playable game, though the physics were still rough [10]. Cost is part of the decision, not just the headline score.

## 3. State and progress files
Can a fresh session reconstruct where the last one stopped without guessing? Each new agent session starts with no memory of what came before [9].

Anthropic’s working pattern is a progress file, a feature list that starts with every item marked failing, git history with descriptive commits, and a startup script. An initializer agent sets up an `init.sh` script, a `claude-progress.txt` log, that failing feature list, and an initial git commit; later coding agents read those artifacts, do one feature at a time, then leave a commit and a progress update. Compaction alone was not enough: even Opus 4.5 on the Claude Agent SDK fell short of building a production-quality web app from a high-level prompt [9]. If your agent “finishes” a multi-hour job in one context window, or leaves half-written work undocumented, this layer is missing.

The useful harness space moves as models improve, rather than shrinking. Anthropic dropped context resets after Opus 4.5 largely removed the “context anxiety” that had made resets essential for Sonnet 4.5, and later removed the sprint decomposition Opus 4.5 had needed once Opus 4.6 could run coherently for more than two hours without it [11]. Every component encodes an assumption about what the model cannot do on its own. When that assumption no longer holds, the scaffolding should come out.

## 4. Tools
How many tools are on the menu, and does the agent actually use the ones you rely on?

An unmentioned skill sat unread on Claude Code and on Hermes — 0 opens in 30 turns — until the prompt named it, which got Claude Code to 30 of 30 [12]. Anthropic saw better bug-finding once the agent had browser tools and was told to test as a user would [9]. Prefer a short, named tool list over a pile of overlapping MCP servers.

## Takeaway
Run the four checks on your own setup before you pay for a model swap. If the same hard tasks fail in every harness — as three corrections tasks did across Tan’s matrix, on Opus 5.5 and on GPT-6.1 Sol [4] — the next move may be a stronger model, a better verifier, or a different task breakdown, not another wrapper.

Treat public leaderboard gaps with care. Terminal-Bench 2.0 is a harder, re-verified set of 89 container tasks, scored as agent-model pairs rather than as models alone. On that set, the same GPT-5.3-Codex model scored 73.3% with Codex CLI and 64.7% with Terminus 2, an 8.6-point gap. The same Claude Opus 4.6 model scored 58.0% with Claude Code and 62.9% with Terminus 2 [7]. Terminal-Bench 2.1 then fixed issues in 28 of those 89 tasks. After the task fixes, Claude Code with Opus 4.6 moved from 58.0% to 70.1% (+12.1 points), the largest gain reported, while Terminus 2 with Opus 4.6 moved from 62.9% to 63.8% (+0.9). The lead between those two harnesses flipped without changing the model [8]. Some of what looks like a harness win is a benchmark artifact. Leaderboard rows can also differ in date, token budget and reasoning effort; they are not a randomized swap of the harness alone.

A cheap first measurement: ten of your own recent tickets, with and without your current progress-file and test-hook setup, before you pay for a model swap.

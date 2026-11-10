# Package — Fix the harness before you switch models

## Title options (pick 1)
1. **Fix the harness before you switch models** ← pick
2. Audit the harness before you pay for a model swap
3. Four checks before you switch coding models

## Hooks (3)
1. Swapping the model when a coding agent disappoints is like replacing the engine when the problem is the dashboard, the checklist, and the toolbox. *(analogy; used as the thread opener)*
2. A 4-part harness audit you can run in about an hour: context, verification, state, and tools.
3. Seven harnesses, same model, same 20 tasks: pass rates 71.3% to 78.8%. Every planned head-to-head came back "can't tell apart." What moved was cost and speed.

## Thread version
Each post is within X's 280-character limit (URLs count as 23).

1/ Swapping the model when a coding agent disappoints is like replacing the engine when the problem is the dashboard, the checklist, and the toolbox.

A 4-part harness audit you can run in about an hour 🧵

*(205 characters)*

2/ A coding agent is the model plus a harness: prompts, tools, context policies, hooks, sandboxes, subagents, feedback loops and recovery paths. A raw model is not an agent until that scaffolding gives it state, tool execution, feedback and constraints.
https://addyosmani.com/blog/agent-harness-engineering/

*(277 characters)*

3/ Same model, same 20 public tasks, 7 harnesses: pass rates from 71.3% to 78.8%. All 6 planned head-to-heads came back "can't tell apart." Gaps were 0 to 3.9 points, below the run's 7.7 to 14.2 point minimum detectable difference.
https://github.com/garrytan/g-harness-evals/blob/1c26ae409de0c90c32f5becd33a2aa7c311e7ef7/docs/benchmarks/2026-11-04-matrix-mu/report.md

*(255 characters)*

4/ 14 of those 20 tasks scored the same in every cell: 11 always passed, 3 never did (all corrections tasks). The report's verdict is to raise the ceiling and rerun on harder tasks, because "the tasks, not the harness, decide most of the score." The model still sets that ceiling.

*(280 characters)*

5/ What moved was cost and speed. On Opus 5.5, cost per solved task was about $0.19 QM, $0.22 Claude Code, $0.24 Hermes Agent and $0.44 OpenClaw: roughly twice as much for OpenClaw. Median time per trial: 40.1 seconds (Claude Code and QM) to 99.4 seconds (OpenClaw).

*(266 characters)*

6/ That is not a promise your pass rate will jump. These are labeled dev results on public tasks at pinned versions, not held-out confirmation. Tan discloses he runs the eval, QM is a Y Combinator project, and Y Combinator invests in Hermes.

*(241 characters)*

7/ 1. Context. What is injected every turn: the system prompt, files like AGENTS.md or CLAUDE.md, tool schemas, memory files? How large is it? Are huge tool outputs re-sent in full?

*(181 characters)*

8/ Claude Code cost $0.165 less per trial than OpenClaw on Opus 5.5, at the same 80% pass rate. About 81% of that gap was cache writes: OpenClaw re-sends a much bigger system prompt and bigger tool results.
https://github.com/garrytan/g-harness-evals/blob/1c26ae409de0c90c32f5becd33a2aa7c311e7ef7/findings/harness-cost/README.md

*(230 characters)*

9/ Trimming is not free. On harder v0.4 tasks, removing Claude Code's memory-and-skills text and tool-description advice together dropped its pass rate from 60.4% to 0.0%. The two layers were cut together, so the loss cannot be pinned on one of them.
https://github.com/garrytan/g-harness-evals/blob/1c26ae409de0c90c32f5becd33a2aa7c311e7ef7/findings/prompt-cuts/README.md

*(274 characters)*

10/ A rule the agent sees every turn was followed in 30 of 30 member turns on Codex, Hermes Agent and OpenClaw running GPT-6.1 Sol. A rule given once faded: 2 of 10 later turns on Hermes, 4 of 10 on OpenClaw. Dev results, 10 public tasks, one repetition.
https://github.com/garrytan/g-harness-evals/blob/1c26ae409de0c90c32f5becd33a2aa7c311e7ef7/findings/rule-placement/README.md

*(278 characters)*

11/ 2. Verification. What, other than the builder, is allowed to call the work done? Agents tend to praise work they just produced even when it is mediocre. Anthropic separated a planner, a generator and an evaluator so the builder was not the only judge.
https://www.anthropic.com/research/harness-design-long-running-apps

*(279 characters)*

12/ Agents marked features complete after unit tests or curl checks without an end-to-end check. Look for typecheck, lint or test hooks that feed failures back; a done-list that starts failing; and an evaluator with no write access to the code it grades.
https://www.anthropic.com/research/effective-harnesses-for-long-running-agents

*(278 characters)*

13/ In one Opus 4.5 comparison, a solo run took 20 minutes and $9 and produced a retro game maker whose play mode did not respond to input. The full harness took 6 hours and $200 and produced a playable game, though the physics were still rough. Cost is part of the decision.

*(275 characters)*

14/ 3. State and progress files. Can a fresh session reconstruct where the last one stopped without guessing? Each new session starts with no memory of what came before. Anthropic's pattern: a progress file, a failing feature list, descriptive git commits, and a startup script.

*(278 characters)*

15/ Harness space moves as models improve. Anthropic dropped context resets after Opus 4.5 largely removed the context anxiety that made resets essential for Sonnet 4.5, then removed the sprint decomposition Opus 4.5 needed once Opus 4.6 could run coherently for over two hours.

*(278 characters)*

16/ 4. Tools. How many tools are on the menu, and does the agent actually use the ones you rely on? An unmentioned skill sat unread on Claude Code and on Hermes (0 opens in 30 turns) until the prompt named it, which got Claude Code to follow the rule in 30 of 30 turns.

*(269 characters)*

17/ Anthropic saw better bug-finding once the agent had browser tools and was told to test as a user would. Prefer a short, named tool list over a pile of overlapping MCP servers.

*(179 characters)*

18/ Run the four checks before you pay for a model swap. If the same hard tasks fail in every harness, as 3 corrections tasks did across Tan's matrix, the next move may be a stronger model, a better verifier, or a different task breakdown, not another wrapper.

*(260 characters)*

19/ Treat leaderboard gaps with care. Terminal-Bench 2.0 is 89 container tasks, scored as agent-model pairs. Same GPT-5.3-Codex model: 73.3% with Codex CLI vs 64.7% with Terminus 2. Same Claude Opus 4.6: 58.0% with Claude Code vs 62.9% with Terminus 2.
https://www.tbench.ai/news/terminal-bench-2-1

*(276 characters)*

20/ Terminal-Bench 2.1 fixed issues in 28 of those 89 tasks. After the fixes, Claude Code with Opus 4.6 moved from 58.0% to 70.1% (+12.1, the largest gain reported). Terminus 2 with Opus 4.6 moved from 62.9% to 63.8% (+0.9). The lead flipped without changing the model.

*(269 characters)*

21/ A cheap first measurement: ten of your own recent tickets, with and without your current progress-file and test-hook setup.

*(127 characters)*

## Images
| File | Alt text |
|---|---|
| assets/lotti-pose-thinking.jpg | Lotti, a man with curly dark hair and a mustache, wearing an orange hoodie, chin in hand, looking up at a glowing lightbulb against an orange circle. |
| assets/lotti-pose-laptop.jpg | Lotti in an orange hoodie typing on a laptop at a wooden desk, a steaming white coffee mug beside him, against an orange circle. |
| assets/lotti-pose-thumbsup.jpg | Lotti in an orange hoodie giving a thumbs-up and a slight smile, against an orange circle. |

Suggested pairing: thinking pose on 1/, laptop pose on the four checks (7/, 11/, 14/, 16/), thumbs-up on 21/.

## Channel versions
### X (launch channel)
Post the thread above. It is the only launch channel this week. Do not publish until both approval boxes below are checked.

### Later (not yet active): TikTok, LinkedIn, YouTube Shorts
Not active yet.

## Approval
- [ ] Lead approved
- [ ] Human approved publish

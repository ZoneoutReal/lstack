# Edit — 2026-W46

## Fact-check
| Claim | Brief # | Verified |
|---|---|---|
| Agent = model + harness (prompts, tools, context policies, hooks, sandboxes, subagents, feedback loops, recovery paths); a raw model is not an agent until scaffolding gives it state, tool execution, feedback and constraints | 1 | ✅ Osmani |
| Seven harness cells on 20 public multi-user tasks: pass rates 71.3% to 78.8%; all six pairs “can’t tell apart”; observed gaps 0 to 3.9 points, below MDD 7.7 to 14.2 | 2 | ✅ matrix report |
| 14 of 20 tasks scored the same in every cell: 11 always passed, 3 never passed (all corrections); verdict is raise the ceiling and rerun on harder tasks; quote “the tasks, not the harness, decide most of the score” | 4 | ✅ counts and verdict in the matrix report; quoted phrase is the scoreboard glossary definition of a saturated task set, same pin |
| Opus 5.5 cost per solved task about $0.19 QM, $0.22 Claude Code, $0.24 Hermes Agent, $0.44 OpenClaw (roughly 2×); median time per trial 40.1s (Claude Code and QM) to 99.4s (OpenClaw); GPT-6.1 Sol $0.17 to $0.22 (descriptive, no cost test) | 3 | ✅ |
| Dev results at pinned versions, not held-out; Claude Code and Codex never compared; two OpenClaw cells incomplete; QM on a different Docker network; Tan discloses he runs the eval, QM is a YC project, YC invests in Hermes | how-to-read | ✅ |
| Separate cost run: Claude Code $0.165 less per trial than OpenClaw on Opus 5.5 at the same 80% pass rate; about 81% of the gap was cache writes | 6 | ✅ |
| On harder v0.4 tasks, cutting Claude Code memory-and-skills text and tool-description advice together dropped pass rate from 60.4% to 0.0%; layers cut together so the loss cannot be pinned on one; full prompt wrote auto-memory files in 37 of 48 trials and every one of 29 passes had them; cut arms wrote none in 96 trials | 5 | ✅ (draft said “harder tasks”; clarified to “harder v0.4 tasks”) |
| Must-follow rule seen every turn followed in 30 of 30 member turns on Codex, Hermes Agent and OpenClaw running GPT-6.1 Sol; a rule given once: 2 of 10 later turns on Hermes, 4 of 10 on OpenClaw; dev results, 10 public tasks, one repetition | 12 | ✅ |
| Agents tend to praise work they just produced even when it is mediocre; Anthropic split planner, generator and standalone evaluator | 10 | ✅ |
| Agents marked features complete after unit tests or `curl` without end-to-end confirmation | 9 | ✅ |
| Opus 4.5 comparison: solo run 20 minutes and $9, play mode did not respond to input; full harness 6 hours and $200, playable game with rough physics | 10 | ✅ |
| Each new session starts with no memory of what came before; initializer sets up `init.sh`, `claude-progress.txt`, a failing feature list and an initial git commit; later agents do one feature at a time and leave a commit plus a progress update; compaction alone was not enough — Opus 4.5 on the Claude Agent SDK fell short of a production-quality web app from a high-level prompt | 9 | ✅ |
| Useful harness space moves rather than shrinks: context resets dropped after Opus 4.5 removed most “context anxiety” that Sonnet 4.5 had; sprint decomposition removed once Opus 4.6 could run coherently for more than two hours without it | 11 | ✅ |
| Unmentioned skill: 0 opens in 30 turns on Claude Code and Hermes; naming it in the prompt got Claude Code to 30 of 30 | 12 | ✅ clarified that the 30 of 30 is following the rule, not 30 skill opens (source: Claude Code checked gbrain in 30 of 30 turns after the prompt named the skill) |
| Browser tools plus instructions to test as a user would improved bug-finding | 9 | ✅ Anthropic: browser automation helped the agent identify and fix bugs that were not obvious from the code alone |
| Three corrections tasks never passed in any cell, on Opus 5.5 or on GPT-6.1 Sol | 4 | ✅ |
| Terminal-Bench 2.0: 89 container tasks, scored as agent-model pairs; GPT-5.3-Codex 73.3% with Codex CLI vs 64.7% with Terminus 2 (8.6-point gap); Claude Opus 4.6 58.0% with Claude Code vs 62.9% with Terminus 2 | 7 | ✅ tbench.ai |
| Terminal-Bench 2.1 fixed issues in 28 of 89 tasks; Claude Code + Opus 4.6 58.0% → 70.1% (+12.1, largest gain reported); Terminus 2 + Opus 4.6 62.9% → 63.8% (+0.9); lead flipped without changing the model | 8 | ✅ |
| Meta-Harness 76.4% and Terminus-KIRA 74.7% | — | ✅ absent (left out as unverifiable, per research/writer note) |
| Jon’s surname or address | — | ✅ absent |

No invented sources, numbers, or results. Every figure in the draft traces to the brief and was checked against the original linked source.

## Scores
| Principle | Score | Note |
|---|---|---|
| Useful | 5 | Four-part audit the reader can run in about an hour, plus a cheap first measurement on ten of their own tickets |
| Clear | 4 | One idea per section; harness defined up front. Added a short gloss on context rot; a few eval terms (member turns, cache writes) remain |
| Credible | 4 | Every figure traces to the brief and the original source; all four brief counterpoints are on the page (ceiling, no pass-rate jump, benchmark artifacts, cost). Numbered refs, not inline links |
| Concise | 4 | Evidence is dense because the claims are numbered; cut one repeated closer. The Terminal-Bench recap is long but it is the outlined warning against treating leaderboard gaps as a clean harness win |
| Iterative | 5 | W45 lesson (use each brief counterpoint) is visible: all four appear. This week’s research caution — frame the harness win around cost and speed, not pass rate, and leave unverifiable figures out — was followed |
| **Average** | **4.4** | |

## Send-backs
0 of 1 used. Angle is sound: harness first, with the model still setting the ceiling, and cost/speed rather than pass rate as what moved. Minor cuts and clarifications only; see `04-final.md`.

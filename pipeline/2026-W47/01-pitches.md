# Pitches — week 2026-W47

## 1. Don't wait for the company rollout: a capped, four-week opt-in for Grok team bots
- **Reader:** open question for Jon. Two fits: an engineering manager who wants to try Grok team bots, or a non-technical exec who would have to approve the spend. Recommendation: write it so the manager can hand the piece to the exec. The objections that matter (cost, control, "we'll do a company-wide rollout later") are the leader's, but the person who needs a document this week is usually the one making the case.
- **Why now:** Grok Bot 1.0 shipped on Nov 11, and the headline is shared Team Bots that work alongside a whole team in Slack and Microsoft Teams ([official launch](https://x.com/bot/status/2120582957782200586)). The launch post itself names no prices and no plan gates. Reports this week, including a [Grok reply](https://x.com/grok/status/2120602842192867694), say Team Bots need a Team or Enterprise plan, and meeting support needs Team, Enterprise, or Ultra; Rhett should confirm that against official docs, and should not treat unofficial dollar figures as sourced. A live audience question this week is how much independence to give an agent before human approval is mandatory ([example, Nov 16](https://x.com/harikesh_devops/status/2122246292629778915)). That is the opening for a position paper: early adopters are already trying shared bots, while leadership that prefers a slow, mass-adoption rollout still has no small, bounded way to say yes.
- **Promise:** a position paper someone can take to a hesitant leader this week, with three named points: (1) meet the "not worth the cost" objection with confirmed pilot cost against hours saved, a capped spend, and a clear stop rule after about four weeks, citing only real figures (Rhett verifies every number; invent nothing, including any hours or spend from the lstack loop); (2) early-adopter employees are scattered across companies, so anyone should be able to raise a hand with a stated rationale and join a bounded opt-in pilot, instead of waiting for an org-wide rollout; (3) proof from how the lstack loop actually runs (human approval before anything goes out, files as handoffs, OKRs per bot), with no invented numbers.
- **Rank reason:** this is Jon's own idea, and the clearest piece he can speak to as himself this week, because 1.0 just made team bots a product question for small teams. It has a natural analogy (opt-in pilot vs company rollout) and a named counterpoint: some work should stay off a bot, and a cap and a stop rule have to be real or the cost case falls apart. The open reader question should be settled at the pick, not in the draft. Scores: useful 5, clear 4, credible 4 (only if every figure is confirmed), concise 4, iterative 4.

## 2. Put the boring checks in before you scale agent volume
- **Reader:** engineering managers and tech leads whose teams are speeding up with coding agents and are tempted to take the volume as proof the process is fine
- **Why now:** Lauren Tan's AI Engineer CODE talk landed over the weekend. In her own post she framed it as how the Grok Bot team ships quickly without giving up quality ([Nov 14](https://x.com/poteto/status/2121673563489140863)), and the official conference clip led with "11,000 pull requests in one month. A revert rate around 0.5%." ([AI Engineer, Nov 15](https://x.com/aiDotEngineer/status/2121981562824564960)). Those figures, plus any contributor or personal-PR counts repeated around the talk, need Rhett to confirm against the talk or transcript; they are team-reported, not an audit. A useful counterpoint already in circulation: a low revert rate does not prove the code is good, only that it was not rolled back ([example](https://x.com/SahilExec/status/2122293348983542189)).
- **Promise:** a numbered list of the boring, deterministic checks (architecture, lint, tests, verification) you apply equally to human and agent work, plus a plain test for whether those checks are in place before you let volume rise
- **Rank reason:** timely, tool-agnostic, and it follows last week's lesson that numbered checks help read-through. It is a different question from the shelved W46 harness pitch (quality gates before you scale volume, not "fix the wrapper before you swap models"). It ranks below #1 because the hook leans on one team's reported numbers, and the counterpoint has to stay in or the piece overclaims. Scores: useful 5, clear 4, credible 3, concise 4, iterative 4.

## 3. Teach the agent when to stay quiet
- **Reader:** operators and team leads whose bots now sit in Slack, Teams, or email and are starting to act without being asked
- **Why now:** on Nov 13, Deepnote released the Agent Initiative Benchmark, which drops proactive agents into a simulated company Slack and scores whether they know when to step in, what to say, and when to stay quiet ([Jakub Jurovych](https://x.com/jakubjurovych/status/2121256499552915586)). The official write-up's sharpest finding is not a model ranking: most models try to help even when they are not needed, and in those cases the unnecessary work takes about 80% more time and money than staying quiet would have. Model scores and per-task costs in that post need Rhett to confirm against the original benchmark write-up.
- **Promise:** a short, numbered test you can run on your own bots this week for when a proactive agent should act, and when it should stay silent
- **Rank reason:** a clear action from a fresh, named source, and it is a different question from W46's "oversee, don't block" (this is the agent's decision to act, not the human's decision to leave the loop). The draft has to keep that line or the two pieces will blur. It ranks third because the evidence is one synthetic benchmark, and a model-bake-off draft would miss the point. Scores: useful 4, clear 5, credible 4, concise 4, iterative 3.

## Clip candidates (3)
Real videos already on X. Each post was looked up through X tools, and each has an attached video (`type=video`). I have not independently timed clock marks against the playback, so moments are described without a verified timestamp. Matt Palmer lists chapter markers in his post; those are the author's labels, not times I checked.

### 1.
- **Post URL:** https://x.com/bot/status/2120582957782200586
- **Moment / timestamp:** the official Grok Bot 1.0 trailer (about 79 seconds), when it presents bots as teammates you can share and invite to meetings
- **Why it's useful:** this is the official 1.0 announcement, posted Nov 11. It is the cleanest clip for pitch 1, and it does not depend on unofficial recuts.

### 2.
- **Post URL:** https://x.com/mattyp/status/2122343944889483583
- **Moment / timestamp:** the Team Bot improvements chapter (the author lists chapter markers in the post, starting with Team Bot improvements, then meetings, initiative, learning, and speed)
- **Why it's useful:** a practical walkthrough of what 1.0 actually changed, posted this morning (Nov 16). Better than the trailer alone if the pick is the opt-in pilot, because it shows the shared-team behavior a leader would be asked to try.

### 3.
- **Post URL:** https://x.com/aiDotEngineer/status/2121981562824564960
- **Moment / timestamp:** the official CODE summit clip (about 91 seconds) on the Grok Bot team's shipping pace and quality
- **Why it's useful:** a first-party conference clip of the talk behind pitch 2, posted by AI Engineer on Nov 15. Prefer this over unofficial recuts of the same talk.

---
_Inputs: public X news and audience-question searches for Nov 10 to 16, 2026; [lookbacks/2026-W45.md](../../lookbacks/2026-W45.md); W46 pick and unused pitches in [pipeline/2026-W46/](../2026-W46/). Pitch 1 is Jon's team-bots position paper. The closed-loop idea was the W46 pick, so it is not repeated. Intake picks nothing; Chet picks the topic._

# Pitches — week 2026-W46

## 1. Fix the harness before you switch models
- **Reader:** engineers and tech leads running AI coding agents who are tempted to swap models when results disappoint
- **Why now:** this past week X's top agent stories were about the harness (the context, tools, checks and saved state wrapped around the model), not the model. Garry Tan's run of seven harnesses on the same 20 tasks and a Terminal-Bench 2.0 comparison both reported wide gaps with the same model ([X story, Nov 8](https://x.com/i/trending/2119521473903862094)), and Addy Osmani's harness write-up was trending too ([X story, Nov 8](https://x.com/i/trending/2118767668119691265)). Every figure needs Rhett to confirm it against the original source.
- **Promise:** a numbered harness audit (context, verification, state and progress files, tools) you can run on your own agent setup in an hour, so you know whether to change the harness or the model
- **Rank reason:** strongest trend this week, a clear action for the reader today, and the claims come from named public evals Rhett can trace. It follows last week's lesson that numbered checks drive read-through. The counterpoint is easy to name: on hard tasks the model still sets the ceiling, and several tasks in those evals tied. Scores: useful 5, clear 4, credible 4, concise 4, iterative 4.

## 2. "Done." How do you know your agent actually did it?
- **Reader:** analysts and architects who let agents take real actions (orders, posts, tickets, merges) and have to answer for the results
- **Why now:** "how do you know it actually happened?" was one of the most repeated audience questions on X this week, from agents claiming a purchase is done ([example](https://x.com/damonemcrp/status/2119113773327802592)) to retailers asking whether a real, authorized shopper is behind an agent checkout ([Okta](https://x.com/okta/status/2118377857470619689)). Most of the answers on offer are crypto product pitches, so a plain, vendor-neutral answer is missing.
- **Promise:** a short receipt pattern for agent actions (what to log, what to check against the system of record, when to require a human) that you can add to any agent this week
- **Rank reason:** demand is real and it builds directly on W45's "evaluate an agent before you trust it" piece, so the series has a clear next step. It ranks below #1 because the conversation is noisy and dominated by crypto, which makes sourcing harder for Rhett. Scores: useful 5, clear 4, credible 3, concise 4, iterative 5.

## 3. One queue for many agents: the chief-of-staff setup
- **Reader:** engineers and team leads juggling several agents across separate chats and losing track of what needs their review
- **Why now:** Brian Armstrong's write-up of lead agents run by a "chief of staff" agent that feeds one prioritized queue for his final say was trending this morning ([X story, Nov 9](https://x.com/i/trending/2119219682615885989)), with others debating whether simpler setups do just as well.
- **Promise:** a simple way to route every agent's output into one review queue, plus a plain test for when that setup is overkill
- **Rank reason:** a timely and relatable hook with a natural analogy (a chief of staff), which matches last week's lesson that analogy hooks win. It ranks third because the story centers on one executive, and the productivity claims around it (3x to 100x) are anecdotal and hard to source. Scores: useful 4, clear 4, credible 3, concise 4, iterative 3.

---
_Inputs: public X news and audience-question searches for Nov 2 to 9, 2026; [lookbacks/2026-W45.md](../../lookbacks/2026-W45.md). I found no notes from Jon in the repo this week. Intake picks nothing; Chet picks the topic._

# Package — Oversee, don't block: close the loop on work you can check

## Title options (pick 1)
1. **Oversee, don't block: close the loop on work you can check** ← pick
2. Oversee by the result, not by every click
3. Close the loop on work you can check

## Hooks (3)
1. Watching every click an agent makes is like standing over a colleague's shoulder and initialing every line. That's not oversight. That's still doing the work. *(analogy)*
2. A 7-step pattern you can run this week: write the goal and the check, let the agent iterate until it passes, step in only when the measure says to, and name who owns the misses.
3. Skift and McKinsey found that more than 70% of travelers use AI for research and comparison, but fewer than 16% are comfortable booking through an AI tool. Help me look; don't book for me.

## Format note
This week's X version is one long-form X Article plus a short teaser post, not a thread. The skill template still has a "Thread version" section; this replaces it on purpose. The piece is a seven-step oversight pattern with sourced evidence (Airbnb guest behavior, the Skift/McKinsey research-versus-booking split, a DeepSeek training-run result, Google OKRs and error budgets, NIST, the EU AI Act, and a New York Times report on Crosby). A thread would either drop those sources or run well past a comfortable length. This is also meant to be the first X Article: the earlier W46 harness package was shelved so the first Article would not be about Claude. The aim is that an engineer or tech lead can read one clean piece and leave with a pattern they can run this week. Publish nothing until both approval boxes are checked. Do not create, edit, or delete any X drafts from this file until a human asks. After the Article is live, put its permalink in the teaser where `ARTICLE_URL` appears (X counts that URL as 23 characters). The teaser below is counted with that slot included (247 / 280).

## Article
### Title
Oversee, don't block: close the loop on work you can check

### Body

If you have to approve every step an agent takes, you have not taken yourself out of the work. You have made yourself [the bottleneck](https://x.com/Evoputa/status/2118923396948140506), and the agent saves little time. Careful oversight is not the same as watching every click.

Here is a short test that separates precision work from taste work and high-stakes work, plus a seven-step pattern you can run this week. It puts clear goals and measured results inside the loop, so you know when to step in without approving every step — and so the loop can improve itself over time.

This is not a claim that dropping step-by-step approvals raises a success rate. The evidence says [approvals become the bottleneck](https://x.com/Evoputa/status/2118923396948140506), and that [a reliable check is what lets a loop run and improve](https://arxiv.org/html/2501.12948v2).

## 1. Sort the work
Ask: can I write a check that most people would grade the same way? If yes — a total that matches, a test suite that passes, a form that is complete, a refund under a stated limit — it is precision work. [Jason Wei's verifier's rule](https://www.jasonwei.net/blog/asymmetry-of-verification-and-verifiers-law) is that the ease of training AI to solve a task is proportional to how verifiable the task is. Tasks that work well have an objective standard of good (people agree) and can be checked quickly and at scale, with low noise. You can make more work checkable by writing the check first: an answer key, or test cases for code.

If "good" depends on voice, taste, or a judgment call people would debate, it is taste work. If it goes to a client, moves money, makes a legal commitment, or cannot be undone, treat it as high-stakes even if some part of it is checkable.

Checkable is not the same as "no human needed." Some work runs the other way: [fact-checking a long essay can take longer than writing it](https://www.jasonwei.net/blog/asymmetry-of-verification-and-verifiers-law). Incomplete checks — tests that miss a bug, a key result that does not cover the real objective — leave misses the loop will not catch unless a person owns them.

## 2. Write the goal and the measure before you step back
[Google's public OKR guide](https://rework.withgoogle.com/intl/en/guides/set-goals-with-okrs) quotes Andy Grove's two questions from *High Output Management*: "Where do I want to go?" (the objective) and "How will I pace myself to see if I am getting there?" (the key results). A key result names a measurable outcome and the evidence you will accept — evidence that is available, credible, and easy to find. It is not a list of steps to approve. [OKRs are not a shared to-do list](https://rework.withgoogle.com/intl/en/guides/set-goals-with-okrs).

If you cannot write a key result that people would score the same way, you do not yet have a closed loop. Stay in it.

## 3. Give the agent the check, not a pile of step approvals
For precision work, let the agent iterate until the check passes. Match the oversight to the action: how much damage if it goes wrong, and can you reverse it? [High-volume, reversible work can run, log, and alert, with a person stepping in only when needed](https://x.com/Evoputa/status/2118923396948140506).

When a result can be checked automatically, a loop can improve itself without a person judging every attempt. [DeepSeek-R1-Zero](https://arxiv.org/html/2501.12948v2) trained with rule-based rewards: math answers checked against ground truth, code checked by a compiler against test cases. In that training run, AIME 2024 pass@1 — first-try success on contest math problems — moved from 15.6% to 77.9%. The paper's conclusion is that the key is hard questions plus a reliable verifier, not a person scoring every step. That movement is a training-run result on verifiable contest problems, not a workplace productivity number, and it is not evidence that removing your step approvals will raise a success rate. It is evidence that a reliable check is what lets a loop improve.

## 4. Oversee by exception, using the measure
Set the threshold for when a person steps in. [Google's published error-budget policy](https://sre.google/workbook/error-budget-policy/) is a concrete pattern: if a service is at or above its SLO (its reliability target), releases proceed; if it has exceeded its error budget for the preceding four-week window, the team halts changes other than P0 (highest-priority) issues or security fixes until the service is back within its SLO. The workbook calls the error budget "a control mechanism for diverting attention to stability as needed."

[NIST's AI Risk Management Framework](https://nvlpubs.nist.gov/nistpubs/ai/NIST.AI.100-1.pdf) organizes the work as Govern, Map, Measure and Manage. Measure means testing before deployment and regularly while the system is running. Manage then allocates a response: among other things, "mechanisms are in place and applied, and responsibilities are assigned and understood, to supersede, disengage, or deactivate AI systems that demonstrate performance or outcomes inconsistent with intended use." Measurement is what tells an overseer when to take that step.

Oversight is not one setting. The [EU High-Level Expert Group on AI](https://digital-strategy.ec.europa.eu/en/library/ethics-guidelines-trustworthy-ai) lists three approaches: human-in-the-loop, human-on-the-loop, and human-in-command. For high-risk AI, the [EU AI Act's Article 14](https://ai-act-service-desk.ec.europa.eu/en/ai-act/article-14) requires that systems be designed so people can effectively oversee them while they are in use, in a way commensurate with the system's risks, autonomy and context. The people assigned to oversee it must be able to monitor for anomalies, interpret outputs, decide not to use the system or to disregard, override or reverse its output, and interrupt it with a stop that leaves it in a safe state.

## 5. Keep taste and high-stakes work in the loop
Review that work before it goes out. Help with research or a first draft is not the same as letting the agent make the choice.

[Airbnb's Q3 2026 results letter](https://news.airbnb.com/airbnb-q3-2026-financial-results) (Nov 5, 2026) argues that today's agents are good at simple, routine tasks such as making a restaurant reservation or scheduling an appointment, but that planning a trip is different: "People don't want to delegate the choice of where to stay. They want to browse unique homes, compare options and decide for themselves, often with the people they're traveling with." On Airbnb's own platform, more than 75% of guests use maps when deciding where to stay, over 90% browse multiple listing photos, 70% read reviews before booking, bookings average 3 guests, and more than 90% of stays involve direct communication between guests and hosts.

These next figures are not from Airbnb. [Skift and McKinsey's seventh annual research collaboration](https://skift.com/2026/09/25/how-travel-search-discovery-and-booking-are-being-rewritten/) — a study of 1,000 consumers and traveler diaries, as written up by Skift — reported that Margaux Constantin of McKinsey said 80% of travelers enjoy spending time researching. The same write-up reports that more than 70% of travelers use AI for research and comparison, but fewer than 16% are comfortable actually booking through an AI tool. Help me look; don't book for me.

Keep a person in the loop for work that [goes to clients, moves money, makes a legal commitment, or cannot be undone](https://x.com/Evoputa/status/2118923396948140506).

## 6. Name who owns the misses
Before you remove a person from a class of actions, write down who is accountable and who pays if the agent is wrong. The [EU guidelines](https://digital-strategy.ec.europa.eu/en/library/ethics-guidelines-trustworthy-ai) require accountability for AI systems and their outcomes, including auditability and accessible redress. If no one owns the misses, you have not closed the loop — you have only moved the risk.

Sarah Kessler, reporting for *The New York Times* (Nov 7, 2026, [full-text reprint](https://www.dailygazette.com/nyt-feed/law-firms-have-malpractice-insurance-should-their-ai-agents/article_65e53fb5-528d-58ed-abde-6e248abd16ea.html)), wrote that Crosby, an AI law firm, secured $5 million of AI-agent liability insurance from Testudo. After the policy took effect, Crosby removed lawyer supervision from gray-area, paralegal-style tasks, which the firm says account for about 20% of its work. It still has lawyers supervising tasks that are clearly legal work. The Times notes that taking lawyers completely out of the loop would run into current rules on unlicensed practice and on lawyers supervising nonlawyers. The insurance answers who pays when a gray-area task goes wrong, not whether high-stakes legal work can run unsupervised.

Ownership is a person or a policy that pays — not "the agent."

## 7. Use the scores to improve the next cycle
Treat a miss as data: refine the goal, the check, or the threshold. Google treats low OKR grades as data to refine the next OKRs, and recommends a [mid-cycle check-in](https://www.whatmatters.com/faqs/weekly-okr-grading-check-in) before final grading. Checking in asks whether you are on track and what would get you back on track; grading asks whether the goal was met. John Doerr, as quoted on [What Matters](https://www.whatmatters.com/faqs/weekly-okr-grading-check-in): "OKRs are driven by data. They are animated by periodic check-ins, objective grading, and continuous reassessment — all in a spirit of no-judgment accountability." A loop with no measured result cannot improve itself.

A loop that only chases a thin metric can improve the wrong thing. Marilyn Strathern, restating Goodhart, wrote: ["When a measure becomes a target, it ceases to be a good measure."](https://gwern.net/doc/statistics/decision/1997-strathern.pdf) [DeepSeek](https://arxiv.org/html/2501.12948v2) reports reward hacking when a learned preference model, rather than a hard verifier, is the score — the system can chase the score without matching the real goal. If the only check is "did the metric move," an agent can hit the number and miss the point.

## Takeaway
Start this week with one checkable workflow: a written goal, a pass/fail check, a threshold for stepping in, and a named owner.

Stay in the loop for taste and for anything you cannot undo. [Article 14](https://ai-act-service-desk.ec.europa.eu/en/ai-act/article-14) also warns overseers to stay aware of automation bias — the tendency to over-rely on what the system produces. Lisanne Bainbridge's ["Ironies of automation"](https://ckrybus.com/static/papers/Bainbridge_1983_Automatica.pdf) made the same point in 1983: after automation, the person is left to monitor the system and to take over if it fails; unused control skills deteriorate, and takeover usually happens when something is already wrong, so more skill is needed, not less. An overseer who only watches a dashboard still needs enough practice to intervene well.

Do not take yourself out of work you cannot check. Close the loop on work you can.

## Teaser post
Each URL counts as 23 characters. Replace `ARTICLE_URL` with the Article permalink after publish. Counted length: 247 / 280.

```
If you have to approve every step an agent takes, you have not taken yourself out of the work. You have made yourself the bottleneck.

I wrote up a 7-step pattern you can run this week: close the loop on work you can check.
ARTICLE_URL
```

## Images
| File | Alt text |
|---|---|
| assets/lotti-pose-thinking.jpg | Lotti, a man with curly dark hair and a mustache, wearing an orange hoodie, chin in hand, looking up at a glowing lightbulb against an orange circle. |
| assets/lotti-pose-laptop.jpg | Lotti in an orange hoodie typing on a laptop at a wooden desk, a steaming white coffee mug beside him, against an orange circle. |
| assets/lotti-pose-thumbsup.jpg | Lotti in an orange hoodie giving a thumbs-up and a slight smile, against an orange circle. |

Suggested pairing: thinking pose at the top of the Article, laptop pose near the seven steps, thumbs-up near the takeaway.

## Channel versions
### X (launch channel)
Publish the Article first, then the teaser with the Article permalink. X is the only launch channel this week. Do not publish until both approval boxes below are checked. Do not create an X draft from this file until a human asks.

### Later (not yet active): TikTok, LinkedIn, YouTube Shorts
Not active yet.

## Approval
- [ ] Lead approved
- [ ] Human approved publish

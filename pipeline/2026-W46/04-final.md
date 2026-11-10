# Oversee, don't block: close the loop on work you can check

If you have to approve every step an agent takes, you have not taken yourself out of the work. You have made yourself the bottleneck, and the agent saves little time [1]. Careful oversight is not the same as watching every click.

Here is a short test that separates precision work from taste work and high-stakes work, plus a seven-step pattern you can run this week. It puts clear goals and measured results inside the loop, so you know when to step in without approving every step — and so the loop can improve itself over time.

This is not a claim that dropping step-by-step approvals raises a success rate. The evidence says approvals become the bottleneck, and that a reliable check is what lets a loop run and improve [1][3].

## 1. Sort the work
Ask: can I write a check that most people would grade the same way? If yes — a total that matches, a test suite that passes, a form that is complete, a refund under a stated limit — it is precision work [2][3]. Jason Wei’s verifier’s rule is that the ease of training AI to solve a task is proportional to how verifiable the task is. Tasks that work well have an objective standard of good (people agree) and can be checked quickly and at scale, with low noise. You can make more work checkable by writing the check first: an answer key, or test cases for code [2].

If “good” depends on voice, taste, or a judgment call people would debate, it is taste work [2][10][11]. If it goes to a client, moves money, makes a legal commitment, or cannot be undone, treat it as high-stakes even if some part of it is checkable [1][9][12].

Checkable is not the same as “no human needed.” Some work runs the other way: fact-checking a long essay can take longer than writing it [2]. Incomplete checks — tests that miss a bug, a key result that does not cover the real objective — leave misses the loop will not catch unless a person owns them.

## 2. Write the goal and the measure before you step back
Google’s public OKR guide quotes Andy Grove’s two questions from *High Output Management*: “Where do I want to go?” (the objective) and “How will I pace myself to see if I am getting there?” (the key results) [4]. A key result names a measurable outcome and the evidence you will accept — evidence that is available, credible, and easy to find. It is not a list of steps to approve. OKRs are not a shared to-do list [4].

If you cannot write a key result that people would score the same way, you do not yet have a closed loop. Stay in it.

## 3. Give the agent the check, not a pile of step approvals
For precision work, let the agent iterate until the check passes [2][3]. Match the oversight to the action: how much damage if it goes wrong, and can you reverse it? High-volume, reversible work can run, log, and alert, with a person stepping in only when needed [1].

When a result can be checked automatically, a loop can improve itself without a person judging every attempt. DeepSeek-R1-Zero trained with rule-based rewards: math answers checked against ground truth, code checked by a compiler against test cases. In that training run, AIME 2024 pass@1 — first-try success on contest math problems — moved from 15.6% to 77.9%. The paper’s conclusion is that the key is hard questions plus a reliable verifier, not a person scoring every step [3]. That movement is a training-run result on verifiable contest problems, not a workplace productivity number, and it is not evidence that removing your step approvals will raise a success rate. It is evidence that a reliable check is what lets a loop improve.

## 4. Oversee by exception, using the measure
Set the threshold for when a person steps in. Google’s published error-budget policy is a concrete pattern: if a service is at or above its SLO (its reliability target), releases proceed; if it has exceeded its error budget for the preceding four-week window, the team halts changes other than P0 (highest-priority) issues or security fixes until the service is back within its SLO. The workbook calls the error budget “a control mechanism for diverting attention to stability as needed” [6].

NIST’s AI Risk Management Framework organizes the work as Govern, Map, Measure and Manage. Measure means testing before deployment and regularly while the system is running. Manage then allocates a response: among other things, “mechanisms are in place and applied, and responsibilities are assigned and understood, to supersede, disengage, or deactivate AI systems that demonstrate performance or outcomes inconsistent with intended use.” Measurement is what tells an overseer when to take that step [7].

Oversight is not one setting. The EU High-Level Expert Group on AI lists three approaches: human-in-the-loop, human-on-the-loop, and human-in-command [8]. For high-risk AI, the EU AI Act’s Article 14 requires that systems be designed so people can effectively oversee them while they are in use, in a way commensurate with the system’s risks, autonomy and context. The people assigned to oversee it must be able to monitor for anomalies, interpret outputs, decide not to use the system or to disregard, override or reverse its output, and interrupt it with a stop that leaves it in a safe state [9].

## 5. Keep taste and high-stakes work in the loop
Review that work before it goes out [1][10][11][12]. Help with research or a first draft is not the same as letting the agent make the choice.

Airbnb’s Q3 2026 results letter (Nov 5, 2026) argues that today’s agents are good at simple, routine tasks such as making a restaurant reservation or scheduling an appointment, but that planning a trip is different: “People don’t want to delegate the choice of where to stay. They want to browse unique homes, compare options and decide for themselves, often with the people they’re traveling with.” On Airbnb’s own platform, more than 75% of guests use maps when deciding where to stay, over 90% browse multiple listing photos, 70% read reviews before booking, bookings average 3 guests, and more than 90% of stays involve direct communication between guests and hosts [10].

These next figures are not from Airbnb. Skift and McKinsey’s seventh annual research collaboration — a study of 1,000 consumers and traveler diaries, as written up by Skift — reported that Margaux Constantin of McKinsey said 80% of travelers enjoy spending time researching. The same write-up reports that more than 70% of travelers use AI for research and comparison, but fewer than 16% are comfortable actually booking through an AI tool [11]. Help me look; don’t book for me.

Keep a person in the loop for work that goes to clients, moves money, makes a legal commitment, or cannot be undone [1].

## 6. Name who owns the misses
Before you remove a person from a class of actions, write down who is accountable and who pays if the agent is wrong [8][9][12]. The EU guidelines require accountability for AI systems and their outcomes, including auditability and accessible redress [8]. If no one owns the misses, you have not closed the loop — you have only moved the risk.

Sarah Kessler, reporting for *The New York Times* (Nov 7, 2026), wrote that Crosby, an AI law firm, secured $5 million of AI-agent liability insurance from Testudo. After the policy took effect, Crosby removed lawyer supervision from gray-area, paralegal-style tasks, which the firm says account for about 20% of its work. It still has lawyers supervising tasks that are clearly legal work. The Times notes that taking lawyers completely out of the loop would run into current rules on unlicensed practice and on lawyers supervising nonlawyers [12]. The insurance answers who pays when a gray-area task goes wrong, not whether high-stakes legal work can run unsupervised.

Ownership is a person or a policy that pays — not “the agent.”

## 7. Use the scores to improve the next cycle
Treat a miss as data: refine the goal, the check, or the threshold [3][5][7]. Google treats low OKR grades as data to refine the next OKRs, and recommends a mid-cycle check-in before final grading. Checking in asks whether you are on track and what would get you back on track; grading asks whether the goal was met [5]. John Doerr, as quoted on What Matters: “OKRs are driven by data. They are animated by periodic check-ins, objective grading, and continuous reassessment — all in a spirit of no-judgment accountability” [5]. A loop with no measured result cannot improve itself.

A loop that only chases a thin metric can improve the wrong thing. Marilyn Strathern, restating Goodhart, wrote: “When a measure becomes a target, it ceases to be a good measure.” DeepSeek reports reward hacking when a learned preference model, rather than a hard verifier, is the score — the system can chase the score without matching the real goal [3]. If the only check is “did the metric move,” an agent can hit the number and miss the point.

## Takeaway
Start this week with one checkable workflow: a written goal, a pass/fail check, a threshold for stepping in, and a named owner.

Stay in the loop for taste and for anything you cannot undo. Article 14 also warns overseers to stay aware of automation bias — the tendency to over-rely on what the system produces [9]. Lisanne Bainbridge’s “Ironies of automation” made the same point in 1983: after automation, the person is left to monitor the system and to take over if it fails; unused control skills deteriorate, and takeover usually happens when something is already wrong, so more skill is needed, not less. An overseer who only watches a dashboard still needs enough practice to intervene well.

Do not take yourself out of work you cannot check. Close the loop on work you can.

# Topic pick: 2026-W47 (replacement)

**Picked:** Pitch 1 in 01-pitches.md: "Don't wait for the company rollout: a capped, four-week opt-in for Grok team bots."

**Why:** This is Jon's own position paper for small teams that want to try Grok team bots while leadership hesitates and prefers a slow, mass-adoption rollout. The reader is an engineering manager who will hand the piece to a non-technical exec. Meet the "not worth the cost" objection head on with a capped spend, a stop rule, and pilot cost weighed against hours saved. Use only figures Rhett can source. The official 1.0 post lists no prices, so leave a figure out rather than estimate it. Reports that Team Bots need a Team or Enterprise plan, and that meeting support needs Team, Enterprise, or Ultra, must be confirmed against official docs; do not treat unofficial dollar figures as sourced. Early adopters are scattered across companies, so everyone should get the chance to raise a hand and try something, with a rationale for why a bounded opt-in beats a mandate. The lstack loop can serve as a real example (human approval before anything goes out, files as handoffs, OKRs per bot), but do not invent results or numbers, including any hours or spend from the loop. The counterpoint must stay in: some work should stay off a bot, and a cap and a stop rule have to be real or the cost case falls apart.

**Format:** a single X Article on @JonLotti, saved as a draft only, plus a short teaser post. No thread. Don't imply Jon uses tools he doesn't, including Claude, Hermes, and OpenClaw.

**Clips going forward:**

1. Keep https://x.com/bot/status/2120582957782200586, the official Grok Bot 1.0 trailer (about 79 seconds), when it presents bots as teammates you can share and invite to meetings. This fits the topic directly. Timestamps are not verified, so describe the moment rather than citing a clock mark.
2. Also keep https://x.com/mattyp/status/2122343944889483583, Matt Palmer's 1.0 walkthrough, for the Team Bot improvements chapter (the author lists chapter markers in the post, starting with Team Bot improvements, then meetings, initiative, learning, and speed). Those chapter markers are his own and have not been timed independently. Timestamps are not verified, so describe the moment rather than citing a clock mark.

The official CODE summit clip (https://x.com/aiDotEngineer/status/2121981562824564960) is not kept this week. It was a better fit for the boring checks piece.

**Approved by:** Jon (Mon Nov 16, 2026).

**Backlog:** The finished earlier W47 pick, "Put the boring checks in before you scale agent volume," is parked in shelved/2026-W47-boring-checks/. It can run in a later week with only a light refresh. Pitch 3, "Teach the agent when to stay quiet," is held for a later week.

**History:** On Mon Nov 16, 2026, Jon first picked and later approved the boring checks piece for Friday publish, then the same day swapped W47 to this opt-in pilot paper. The parked pipeline and its unpublished X Article drafts are in shelved/2026-W47-boring-checks/.

## Direction update 5 (Fri Nov 20, 2026, from Jon): split into two articles

Jon said the current final limits what the tools can do. The fit section and its four-row table (shared agents, scheduled work, joins meetings, admin and data controls) read as too general. He also said the line "if the pilot does not help, stopping is the result" doesn't make sense, so cut it. Jon chose to split the work into two articles.

**W47, publish first: the exec opt-in case.** Keep it tool-agnostic. It should explain why an executive should sanction a capped, opt-in pilot of AI agents across use cases, not only Grok Bot. Grok Bot can be one example among others, but the article should not be a Grok Bot pitch. Keep the sourced productivity evidence, the definitions, the limits of the evidence, and the risk line about agents that act on their own. Drop the generic Grok Bot fit table. Write any stop rule in plain, concrete words: what gets measured, by when, and what happens if the bar isn't met.

**W48, next week: the Grok Bot team article.** The differentiator is a team of Grok Bots in roles, such as an analyst, an architect, or a scrum master, doing real work together. It should not be a list of features. Concrete role use cases only, with nothing invented. Any capability claim must be sourced to official docs. The lstack loop can serve as a real example, but don't add invented numbers.

All of Jon's writing rules still apply. Avoid jargon, prefer US studies, and define academic terms with an APA citation. Name sources in full at first mention. Write "article," not "piece." State the purpose plainly. Use no em dashes. Never use Jon's surname.

**Approved by:** Jon (Fri Nov 20, 2026, 5:32 PM ET).

## Direction update 6 (Sat Nov 21, 2026, from Jon): AI-source recency

**Rule.** Every AI-specific claim must cite a source whose data is from the last six months. For W47 the cutoff is May 20, 2026. Where a source was published inside the window but some of its data is older, say which years the data covers. Non-AI points and definitions are exempt, so the definitions from Puthal et al. (2025), the Center for AI Standards and Innovation (CAISI, 2026) and the U.S. Government Accountability Office (GAO, 2025) stay. The GOV.UK discovery-phase guide (GDS, 2021) stays too, because it is not about AI.

**Swaps.** Each quote below was checked live at its URL on Nov 20, 2026.
- Employer encouragement (opening and "Encouragement goes with use"): replace Bick et al. (86% vs 13%, and 65 points) and Lin and Parker of the Pew Research Center (half say neither) with the Gallup AI indicator, https://www.gallup.com/699797/indicator-artificial-intelligence.aspx. Section "Do Managers Support Employee Use of AI?" (data as of May 2026): employees in AI-adopting organizations who strongly agree that their manager actively supports their team's use of AI are "1.7x as likely to use AI a few times a week or more." Section "Do Most Companies Have a Clear AI Strategy?": "As of August 2026, 26% of U.S. employees say their organization has communicated a clear plan for integrating AI into current practices." The 26% measures a clear plan, not encouragement, so reword the sentence to match. The "not necessarily causal" caveat becomes our own words, because Gallup is also a survey.
- Task mix ("Real pilots already cover several uses"): Gallup, "Organizational AI Adoption Jumps Six Points" (July 20, 2026; survey May 6 to 20, 2026), https://www.gallup.com/workplace/712736/organizational-adoption-jumps-six-points.aspx: "the most common uses of AI are writing and editing (51%), search or research (49%), and general assistance or problem-solving (39%)."
- Average time saved ("Results differ by use"): replace Bick et al.'s 1.4% with the FRED Blog of the Federal Reserve Bank of St. Louis, "Does generative AI save time at work?" (August 27, 2026), https://fred.stlouisfed.org/blog/2026/08/does-generative-ai-save-time-at-work/: "the share of work hours saved thanks to AI assistance grew from 1.6% to 2.2%" (through Q2 2026). Label it self-reported. The post says "The information is based on how respondents self-report their 'time saved,' so the measurements are inherently approximate."
- Drafting, and uneven gains: replace Noy and Zhang (2023) and the Brynjolfsson et al. experience finding with Autor et al., "Does AI Assistance Enhance or Erode Expertise? Evidence from a Three-Month Field Experiment in Patent Drafting," NBER Working Paper 35720 (September 2026), https://www.nber.org/papers/w35720. This is a US randomized trial with 133 patent lawyers at eleven US firms, with data from May 2025 to February 2026. PDF p. 4: "Treated lawyers spent about 10 fewer minutes on the 10-day drafting task than controls (p = 0.05), whose mean was 110 minutes." Abstract: "this advantage was concentrated entirely among senior lawyers" and "Junior lawyers showed no average gain." The second quote is about judgment on a later task done without AI, and its direction differs from Brynjolfsson, so rewrite the bullet rather than swapping one number. Label: funded by Google, with Google staff among the authors.
- Self-reports ("Time the work rather than ask people"): replace METR (Becker et al., data from February to June 2025) with Yu et al., "Cognitive offloading and the speedup illusion in human-AI interaction" (Stanford; arXiv 2605.23177, May 22, 2026), https://arxiv.org/abs/2605.23177. N = 1,237. Abstract: "While actual completion times between independent completion and AI-assisted completion did not differ, participants predicted AI to be significantly faster." Label: preprint; simple lab tasks, not real jobs. This becomes the new teaser hook.
- Trust and checking ("What the evidence does not show"): replace Lee et al. (2025), and the workslop numbers (see below), with Ma et al., "Impact of Expertise and Trust on AI-assisted Work" (Carnegie Mellon University and Microsoft; arXiv 2610.14660, October 10, 2026), https://arxiv.org/abs/2610.14660. Abstract: "participants who delegated more completed more of the task, but were also more likely to produce invalid solutions." Label: preprint; 20 professionals in a think-aloud study; Microsoft authors.
- Agents: Wang et al., "Agentic AI and Human-in-the-Loop Interventions: Field Experimental Evidence from Alibaba's Customer Service Operations" (arXiv 2605.14830; v1 May 14, 2026, revised June 1, 2026), https://arxiv.org/abs/2605.14830. Abstract: "AI deployment reduces average chat duration and has limited effects on retrial rates, but substantially lowers ratings for AI-eligible chats." Label: not US (Taobao, China). Rewrite the "no workplace study of agents that act on their own" gap around it: there is now one randomized field trial, outside the US and in customer service only.

**Cuts.** The UK trial numbers (GDS 2025b, the DBT pilot, the DSIT "26 minutes" release), escalations (Brynjolfsson et al.), the Excel finding (DBT), Humlum and Vestergaard (Denmark), Bick et al.'s 6-point gender gap, and the UK "83%" and "around 80%" adoption line in the stop-rule section. My calls on the three open items:
- Workslop (BetterUp Labs and Stanford Social Media Lab, data from August to September 2025): cut the 40% and 1hr56m figures and the bullet. Ma et al. covers the point, and I found no newer workslop data.
- UK AI Playbook (GDS, 2025a): cut. It is not US and not recent. The advice to start agents read-only, with a named reviewer and an off-limits list, stays as our own judgement.
- Olson et al. (2025, AI note-takers, data from 2024): keep, labeled "data from 2024." Note-taking relief is one of Jon's core examples, and I found no in-window replacement I could verify. If Rhett finds a verifiable source from inside the window, swap it in. Otherwise keep the label.

**Keep, with a "data from" label.** Dillon et al., the 66-firm randomized trial (data from 2023 to 2024; still forthcoming in *American Economic Review: Insights*). The Commonwealth of Pennsylvania pilot (data from 2024 to 2025), which is still the only US opt-in pilot evaluation we have. Its volunteer, self-report and teams quotes stay, with the label.

**Knock-on fixes.**
- Teaser: drop the METR hook and lead with Yu et al. (people predicted AI would be faster when it took no less time). "Time tasks by the clock" still works.
- Takeaway: "none of it from tests of agents acting on their own" is no longer true. Rewrite it to say that one non-US field trial of agents exists, in customer service only.
- Stop-rule Sources line: rewrite it to name only the sources still in the article.
- Last sentence of "Three terms": rewrite it around the Gallup measures (manager support, a clear plan) instead of Bick et al. and Pew.
- References: drop every cut source and add the new ones in APA.

Everything from Direction updates 1 to 5 still stands. Keep the article tool-agnostic, with no Grok Bot. Use no em dashes, name sources in full at first mention, use APA and et al., write "article," not "piece," and keep Jon's academic voice. Never invent sources or numbers. If a figure can't be verified at its URL, cut it rather than guess.

**Approved by:** Jon (Sat Nov 21, 2026, 9:45 AM ET).

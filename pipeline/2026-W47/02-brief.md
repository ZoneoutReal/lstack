# Brief — Don't wait for the company rollout: a capped, four-week opt-in for Grok team bots

## Reader and promise
An engineering manager who will hand this paper to a non-technical exec who prefers a slow, company-wide rollout. Promise: a position paper they can take to that exec this week. It answers the "not worth the cost" objection with official list prices, a hard spend cap the product actually supports, a stop rule written before the pilot starts, and an honest way to weigh pilot cost against time saved. It also makes the case for letting early adopters raise a hand for a bounded, sanctioned opt-in instead of waiting for a mass rollout.

All web sources were accessed Mon Nov 16, 2026. Prices are US list prices as shown that day, excluding tax, and the pricing page says "Prices subject to change." Re-check them before publish.

## Key claims
| # | Claim | Source (link) |
|---|---|---|
| 1 | **Official individual prices** (The X Subscription). Free $0/month; Plus $8/month; Premium $30/month; Super $100/month; Ultra $200/month. Annual options: Plus $80/yr, Premium $300/yr, Super $1000/yr, Ultra $2000/yr. Included usage is shown relative to Plus: Premium "4x," Super "15x," Ultra "50x." "Prices shown do not include applicable taxes or fees," and "Third Party model usage in Cursor is not included in the monthly prices shown and must be purchased separately." | https://x.ai/pricing ; https://docs.x.ai/x-subscription/pricing |
| 2 | **Which plans include Grok Bot.** "Grok Bot is included on Premium, Super, and Ultra. Plus does not include Grok Bot." Bot usage "draws from that seat's shared weekly usage pool, not a separate additive pool." No official page states the pool in hours, tasks or dollars, only as multiples. | https://docs.x.ai/x-subscription/pricing ; https://docs.x.ai/grok-bot/faq ; https://docs.x.ai/x-subscription/usage-limits |
| 3 | **Official team prices.** "Team plans are available on Premium at $30 per seat, Super at $100 per seat, and Ultra at $200 per seat. Each seat includes the same usage as the matching individual tier." Tiers can be mixed, for example "three Premium seats and one Super seat." "Plus isn't available for teams." On self-serve team plans, "each paid seat has its own weekly pool ... Seats do not share weekly pools." Enterprise is sold through sales; the pricing page says organizations that "need invoicing, pooled usage, or advanced security should choose Enterprise." | https://docs.x.ai/x-subscription/pricing ; https://cursor.com/docs/account/teams/pricing ; https://docs.x.ai/x-subscription/usage-limits ; https://x.ai/pricing |
| 4 | **Plan gates, now confirmed officially.** Grok Bot 1.0 post: "Team Bots are available on Team and Enterprise plans. Meetings are available on Team, Enterprise, and Ultra plans. Enterprise admins can turn on Meetings in settings." The admin docs say the same about Meetings. This confirms the unofficial Grok reply quoted in the pitch, so cite these official sources, not the reply. | https://x.ai/news/grok-bot-1-0 ; https://docs.x.ai/grok-bot/teams-and-enterprises ; (pitch's unofficial source: https://x.com/grok/status/2120602842192867694) |
| 5 | **The hard cap exists, but it sits on the account or team, not on Grok Bot.** A "monthly additional usage limit (spending cap) controls how much paid Additional Usage you can use in a calendar month," on individual and self-serve team plans. Additional Usage stops when "the prepaid balance is empty, or the team's monthly extra-usage cap is reached." "Alerts do not stop usage. To put a hard stop on paid Additional Usage, set a monthly additional usage limit." Auto Top-up is "off unless you turn it on." Admins can also set "a default monthly limit per member and per-member overrides." There is no Grok Bot-specific cap: "A separate Grok Bot spend cap is not available today. Account-level on-demand controls apply." | https://docs.x.ai/x-subscription/spending-caps ; https://cursor.com/docs/account/teams/pricing ; https://docs.x.ai/grok-bot/teams-and-enterprises |
| 6 | **The stop mechanics, in the vendor's words.** When someone joins, "a new seat is bought and charged a prorated amount for the rest of the billing period." A removed member "lose[s] access to the team right away," but "Their seat stays on your plan" until an admin selects Reduce seats, and "Removed seats come off at the end of the billing period." "On Team plans, a canceled seat stays active until the end of the billing period." On the pricing page: "Cancel anytime, at least 24 hours prior to renewal to avoid additional charges." | https://docs.x.ai/x-subscription/team-plans ; https://docs.x.ai/x-subscription/cancel ; https://x.ai/pricing |
| 7 | **The boundary of a self-serve pilot is team membership.** "On the Teams plan, Grok Bot is enabled by default, and every member has access without any admin action ... There is no switch to turn it off." On Enterprise, an admin turns it on and can "limit it to specific groups." Several admin controls are "Enterprise only," including Network Controls, Team Secrets, Enforce Auto-review, Auto-review rules and the organization-wide enable switch. "People can belong to more than one workspace," so a pilot can live in its own team workspace. | https://docs.x.ai/grok-bot/teams-and-enterprises ; https://docs.x.ai/x-subscription/team-plans |
| 8 | **Capped, time-boxed pilots are normal practice, even in large organizations.** The UK government ran a cross-government M365 Copilot trial "from 30 September 2024 to 31 December 2024, involving 20,000 government employees," with each organisation committing to at least 1,000 licences. Before that, "previous trials and pilots [were] limited to 300 licences at most." The UK Department for Business and Trade (DBT) had "One thousand licences ... for a 3-month pilot from October to December 2024." | https://www.gov.uk/government/publications/microsoft-365-copilot-experiment-cross-government-findings-report/microsoft-365-copilot-experiment-cross-government-findings-report-html ; https://assets.publishing.service.gov.uk/media/68adbe409e1cebdd2c96a19d/dbt-microsoft-365-copilot-evaluation.pdf |
| 9 | **Stopping is a legitimate result, if you decide the test up front.** The GOV.UK Service Manual says to decide whether it is "cost effective to pursue the problem - this means weighing up how much it'd cost against how much of an improvement you think you could make," and that "It's not a failure to stop at the end of the discovery phase if your research shows that's the best thing to do. In fact, you'll be saving time and money." On timing: "There's no set time period for a discovery, but around 4 to 8 weeks is typical." | https://www.gov.uk/service-manual/agile-delivery/how-the-discovery-phase-works |
| 10 | **Self-reported time savings: what a big pilot found, and the fine print.** Cross-government trial: "Trial participants saved an average of 26 minutes a day," "only 17% not noticing any clear time savings," and "users could save 13 days" a year if replicated. GOV.UK's press release: "Figures are derived from self-reported daily time savings." Adoption reached "83%," then "around 80% was maintained," but Excel and PowerPoint peaked at "23% and 24%." The report also says "resources were required to drive engagement and adoption." | https://www.gov.uk/government/publications/microsoft-365-copilot-experiment-cross-government-findings-report/microsoft-365-copilot-experiment-cross-government-findings-report-html ; https://www.gov.uk/government/news/landmark-government-trial-shows-ai-could-save-civil-servants-nearly-2-weeks-a-year |
| 11 | **A sobering pilot to set against claim 10.** DBT found "Small time savings were observed across most use cases," but "The evaluation did not find evidence that time savings have led to improved productivity." Users "completed Excel data analysis more slowly and to a worse quality and accuracy than non-users." "Further evaluation is needed to assess the value for money." | https://assets.publishing.service.gov.uk/media/68adbe409e1cebdd2c96a19d/dbt-microsoft-365-copilot-evaluation.pdf ; https://www.gov.uk/government/publications/microsoft-365-copilot-pilot-dbt-evaluation-report |
| 12 | **Volunteers aren't a random sample, and a careful pilot plans for that.** DBT let colleagues "volunteer for a licence, until around ~70% of licences had been allocated. The remaining ~30% of licences were assigned to a random sample ... stratified by directorate group and grade to improve representation." | https://assets.publishing.service.gov.uk/media/68adbe409e1cebdd2c96a19d/dbt-microsoft-365-copilot-evaluation.pdf |
| 13 | **People aren't waiting for the rollout.** Denmark (Humlum and Vestergaard, NBER, revised March 2026): "even among workers whose employers neither encourage chatbot use, provide an enterprise chatbot, nor offer training, about 41% have used AI chatbots at work at least once, and 7% use them daily." Microsoft and LinkedIn (2024; 31,000 people, 31 countries): "75% of knowledge workers use AI at work today," and "78% of AI users are bringing their own AI tools to work (BYOAI)—it's even more common at small and medium-sized companies (80%)." Gallup (US, June 2025): 40% have used AI at work a few times a year or more, while "only 22% say their organization has communicated a clear plan or strategy." | https://www.nber.org/system/files/working_papers/w33777/w33777.pdf ; https://www.microsoft.com/en-us/worklab/work-trend-index/ai-at-work-is-here-now-comes-the-hard-part ; https://www.gallup.com/workplace/691643/work-nearly-doubled-two-years.aspx |
| 14 | **Employer backing raises take-up and benefits; this is not evidence for mandates.** Same NBER paper: "Encouraged use, Enterprise chatbots, and Training each raise extensive-margin take-up rates to 76%, 57%, and 69%, respectively." With all three in place, "93% of workers ... report having used AI chatbots at work, and 28% use them daily." Encouraged-use policies are "consistently associated with users reporting greater time savings, improved quality, and enhanced creativity." These are associations, and "encouraged" means allowed and promoted, not required. | https://www.nber.org/system/files/working_papers/w33777/w33777.pdf |
| 15 | **Peers and managers shape uptake; hands-on experience changes minds.** DBT: "Users were also anecdotally less likely to use M365 Copilot if their colleagues and line managers were hesitant about its use," and "self-led training [was] more effective than formal departmental training sessions." Gallup: "Sixty-eight percent of employees who had firsthand experience using AI to interact with customers said it had a positive effect ...; only 13% of employees who had not used AI with customers believed it would." | https://assets.publishing.service.gov.uk/media/68adbe409e1cebdd2c96a19d/dbt-microsoft-365-copilot-evaluation.pdf ; https://www.gallup.com/workplace/691643/work-nearly-doubled-two-years.aspx |
| 16 | **Clear direction from the top matters too.** Gallup: "When employees strongly agree that their leadership has communicated a clear plan for integrating AI, they are three times as likely to feel very prepared to work with AI and 2.6 times as likely to feel comfortable using AI in their role." | https://www.gallup.com/workplace/691643/work-nearly-doubled-two-years.aspx |
| 17 | **Pure opt-in can widen gaps.** PNAS (Humlum and Vestergaard; 18,000 Danish workers): "Women are 16 percentage points less likely to have used the tool for work." Comparing coworkers in the same workplace with similar tasks, "the gender gap shrinks to 12 percentage points." Workers "are often hindered by employer restrictions and a perceived need for training." | https://pubmed.ncbi.nlm.nih.gov/39793088/ |
| 18 | **Time saved doesn't show up as money yet.** The revised NBER paper estimates "precise null effects on earnings and recorded hours at both the worker and workplace levels, ruling out effects larger than 2% two years after the launch of ChatGPT." | https://www.nber.org/system/files/working_papers/w33777/w33777.pdf |
| 19 | **Governance is a real reason for central control.** UK Government AI Playbook principles include "You know how to use AI securely," "You have meaningful human control at the right stage" (including "ensuring that humans validate any high-risk decisions influenced by AI"), and "You work with commercial colleagues from the start." Grok Bot's own rollout checklist asks admins to review proxy and TLS inspection, sign-in method and inherited policies before rollout. | https://www.gov.uk/government/publications/ai-playbook-for-the-uk-government/artificial-intelligence-playbook-for-the-uk-government-html ; https://docs.x.ai/grok-bot/teams-and-enterprises |
| 20 | **lstack's structure as a worked pattern (structure only, no results).** "Files are the handoff." "A human approves every publish. No exceptions." "Work goes back to the previous step at most once." Each bot has a role file with OKRs, for example the Researcher's "KR1: 100% of claims sourced." | https://github.com/ZoneoutReal/lstack/blob/main/AGREEMENTS.md ; https://github.com/ZoneoutReal/lstack/blob/main/roles/researcher.md |

## Counterpoints
- **Mandated or centralized rollouts do some things better.** Security review, network controls, identity, data handling and procurement are easier to get right once than many times (claim 19). Several Grok Bot controls exist only on Enterprise (claim 7). The exec may reasonably say the pilot must clear security and commercial review first. The paper should invite that, not route around it.
- **Opt-in skews who benefits and what you learn.** Volunteers are not representative, which is why DBT added a random 30% (claim 12). Self-selected adoption shows a large gender gap (claim 17), and employer encouragement plus training raises take-up across the board (claim 14). A pure "raise your hand" pilot can measure the enthusiasts and miss everyone else.
- **Self-reported time savings are weak evidence.** The 26 minutes a day is self-reported (claim 10). DBT found no evidence that time savings improved productivity, and some tasks got slower and worse (claim 11). In Denmark, earnings and hours haven't moved (claim 18). An exec who distrusts "hours saved" has a point unless the pilot measures it carefully.
- **The cap is only as real as the settings.** There's no Grok Bot-only cap. Alerts don't stop spend. Seats bill per period, and removed seats stay billed until reduced (claims 5 and 6). If the cap and the seat count aren't set up front, the cost case falls apart. The topic requires this counterpoint to stay in.
- **Some work should stay off a bot.** The UK trial saw "limitations when dealing with complex, nuanced, or data-heavy aspects of work," and "Human oversight was required at all times." DBT reported hallucinations (https://www.gov.uk/government/publications/microsoft-365-copilot-experiment-cross-government-findings-report/microsoft-365-copilot-experiment-cross-government-findings-report-html ; claim 11). High-risk decisions need a human (claim 19). The topic requires this counterpoint to stay in.
- **Clear central direction helps.** Gallup links a communicated leadership plan with readiness (claim 16). The strongest version of the paper asks leadership to sanction and encourage the pilot. It shouldn't frame early adopters as going around leadership.

## Examples / data
**Pricing table (official; accessed Nov 16, 2026; US list prices, excluding tax):**

| Plan | Price | Grok Bot | Team Bots | Meetings |
|---|---|---|---|---|
| Free | $0/month | No | No | No |
| Plus | $8/month ($80/yr) | No | No | No |
| Premium | $30/month ($300/yr); team seat $30/seat | Yes | Team seat only | Team seat only |
| Super | $100/month ($1000/yr); team seat $100/seat | Yes | Team seat only | Team seat only |
| Ultra | $200/month ($2000/yr); team seat $200/seat | Yes | Team seat only | Yes (individual or team) |
| Enterprise | Contact sales (no list price) | Admin enables | Yes | Yes (admin turns on) |

The Team Bots and Meetings columns are inferred from claim 4's plan names ("Team, Enterprise, and Ultra"); "Team seat only" means available when the seat is on a Team plan. Sources: claims 1 to 4. Third-party models cost extra at list API prices (claim 1).

**Spend-ceiling template.** Every value is either a sourced list price or a blank to fill in. Don't publish invented values.
- Seat cost per billing period = [number of pilot seats] × [tier price: $30 / $100 / $200 per seat] (claim 3). A seat added mid-cycle is prorated (claim 6).
- Plus additional usage, capped at [monthly additional usage limit, $ blank] (claim 5). Set Auto Top-up off or bounded (claim 5).
- Maximum pilot spend = seat cost for each billing period the pilot touches + the additional usage limit for each calendar month it touches. The cap stops paid usage when it's hit; alerts don't (claim 5).
- Stop on [date blank] (four weeks per the topic). Before the period ends, remove members and Reduce seats so nothing renews (claim 6).

**Stop-rule ingredients (sourced pattern; values are blanks):**
- A pre-stated cost-versus-improvement test (claim 9).
- A fixed end date (claims 8 and 9).
- A participation mix: volunteers plus [some non-volunteers] (claim 12).
- A pre-defined measure of time saved that isn't only self-report (claims 10 and 11).
- Named off-limits work: high-risk decisions, and nuanced or data-heavy tasks without review (claim 19 and counterpoints).
- Kill if [usage below threshold blank], [spend reaches cap blank], or [quality incidents blank].

**Real-world pilot shapes to cite:**
- UK cross-government: 3 months, 20,000 licences, each organisation at least 1,000; earlier pilots at most 300 (claim 8).
- DBT: 3 months, 1,000 licences, about 70% volunteers and about 30% random (claims 8 and 12).

**lstack as the "how it runs" example:** human approval before publish, files as handoffs, OKRs per bot role (claim 20). Structure only, with no hours, spend or results.

**Clips:** the official Grok Bot 1.0 trailer (https://x.com/bot/status/2120582957782200586, about 79 seconds; post text: "Share Bots, collaborate with them in Slack and Teams, invite them to meetings"). Matt Palmer's walkthrough chapter "Team Bot improvements" (https://x.com/mattyp/status/2122343944889483583; chapter labels are his and haven't been timed). Describe moments; don't cite clock marks.

## Open questions
- How big is a Premium seat's weekly pool in real work (tasks or hours of Bot use)? Official pages give only multiples. The pilot will have to measure it.
- Can a pilot member on a Free team seat who personally pays for Premium use Team Bots through the team? The docs say Free seats draw "from their own personal plan," but don't say how Team Bots behave there.
- Which security and commercial reviews does the reader's company require before any self-serve team plan? That's company-specific; the paper should tell readers to ask.
- How should "hours saved" be measured in four weeks without relying only on self-report: task timing, before-and-after samples, or a comparison group?
- Is four weeks long enough? GOV.UK puts a typical discovery at 4 to 8 weeks, and the UK Copilot pilots ran 3 months.
- No study found compares opt-in with mandated AI rollouts head to head. The evidence covers bottom-up use, employer encouragement, and volunteer versus random samples. Is there a head-to-head study we missed?
- The x.ai/bot page shows "3.5x Premium usage" and "12x Premium usage," but the pricing pages imply 3.75x and 12.5x (15x and 50x over Plus, against Premium's 4x). Which is current?

## Dropped as unverifiable
- **Any unofficial Grok Bot dollar figures** and the Grok account's reply as a pricing source. It's superseded by the official pages (claim 4).
- **Australian Government (DTA) Copilot trial figures.** The official digital.gov.au report pages returned errors (HTTP 500, or no connection), so nothing could be confirmed at source.
- **Annie Duke's "kill criteria."** Only secondhand summaries were found; no primary text was fetched. The stop-rule material uses GOV.UK and the UK pilots instead.
- **Earlier-version Humlum and Vestergaard figures** ("47% to 83%" take-up; gender gap "11.9 to 5 percentage points"). They appear in the April 2025 working paper but not in the revised March 2026 NBER version. The brief uses only the revised figures (claims 13, 14 and 18) and the peer-reviewed PNAS paper (claim 17).
- **"Nearly 2 weeks a year" and "1,130 people a full year back"** (GOV.UK press release). These are scaled-up extrapolations from self-reported data. Use the report's own "26 minutes a day" with the self-report caveat if needed.
- **Any hours, spend or results from the lstack loop.** None exist in a source, and the topic forbids inventing them.

## Corrections to the pitch (for the writer)
- Pricing is now sourced from official pages (claims 1 to 3). Quote plan names and prices exactly, say they exclude tax and that third-party models cost extra, and note the access date.
- The "Team Bots need Team or Enterprise" and "Meetings need Team, Enterprise, or Ultra" reports are correct. Cite the official 1.0 post and docs, not the Grok reply.
- "Capped spend" has to mean two settings: a fixed number of seats at list price, plus a monthly additional usage limit. There's no Grok Bot-only cap, and alerts don't stop spend. Removed seats bill until reduced, effective at period end.
- On a self-serve Teams plan, every member gets Grok Bot and there's no off switch. The pilot's boundary is who's in the pilot's team workspace.
- The evidence doesn't show opt-in beats mandates. It shows people already use AI without waiting, that employer encouragement, tools and training raise take-up and reported benefits, and that volunteers aren't representative. Make the case as "a sanctioned, encouraged, bounded opt-in beats waiting," and invite leadership's security and commercial review.
- Don't claim hours saved for Grok Bot; there's no source. Treat the UK 26 minutes a day as self-reported and pair it with DBT's no-productivity-evidence finding.
- The lstack loop is a structural example only: human approval, files as handoffs, OKRs per bot. Don't imply results, spend or which tools Jon uses beyond what 01-topic.md says.
- Keep both required counterpoints visible: some work stays off a bot, and the cap and stop rule must be real.

## Addendum (Nov 20): US source and definition

Jon held the publish: his readers are American, so the Danish "used without employer encouragement" figure needs a US replacement, and the piece should define "sanctioned use" before using it. Everything below was checked at the original source on Fri Nov 20, 2026. Nothing above this section was changed.

### What this replaces
- **Claim 13, first sentence** (Humlum and Vestergaard: "about 41% have used AI chatbots at work at least once, and 7% use them daily" among Danish workers with no encouragement, enterprise chatbot or training). It is used in the hook of `04-final.md` and in pull quote 2 of `05-package.md`. Replace it with claim 13a.
- **Optional: the Danish figures in claim 14** (76%, 57%, 69%, 93%, 28%). Claim 13a includes a US version of "employer encouragement goes with much higher take-up." Claims 17 (Danish gender gap) and 18 (Danish earnings) are also Danish; Jon's note didn't cover them. See open questions.

### Replacement claims
| # | Claim | Source (link) |
|---|---|---|
| 13a | **US: some workers use generative AI without employer encouragement, and encouragement goes with far more use.** Bick, Blandin and Deming, using the Real-Time Population Survey (RPS), "a series of nationally representative U.S. surveys" (abstract): "The RPS asked workers 'Does your employer encourage you to use Generative AI for your job?'. Employer encouragement is highly correlated with adoption: 86% of respondents whose employer encourages genAI use report adopting it, compared to just 13% among those whose employer does not." (Working paper 2024-027F, Oct 2025 revision, p. 16.) Adoption at work is a yes to "Do you use Generative AI for your job?" (question wording, p. 5). In Table 1 (p. 17; August and November 2024 RPS waves, employed ages 18 to 64, N = 6,883), "a worker is 65 percentage points more likely to use genAI for work if their employer encourages them to do so," and the authors "caution that the estimated effect of employer encouragement is not necessarily causal." The paper is now published in *Management Science* (2026). | https://doi.org/10.20955/wp.2024.027 (resolves to the Fed PDF) ; published version: https://doi.org/10.1287/mnsc.2025.02523 (paywalled; the 13% sentence was checked only in the working paper) |
| 13b | **Most US employers haven't taken a side.** Pew Research Center (survey of 5,273 employed US adults, Oct 7 to 13, 2024): "Among all workers who are not self-employed, half say their employer neither encourages nor discourages the use of AI chatbots at work. Some 12% say their employer encourages it, and 8% say their employer discourages it." The 29% who hadn't heard of workplace AI chatbot use weren't asked (chart note, report p. 23). | https://www.pewresearch.org/social-trends/2025/02/25/workers-experience-with-ai-chatbots-in-their-jobs/ ; report PDF: https://www.pewresearch.org/wp-content/uploads/sites/20/2025/02/ST_2025.2.25_AI-Workers_REPORT.pdf |
| 13c | **US workers are the most likely to get employer support, yet many still get none.** Bick, Blandin, Deming, Fuchs-Schündeln and Jessen (Brookings Papers on Economic Activity conference draft, March 2026; worker survey Jan to Feb 2026, about 3,000 respondents per country): "The US also exhibits the lowest share of workers receiving none of the three supports we consider (44%, versus 69% in France and 70% in Italy)." The three supports are employer encouragement, AI training and AI tool provision (p. 28, Figure 14b). Their pooled figure that 10% of workers with no encouragement, training or tools adopted AI covers all countries together, with country fixed effects. It isn't a US figure, so don't use it as one. | https://www.brookings.edu/wp-content/uploads/2026/03/6%5FBick-et-al%5Funembargoed.pdf |

**Suggested wording for the writer** (the writer's call; stays within the sources): "Most US employers haven't said anything either way: half of workers say their employer neither encourages nor discourages AI chatbots (Pew). Some people use it anyway: 13% of US workers whose employer doesn't encourage generative AI say they use it for their job. Where employers do encourage it, 86% do (Bick, Blandin and Deming)."

### Is it a true US match for the Danish figure? Not exactly.
| | Denmark (Humlum and Vestergaard, claim 13) | US (Bick, Blandin and Deming, claim 13a) |
|---|---|---|
| Who | Workers in 11 occupations highly exposed to AI chatbots | All employed adults ages 18 to 64, nationally representative |
| Condition | Employer neither encourages chatbot use, nor provides an enterprise chatbot, nor offers training | Employer does not encourage genAI use (no condition on tools or training) |
| Outcome | Ever used AI chatbots at work (41%); daily use (7%) | Says yes to "Do you use Generative AI for your job?" (13%) |
| When | Late 2024 | August and November 2024 |

The US figure is the closest rigorous match found. It's lower than 41% mainly because it covers all workers, not only highly exposed occupations. **Don't put 41% and 13% side by side as a US-versus-Denmark comparison.** Also, "not encouraged" isn't the same as "unsanctioned": an employer can allow a tool without encouraging it. Neither study measures use the employer has forbidden or doesn't know about.

### Closest direct "unsanctioned use" US figure (weaker; use with care, or not at all)
- KPMG and the University of Melbourne, *Trust, attitudes and use of artificial intelligence: A global study 2025*. Led by Gillespie and Lockey (Melbourne Business School) with KPMG; 48,000+ people in 47 countries, including 1,019 in the US, Nov 2024 to Jan 2025. The US press release says: "Half of the U.S. workforce reported that they use AI tools at work without knowing whether it is allowed and more than four in ten (44%) are knowingly using it improperly at work." The US snapshot PDF shows "44% used AI in ways that contravene policies and guidelines" (p. 2, Workplace indicators). Caveats: the "half ... without knowing whether it is allowed" figure appears in the press release but not in the US snapshot; the base (all workers or AI-using workers) isn't stated next to the figures; and KPMG sells AI advisory services. It measures unsanctioned use more directly than 13a does, but it's less rigorous and less clear. Links: https://kpmg.com/us/en/media/news/trust-in-ai-2025.html ; https://kpmg.com/kpmg-us/content/dam/kpmg/pdf/2025/trust-attitudes-and-use-of-artificial-intelligence-us-summary-report.pdf

### Definition: sanctioned vs. unsanctioned ("shadow") AI use
- Puthal et al. (2025), *SN Computer Science* (peer-reviewed, open access), Introduction, paragraph 1: "Such deployment and usage of AI tools, models, or systems by employees of an organization without explicit endorsement, supervision, or management by IT and cyber security departments is defined as Shadow AI." The abstract says: "Shadow AI implies the usage of AI tools and systems by individuals within an entity, respectively, without permission thereby implying that these tools were not directly monitored or controlled by the centralized IT or security department." The article has no page numbers, so cite it by section and paragraph. https://link.springer.com/article/10.1007/s42979-025-03962-x
- No source found defines "sanctioned use" on its own; it's defined by contrast with shadow AI. Suggested plain-words definition, built from the quote: *sanctioned use* is AI use the organization has explicitly endorsed and supervises; *unsanctioned* or *shadow AI* is use without that endorsement or oversight. If the piece wants a quote, quote Puthal et al.; don't present our paraphrase as theirs.
- Not used: Ross, Hibbert and Moss (2025, IEEE ACDSA), "Shadow AI: Governance, Risk, and Organisational Resilience." Secondary summaries credit it with defining shadow AI as "the unsanctioned, informal use of artificial intelligence technologies within organisations," but IEEE Xplore returned 403 and the text couldn't be checked at source.

### Counterpoints and caveats
- **The US number makes "people aren't waiting" a weaker hook.** 13% is much lower than Denmark's 41%. The US evidence better supports "employer encouragement is the biggest lever" (86% vs 13%; 65 points in the regression) than "everyone's already doing it." The hook may need to lead with Pew's "half of employers are silent" and the encouragement gap instead.
- **Correlation, not causation.** The authors say the encouragement effect "is not necessarily causal as it may be highly correlated with a worker's roles and responsibilities."
- **Data age.** The 86%/13% split comes from 2024 survey waves. US use has risen since: Gallup's Q2 2026 workforce panel reports 52% use AI in their role (https://www.gallup.com/workplace/712736/organizational-adoption-jumps-six-points.aspx). But no newer public encouragement split was found.
- **Self-report.** All of these are survey answers. Shadow use is probably under-reported if people hide it, and the KPMG release says 53% "claim to present AI-generated content as their own."
- **The Microsoft and LinkedIn "78% BYOAI" figure in claim 13 is global and from a vendor.** It isn't a US figure. If the piece keeps it, say so; for a US-only paper, consider dropping it in favor of 13a and 13b.

### APA 7 references
Bick, A., Blandin, A., & Deming, D. J. (2025). *The rapid adoption of generative AI* (Working Paper No. 2024-027F). Federal Reserve Bank of St. Louis. https://doi.org/10.20955/wp.2024.027

Bick, A., Blandin, A., & Deming, D. J. (2026). The rapid adoption of generative AI. *Management Science, 72*(10), 8440–8456. https://doi.org/10.1287/mnsc.2025.02523

Bick, A., Blandin, A., Deming, D. J., Fuchs-Schündeln, N., & Jessen, J. (2026, March 26–27). *Mind the gap: AI adoption in Europe and the US* [Conference draft]. Brookings Papers on Economic Activity, Spring 2026, Washington, DC, United States. https://www.brookings.edu/wp-content/uploads/2026/03/6%5FBick-et-al%5Funembargoed.pdf

Lin, L., & Parker, K. (2025, February 25). *U.S. workers are more worried than hopeful about future AI use in the workplace*. Pew Research Center. https://www.pewresearch.org/social-trends/2025/02/25/u-s-workers-are-more-worried-than-hopeful-about-future-ai-use-in-the-workplace/

Puthal, D., Mishra, A. K., Mohanty, S. P., Longo, A., & Yeun, C. Y. (2025). Shadow AI: Cyber security implications, opportunities and challenges in the unseen frontier. *SN Computer Science, 6*(5), Article 405. https://doi.org/10.1007/s42979-025-03962-x

KPMG. (2025, April 29). *The American trust in AI paradox: Adoption outpaces governance* [Press release]. https://kpmg.com/us/en/media/news/trust-in-ai-2025.html (only if the KPMG figure is used)

Gillespie, N., Lockey, S., & KPMG. (2025). *Trust, attitudes and use of artificial intelligence: A global study 2025 — USA insights* [Fact sheet]. The University of Melbourne & KPMG. https://kpmg.com/kpmg-us/content/dam/kpmg/pdf/2025/trust-attitudes-and-use-of-artificial-intelligence-us-summary-report.pdf (only if the KPMG figure is used)

### Open questions
- Should the piece cite the *Management Science* version, the journal of record, or the open working paper? The 13% sentence was checked only in the working paper (Oct 2025); the journal page returned 403. If the writer cites the journal, someone with access should confirm the sentence survived peer review.
- Is there a newer US split of use by employer encouragement than the 2024 RPS waves? The public FRED series (RPSGENAIUSAGESHAREWORK) gives overall work use through 2026 Q3 but not by encouragement.
- Should claims 17 (Danish gender gap) and 18 (Danish null earnings effects) also get US replacements, or stay as clearly labeled international evidence? No US study with the same design was searched for in this pass.
- Does Jon want "sanctioned" defined as *endorsed and supervised by the organization*, the Puthal et al. framing, which centers IT and security, or more broadly as *allowed by the employer*? The two differ, and the US data measure *encouragement*, which is neither.

## Addendum 2 (Nov 20): hook decision and claims 17 and 18

### Decision note for Wade (approved by Chet)
- **The hook moves to the encouragement gap.** Lead with Bick, Blandin and Deming (claim 13a): "86% of respondents whose employer encourages genAI use report adopting it, compared to just 13% among those whose employer does not" (Working Paper 2024-027F, p. 16). Support it with Pew (claim 13b): "half say their employer neither encourages nor discourages the use of AI chatbots at work" (report p. 23).
- Retire the Danish 41%/7% hook. Don't set 13% against 41% as a country comparison (see the comparison table above).
- Keep the authors' caveat close by: the encouragement effect "is not necessarily causal."

### Claim 17 (Danish gender gap): REPLACED with a US figure
- **17-US.** Bick, Blandin and Deming (nationally representative US survey; August and November 2024 waves; employed ages 18 to 64): "Figure 3 documents demographic heterogeneity in work adoption of genAI. The top panel shows genAI adoption is 6 percentage points higher for men" (p. 10; Figure 3 on p. 11, N = 6,935).
- Table 1 (p. 17, N = 6,883) gives the same pattern as regression coefficients on "Female": −0.070 with demographic controls only; −0.048 after adding occupation controls; −0.018 after also adding "Employer Encourages AI Use." These are regression coefficients, so treat them as supporting detail, not a headline. They suggest the gap mostly tracks occupation and encouragement, and that fits the piece's argument for a deliberate, encouraged pilot over pure self-selection.
- **Caveat:** this isn't the Danish measure. Denmark found 16 points for ever using ChatGPT for work in exposed occupations, and 12 points within the same workplace. The US figure is a 6-point gap in current work use across all workers. Say "6 percentage points" for the US; don't carry over 16 or 12.
- **Link:** https://doi.org/10.20955/wp.2024.027
- **APA:** Bick, A., Blandin, A., & Deming, D. J. (2025). *The rapid adoption of generative AI* (Working Paper No. 2024-027F). Federal Reserve Bank of St. Louis. https://doi.org/10.20955/wp.2024.027

### Claim 18 (Danish null effects on earnings and hours): DROP: no verified US figure
- None of the sources read this session gave a checked US earnings or hours effect of AI use. The Bick, Blandin and Deming working paper has an earnings figure (Figure 4), but its results weren't checked at source. Per Jon's note, there was no new search.
- Wade: cut the Danish earnings sentence from the "be careful how" section. The UK self-report caveat (claim 10) and DBT's no-productivity-evidence finding (claim 11) still cover "time saved isn't proven value."

## Addendum 3 (Nov 20): Grok Bot vs enterprise AI tools

**Purpose (from Jon via Chet):** add a section that helps a non-technical exec see where Grok Bot fits next to Codex, ChatGPT Enterprise, Microsoft 365 Copilot and Gemini for Google Workspace. It should cover business capabilities and use cases, not only cost, and be framed as fit and differences, never as attacks.

**Method:** only official vendor pages and docs, all opened and read Fri Nov 20, 2026. Bracketed tags such as [G3] point to the APA list below. If a capability wasn't found on an official page, it's marked **UNVERIFIED**. That means "not confirmed," not "doesn't exist." These products change monthly, so re-check before publish.

**Writer floor:** no "better," "best" or "beats." Use "differs" and "fits when." Don't imply which tools Jon or lstack use.

### Correction to the Nov 16 brief (claim 4)
The Grok Bot meetings doc now says: "Meetings are available on Team, Enterprise, Ultra, and Super plans" [G4]. Claim 4 and the pricing table listed Team, Enterprise and Ultra only. Add **Super** to the Meetings column. Prices themselves are unchanged from Nov 16 [G1][G2].

### Comparison table (capability by tool, each cell sourced)
| Capability | Grok Bot | Codex (OpenAI) | ChatGPT Enterprise / Business | Microsoft 365 Copilot | Gemini for Google Workspace |
|---|---|---|---|---|---|
| **What it is, in one line** | An assistant that works from its own persistent cloud computer with a browser, command line and files [G6] | "OpenAI's coding agent that helps you write, review, and ship code" [O7] | ChatGPT workspace for teams; Business Standard seats "include access to ChatGPT, ChatGPT Work, and Codex" [O1] | AI assistant across Microsoft 365 apps; add-on to a Microsoft 365 plan [M1] | Gemini built into Workspace apps (Gmail, Docs, Meet) [W1] |
| **Shared or custom agents** | Team Bots: "share a Grok Bot with your team… They can use it in Grok Bot, Slack, Microsoft Teams, or even your calls" [G3] | Not a shared-agent product. Slack users can mention @ChatGPT, which "can send repository work to a separate Codex Cloud task" [O9] | Workspace agents: "share it with teammates or your workspace, use it in Slack, run it on a schedule, or trigger it through an API" [O2]. New custom GPT creation disabled for affected Enterprise workspaces from Oct 26, 2026; "Use Plugin Creator" instead [O3] | "Agent creation using Agent Builder and Copilot Studio"; pre-built "Researcher, Analyst, and Facilitator" agents [M1] | Gems: "customizable versions of Gemini"; "you can share Gems with other users in your organization and beyond" [W2] |
| **Scheduled or triggered work** | Routines run "on a schedule, or when something happens, such as a Slack message, a GitHub, Linear, Sentry, or PagerDuty event, an email, or a webhook call" [G5] | Scheduled tasks in the ChatGPT desktop app ("Schedule recurring tasks to run in the background") [O10] | Team tasks "run on a schedule or supported trigger, using approved company tools"; webhook triggers for "new Gmail messages, Slack channel messages, and GitHub pull request activity" [O3] | Scheduled prompts "at specified times and frequencies across Microsoft Teams, Office.com chat, and Microsoft Outlook"; "up to 10 active and 50 total schedules per user" [M4] | Gemini schedules: "up to 10 active schedules at a time" [W4]. Workspace Studio flows start from "an event, schedule, or… manually" [W5] |
| **Connectors and plugins** | "Connect apps" catalog. A Bot "can also add an MCP server that isn't in the catalog"; the team's MCP policy "applies in full" [G6][G7] | Plugins "can include skills and MCP servers"; one directory shared with ChatGPT [O11] | Same plugin directory [O11]; admins "configure app connections for teams" [O3] | Copilot connectors for external data [M1]. Copilot Studio offers prebuilt connectors and "Custom connectors… to connect to any publicly available API" [M6] | Schedules that use another app need it "connected" [W4]. Workspace Studio steps reach "Gmail, Sheets, and Drive, as well as other common apps" [W5]. Breadth of third-party connectors: **UNVERIFIED** |
| **Computer use or agent mode** | Persistent cloud computer; "files, sign-ins, and browser sessions persist between tasks" [G6] | Codex Cloud "runs coding tasks on OpenAI-managed computers" [O7]. Desktop Computer Use on macOS and Windows [O12] | Dots and Work Cloud: admin toggles for "Cloud browser use," "Cloud network access," "Cloud computer use" [O4] | Copilot Studio computer use "lets your agent interact with and automate tasks on a Windows computer" you set up; "bills usage through the Agent action feature with a billing rate of five Copilot Credits" [M5] | Chrome auto browse: "Gemini works in Chrome browser tabs to complete multi-step tasks"; "off by default for managed users" [W6] |
| **Joins meetings** | Joins "Google Meet, Zoom, or Microsoft Teams calls… listens, takes notes, answers questions in the meeting chat" [G4] | **UNVERIFIED** (no meeting feature found; it's a coding agent) | Record transcribes meetings ("only available for the macOS desktop app"). With Google Calendar connected, it can "join on schedule," but "Calendar auto-join currently supports Google Meet links only"; Zoom and Teams need a manual start [O5]. Answering in the meeting chat like a participant: **UNVERIFIED** | Facilitator in Teams meetings "Answers open-ended questions in the meeting chat"; "can only be added to scheduled meetings" [M3] | Meet note-taking: "a Google Doc with the notes is emailed to the organizer"; Business Standard and up [W3] |
| **Admin and data controls (examples)** | SCIM; Enterprise-only items include "Network Controls… Enforce Auto-review"; with Privacy Mode "customer data is not used for training" [G7] | Enterprise: "SCIM, EKM… RBAC… Audit logs… via the Compliance API… Data retention and data residency controls" [O6] | Business: "OpenAI won't train on your workspace's data" [O1]; admin controls for dots and agents [O2][O4] | "Enterprise Data Protection (EDP), management, compliance, and controls" [M2]; scheduled-task data "stored within the Microsoft 365 compliance boundary" [M4] | Work accounts: chats "won't be reviewed by human reviewers or otherwise used to improve generative AI models" [W7] |
| **Public list price (US)** | Team seats: Premium $30, Super $100, Ultra $200 per seat per month; Enterprise via sales [G2][G1] | Included in ChatGPT plans. Business "$20 / user / month" annual, "$25 per user per month when billed monthly"; Enterprise "Contact sales" [O6] | Business Standard seat $25 monthly or $20 annual; Premium seat $125 monthly or $100 annual [O1]. Enterprise: no public price (contact sales) [O6] | Enterprise add-on "$30.00 user/month, paid yearly", plus "a qualifying Microsoft 365 plan" [M1]. Copilot Business add-on "starting from $18.00" (promo; was $21.00) [M2] | Business Starter $7, Standard $14, Plus $22 per user per month, each listing a "Gemini AI assistant"; Enterprise "Contact sales" [W1]. Billing term for those figures: **UNVERIFIED** (see open questions) |

### "Fits when" use cases (from the documented capabilities above; no performance claims)
- **Grok Bot fits when** a team wants one shared assistant that works in Slack and Microsoft Teams and joins Meet, Zoom and Teams calls, answering in the meeting chat [G3][G4]. It also fits when the team wants work to run on triggers from tools like GitHub, Linear or PagerDuty [G5], or on its own persistent computer for browser tasks [G6]. That fits a small, mixed-tool pilot team.
- **Codex fits when** the work is mainly code: repository tasks in the cloud, from Slack, or on the desktop [O7][O9][O12]. It comes with ChatGPT plans rather than as a separate purchase [O6].
- **ChatGPT Enterprise or Business fits when** a company wants a broad ChatGPT workspace with shared agents, team tasks and the Codex coding agent under one admin console [O1][O2][O3].
- **Microsoft 365 Copilot fits when** the company already runs on Microsoft 365 and Teams and wants AI inside Outlook, Word and Teams meetings [M1][M3]. It also fits when the company wants agents built in Copilot Studio with Power Platform connectors [M6].
- **Gemini for Google Workspace fits when** the company runs on Gmail, Docs and Meet and wants AI included in the Workspace subscription [W1], with Meet note-taking [W3] and shared Gems [W2].
- **Honest framing for the exec:** if the company already pays for Microsoft 365 Copilot or a Workspace edition with Gemini, the first question is what that tool doesn't cover for this team. The pilot then tests the difference, for example cross-platform meetings, event-triggered routines or a persistent bot computer. It isn't a replacement decision.

### Caveats and counterpoints
- **Overlap is large.** Every tool now has some form of shared agents, schedules, connectors and browser automation. The differences are mostly in *where* the tool lives (Slack, Teams or Workspace), *which* meetings it joins, and *how* it's bought and governed. Don't present any single feature as unique without a source.
- **Bundling matters to a cost-minded exec.** Gemini is included in Workspace plans [W1], and Codex is included in ChatGPT plans [O6]. Microsoft 365 Copilot is an add-on to an existing plan [M1]. A Grok Bot pilot is a separate line item [G2].
- **Feature churn.** Custom GPTs are being retired for affected Enterprise workspaces ("Dec 11, 2026 for standard retirement") [O3], and Microsoft's Power Platform scheduled prompts retire Dec 31, 2026 [M4]. Re-check before publish.
- **Metered extras.** Microsoft lists Cowork, Autopilot and agent usage as metered or usage-based [M1][M2]. OpenAI and Grok Bot both sell usage beyond included limits [O1][G2]. List price isn't total cost.
- **Defaults.** Several capabilities are off by default and need an admin: ChatGPT Enterprise workspace agents [O2], Gemini auto browse [W6], and some Grok Bot controls that are Enterprise only [G7]. A pilot needs admin time on any of them.

### UNVERIFIED (not confirmed on an official page this pass)
1. Codex: any meeting participation.
2. ChatGPT Enterprise: whether Record acts as a meeting participant (answers in the meeting chat). Confirmed: macOS Record, plus calendar auto-join for Google Meet links only. The same page says the newer Meetings plugin has "Windows and ChatGPT Enterprise support coming soon," while listing Record as available for Enterprise. Treat Enterprise meeting features as in flux.
3. Gemini for Workspace: breadth of third-party, non-Google connectors.
4. Google Workspace: whether $7, $14 and $22 are annual or flexible (monthly) prices. The page shows a promo and an annual toggle, and the static text didn't say which plan the figures belong to.
5. ChatGPT Enterprise and Gemini Enterprise list prices (sales-led; none published).
6. Microsoft Facilitator in non-Teams meetings (docs describe Teams meetings only).

### APA 7 references (all accessed November 20, 2026)
- [G1] xAI. (n.d.). *Pricing*. Retrieved November 20, 2026, from https://x.ai/pricing
- [G2] xAI. (n.d.). *Pricing* [The X Subscription documentation]. Retrieved November 20, 2026, from https://docs.x.ai/x-subscription/pricing
- [G3] xAI. (n.d.). *Team Bots* [Grok Bot documentation]. Retrieved November 20, 2026, from https://docs.x.ai/grok-bot/team-bots
- [G4] xAI. (n.d.). *Add a Bot to your meetings* [Grok Bot documentation]. Retrieved November 20, 2026, from https://docs.x.ai/grok-bot/meetings
- [G5] xAI. (n.d.). *Skills and routines* [Grok Bot documentation]. Retrieved November 20, 2026, from https://docs.x.ai/grok-bot/skills-routines-and-automations
- [G6] xAI. (n.d.). *Use the computer and apps* [Grok Bot documentation]. Retrieved November 20, 2026, from https://docs.x.ai/grok-bot/computer-and-apps
- [G7] xAI. (n.d.). *Grok Bot for teams and enterprises* [Grok Bot documentation]. Retrieved November 20, 2026, from https://docs.x.ai/grok-bot/teams-and-enterprises
- [O1] OpenAI. (n.d.). *ChatGPT Business overview*. OpenAI Help Center. Retrieved November 20, 2026, from https://help.openai.com/en/articles/8792828-chatgpt-business-overview
- [O2] OpenAI. (n.d.). *ChatGPT workspace agents for Enterprise and Business*. OpenAI Help Center. Retrieved November 20, 2026, from https://help.openai.com/en/articles/20001143-chatgpt-workspace-agents-for-enterprise-and-business
- [O3] OpenAI. (n.d.). *ChatGPT Enterprise and Edu release notes*. OpenAI Help Center. Retrieved November 20, 2026, from https://help.openai.com/en/articles/10128477-chatgpt-enterprise-and-edu-release-notes
- [O4] OpenAI. (n.d.). *Managing dots in ChatGPT workspaces*. OpenAI Help Center. Retrieved November 20, 2026, from https://help.openai.com/en/articles/20001554-managing-dots-in-chatgpt-workspaces
- [O5] OpenAI. (n.d.). *ChatGPT Record*. OpenAI Help Center. Retrieved November 20, 2026, from https://help.openai.com/en/articles/11487532-chatgpt-record
- [O6] OpenAI. (n.d.). *Pricing* [Codex documentation]. Retrieved November 20, 2026, from https://developers.openai.com/codex/pricing
- [O7] OpenAI. (n.d.). *Using Codex with your ChatGPT plan*. OpenAI Help Center. Retrieved November 20, 2026, from https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan
- [O9] OpenAI. (n.d.). *Use ChatGPT in Slack* [Codex documentation]. Retrieved November 20, 2026, from https://developers.openai.com/codex/third-party/slack
- [O10] OpenAI. (n.d.). *Scheduled tasks* [Codex documentation]. Retrieved November 20, 2026, from https://developers.openai.com/codex/automations
- [O11] OpenAI. (n.d.). *Plugins* [Codex documentation]. Retrieved November 20, 2026, from https://developers.openai.com/codex/plugins
- [O12] OpenAI. (n.d.). *Computer Use* [Codex documentation]. Retrieved November 20, 2026, from https://developers.openai.com/codex/computer-use
- [M1] Microsoft. (n.d.). *Microsoft Copilot plans and pricing: Enterprise*. Retrieved November 20, 2026, from https://www.microsoft.com/en-us/copilot/pricing/enterprise
- [M2] Microsoft. (n.d.). *Microsoft Copilot plans and pricing: AI for business*. Retrieved November 20, 2026, from https://www.microsoft.com/en-us/copilot/pricing/business
- [M3] Microsoft. (n.d.). *Facilitator in Microsoft Teams meetings*. Microsoft Support. Retrieved November 20, 2026, from https://support.microsoft.com/en-us/teams/copilot/facilitator-in-microsoft-teams-meetings
- [M4] Microsoft. (n.d.). *Manage scheduled prompts for Microsoft Copilot*. Microsoft Learn. Retrieved November 20, 2026, from https://learn.microsoft.com/en-us/copilot/manage/scheduled-prompts
- [M5] Microsoft. (n.d.). *Automate web and desktop apps with computer use*. Microsoft Learn. Retrieved November 20, 2026, from https://learn.microsoft.com/en-us/microsoft-copilot-studio/computer-use
- [M6] Microsoft. (n.d.). *Use connectors in Copilot Studio agents*. Microsoft Learn. Retrieved November 20, 2026, from https://learn.microsoft.com/en-us/microsoft-copilot-studio/advanced-connectors
- [W1] Google. (n.d.). *Compare flexible pricing plan options*. Google Workspace. Retrieved November 20, 2026, from https://workspace.google.com/pricing
- [W2] Google Workspace. (2025, September 18). *Introducing Gems sharing in the Gemini app, including admin controls*. Google Workspace Updates. https://workspaceupdates.googleblog.com/2025/09/gem-sharing-gemini-app-workspace.html
- [W3] Google. (n.d.). *Let Google Meet AI take notes for my users*. Google Workspace Help. Retrieved November 20, 2026, from https://knowledge.workspace.google.com/admin/meet/let-google-meet-ai-take-notes-for-my-users
- [W4] Google. (n.d.). *Schedules in Gemini Apps*. Gemini Apps Help. Retrieved November 20, 2026, from https://support.google.com/gemini/answer/16316416?hl=en
- [W5] Google. (n.d.). *Get started with Google Workspace Studio*. Workspace Studio Help. Retrieved November 20, 2026, from https://support.google.com/workspace-studio/answer/16444479?hl=en
- [W6] Google. (n.d.). *Gemini in Chrome*. Chrome Enterprise and Education Help. Retrieved November 20, 2026, from https://support.google.com/chrome/a/answer/16291696?hl=en
- [W7] Google. (n.d.). *Use Gemini Apps with a work or school Google Account*. Gemini Apps Help. Retrieved November 20, 2026, from https://support.google.com/gemini/answer/14620100?hl=en&co=DASHER._Family%3DBusiness-Enterprise

### Open questions
- Does Jon want Codex as its own column? OpenAI now sells Codex inside ChatGPT plans [O1][O6], so for an exec the real choice may be "ChatGPT Business/Enterprise (with Codex)." Merging the two columns would shorten the table.
- Should the piece show Microsoft's $18 Copilot Business promo price, or only the $30 enterprise add-on? The promo may expire before publish.
- Google Workspace billing term for $7/$14/$22 (UNVERIFIED #4): check the live page's Annual/Flexible toggle before quoting.
- The table is too wide for a one-page exec handout. Wade may want to cut it to four rows (shared agents, scheduled work, meetings, price) and move the rest to an appendix.

## Addendum 4 (Nov 20): productivity case replaces cost

**Change (Jon via Chet):** drop the cost argument. Enterprise prices aren't public, and the reader is a company, so cost comparisons are weak. Make the case on productivity instead: time saved, and less mental strain on simple, repeatable work. The reader is still an engineering manager handing this to a non-technical executive.

**Method:** every figure below is quoted word for word from the original document, with its page or section, checked on Fri Nov 20, 2026. Each source is labeled by where the people studied were and who paid for or ran the study. Nothing is estimated or rounded.

### Which examples the evidence supports (strongest first)
1. **Email (strongest).** This is the only randomized field experiment on everyday office tools, run across 66 firms. See claim P1.
2. **Customer escalations (strong, one company).** Requests to "speak to a manager" fell in a large field study. See claim P2.
3. **Drafting routine documents (strong, but in a test setting).** A randomized online experiment. See claim P3.
4. **Notes from conversations (good evidence on strain and burnout, but from doctors' visit notes, not office meetings).** See claim P4. In the email experiment, time spent *in* meetings didn't change (claim P1). Promise better notes and less note-taking strain, not shorter meetings.
5. **Status summaries and ticket routing: no verified study found.** Don't use them as evidence-backed examples. They can appear as "ideas to test in the pilot," labeled as untested.

### Productivity claims (new)
| # | Claim | Source and location | Label |
|---|---|---|---|
| P1 | **Email time fell; meeting time didn't.** "We present evidence from a field experiment across 66 firms and 7,137 knowledge workers. Workers were randomly selected to access a generative AI tool integrated into applications they already used at work for email, meetings, and writing. In the second half of the 6-month experiment, the 80% of treated workers who used this tool spent two fewer hours on email each week and reduced their time working outside of regular hours" (abstract). On p. 7: "workers with access to Copilot spent an average of 1.4 (2) fewer hours per week in email sessions over post-period months 4-6, a 12% (17%) decline from their pre-period average." On meetings, p. 7: "We find no similar shifts in the time workers spent in Teams meetings or working in Word." After hours, p. 7: "workers spent a quarter of an hour less per week working outside of their modal work hours, a 9% reduction." | Dillon et al. (2025), National Bureau of Economic Research Working Paper 33795. https://www.nber.org/system/files/working_papers/w33795/w33795.pdf | Randomized field experiment, not peer-reviewed. "The experiment includes workers from many countries, with the majority based in the United States or Europe" (p. 19). Three of the four authors are at Microsoft Research, and the tool tested was Microsoft 365 Copilot. In the 1.4 (2) style, the first number is everyone given access and the number in brackets is those who actually used it. |
| P2 | **Fewer escalations, faster resolution, less staff turnover in customer support.** "Access to the tool increases productivity, as measured by issues resolved per hour, by 14% on average, including a 34% improvement for novice and low-skilled workers but with minimal impact on experienced and highly skilled workers" (abstract). On p. 26: "AI assistance generates an almost 25% decline in customer requests to speak to a manager." On staff leaving, also p. 26: among agents with under six months' experience, "around 10 percentage points, translates into a 40% decrease relative to a baseline attrition rate in this group of 25%." The authors add that the attrition results "should be taken with more caution relative to our main results." | Brynjolfsson, Li and Raymond (2023), National Bureau of Economic Research Working Paper 31161, revised November 2023. https://www.nber.org/system/files/working_papers/w31161/w31161.pdf. Published later in *The Quarterly Journal of Economics* (2025). | Field study of 5,179 support agents at one US software firm, where "89%, are located outside of the United States, primarily in the Philippines" (p. 11). Figures were checked in the working paper only; the journal version may differ slightly. |
| P3 | **Routine drafting gets faster without losing quality.** "In a preregistered online experiment, we assigned occupation-specific, incentivized writing tasks to 453 college-educated professionals and randomly exposed half of them to ChatGPT. Our results show that ChatGPT substantially raised productivity: The average time taken decreased by 40% and output quality rose by 18%" (abstract, p. 187). The tasks "included writing press releases, short reports, analysis plans, and delicate emails" (p. 187). | Noy and Zhang (2023), *Science*. Author copy: https://shakkednoy.com/noy-zhang.pdf. DOI below (the publisher page blocked my link check). | Peer-reviewed randomized experiment. These were 20- to 30-minute test tasks on an online survey platform, not real jobs, and the paper doesn't say what country participants were in. |
| P4 | **Automatic notes cut note-taking strain and burnout (doctors).** "After 30 days with an ambient AI scribe, burnout among those working in ambulatory clinics decreased significantly from 51.9% to 38.8%. There were also significant improvements in the cognitive task load, time spent documenting after hours, focused attention on patients, and urgent access to care" (Key Points). From the abstract results: improvement in "note-related cognitive task load (mean [SE] difference, 2.64 [0.13] points)" on 10-point scales, and "time spent documenting after hours (mean [SE] difference, 0.90 [0.19] hours)." | Olson et al. (2025), *JAMA Network Open*. Open copy: https://pmc.ncbi.nlm.nih.gov/articles/PMC12492056/ | Peer-reviewed, 263 clinicians in "6 academic and community-based health care systems across the US." But: "There was no control group to adjust for temporal trends"; "participation was voluntary"; and two authors work for or held posts at the scribe vendor, Abridge AI (disclosures). This is doctors' visit notes, not office meetings, so treat it as the closest real evidence on strain from note-taking. |
| P5 | **People feel less mental effort, but the work shifts to checking.** In 936 real work examples from 319 knowledge workers, "examples that were reported as 'much less effort' or 'less effort' comprise 72% in Knowledge, 79% in Comprehension, 69% in Application, 72% in Analysis, 76% in Synthesis, and 55% in Evaluation" (section 5.1, p. 12). The same paper: "For tasks like knowledge retrieval, AI reduces effort by automating information gathering, but workers must now invest more in verifying the accuracy of AI outputs" (p. 2). It also found that "higher confidence in GenAI is associated with less critical thinking" (abstract). | Lee et al. (2025), Conference on Human Factors in Computing Systems (CHI 2025). https://www.microsoft.com/en-us/research/wp-content/uploads/2025/01/lee_2025_ai_critical_thinking_survey.pdf | Peer-reviewed conference survey, all self-reported. Mostly non-US: US participants were "20 (6.27%)" (Table 3). Six of the seven authors are at Microsoft Research. |
| P6 | **Across US workers, reported time savings are real but modest.** "Based on self-reported time savings due to genAI, the average genAI user would need to work 5.2% more hours in order to complete their work without genAI, implying 1.4% time savings across all workers (including non-users)" (p. 2). | Bick, Blandin and Deming (2025), Federal Reserve Bank of St. Louis Working Paper 2024-027F (already in the brief as claim 13a). https://doi.org/10.20955/wp.2024.027 | US, nationally representative, but self-reported. |

**Suggested plain-words line for the writer** (stays inside the sources): "The best evidence says AI helps most with routine work. In a large randomized trial, workers who used an AI assistant spent about two fewer hours a week on email (Dillon et al.). In customer support, requests to speak to a manager fell by almost a quarter (Brynjolfsson et al.). Doctors using automatic note-taking reported less burnout and less mental strain from paperwork, though that study had no comparison group (Olson et al.)."

### Counterpoints (keep at least two in the piece)
- **Most time savings are self-reported.** P5 and P6 rest on people's own estimates, and P4 on before-and-after surveys with no comparison group. The UK trial's 26 minutes a day is also self-reported, and the UK Department for Business and Trade (DBT) found no productivity evidence (claims 10 and 11). The pilot should time real tasks, not only ask people.
- **AI output can create review work for others ("workslop").** In an online survey of 1,150 full-time US desk workers (August to September 2025), "40% of desk workers received workslop in the last month," with "1hr56m lost per incident" (BetterUp Labs and Stanford Social Media Lab one-page summary, p. 1). This is **vendor research**: BetterUp sells coaching services, and its chief scientist is the lead author of the related Harvard Business Review article. The full article is paywalled, so these figures were checked only in the BetterUp summary. Lee et al. (P5) independently find that effort shifts toward "verifying the accuracy of AI outputs."
- **Saved time may not show up in output or pay.** In P1: "Apart from these individual time savings, we do not detect shifts in the quantity or composition of workers' tasks" (abstract), and "much of the time saved appears to have shifted to activities we cannot measure" (p. 7). In Denmark (non-US, labeled), Humlum and Vestergaard "estimate precise null effects on earnings and recorded hours at both the worker and workplace levels, ruling out effects larger than 2% two years after the launch of ChatGPT" (National Bureau of Economic Research Working Paper 33777, revised March 2026, abstract).
- **Gains are uneven.** P2 found "minimal impact on experienced and highly skilled workers." DBT found Excel analysis got slower and worse (claim 11). Gains concentrate in routine work done by less experienced staff.
- **Less effort can mean less checking.** P5: "higher confidence in GenAI is associated with less critical thinking." The pilot should name who reviews AI output, and where.

### Cut or demote, now that cost is out
| Brief item | Action | Why |
|---|---|---|
| "Reader and promise": "answers the 'not worth the cost' objection with official list prices… weigh pilot cost against time saved" | **Rewrite** | The promise changes to: "shows where AI saves time and mental effort on routine work, with a stop rule written before the pilot starts." |
| Claims 1 to 3 (individual and team list prices; which plans include Grok Bot) | **Footnote** (one line) | Without the cost argument, prices are only admin detail. One footnote is enough: "Grok Bot is included on Premium, Super and Ultra; team seats are priced per seat; see x.ai/pricing." Drop the yearly prices and usage multiples. |
| Claim 4 (which plans include Team Bots and Meetings) | **Keep as a footnote**, with Addendum 3's correction (add Super to Meetings) | It's capability, not cost: the meeting-notes example needs a plan that includes Meetings. |
| Claim 5 (spending cap) and claim 6 (stop and seat-billing mechanics) | **Footnote** | A pilot still needs a spend ceiling set by the admin, but it's no longer an argument. One sentence: "Set a monthly usage limit; alerts alone don't stop spend." |
| Claim 7 (pilot boundary is team membership) | **Keep** | It's about scope and governance, not cost. |
| Claim 9 (GOV.UK: weigh cost against improvement; stopping is legitimate) | **Keep, reframed** | Keep "It's not a failure to stop" and the 4-to-8-week guidance. Drop the "cost effective" quote, or make the improvement test about time and quality. |
| Pricing table (Examples / data) | **Cut** | It's the core of the cost argument and goes stale fast. |
| Spend-ceiling template | **Cut**, leaving a one-line footnote | Same reason. |
| Stop-rule ingredients | **Keep, edit** | Replace "cost-versus-improvement test" with "a time-and-quality test measured before and after (timed tasks, not only self-report)." Replace "spend reaches cap" with "review burden grows (workslop)." |
| Counterpoint "The cap is only as real as the settings" | **Footnote** | It was required by the cost framing. Replace it in the main text with the workslop / review-burden counterpoint above. |
| Corrections to the pitch: first bullet (pricing) and "Capped spend" bullet | **Footnote** | They're no longer central. |
| Open question on usage multiples (3.5x vs 3.75x) | **Cut** | It matters only for cost. |
| Addendum 3: "Public list price (US)" row | **Cut**; put one footnote under the table: "Pricing: Grok Bot team seats are listed per seat; ChatGPT Enterprise and Gemini Enterprise prices aren't public; Microsoft 365 Copilot is an add-on to a Microsoft 365 plan." | Mixed public and private prices invite exactly the comparison Jon wants to avoid. |
| Addendum 3 caveats "Bundling matters to a cost-minded exec" and "Metered extras" | **Footnote**, or cut | They're cost-only. The "already pay for Copilot or Gemini? test the difference" framing in "fits when" stays, because it's about fit. |
| Addendum 3 UNVERIFIED items 4 and 5 (Workspace billing term; enterprise prices not public) | **Cut** | They're no longer needed. |

**Table rows to keep (Addendum 3), so it stays readable for an executive:** four rows.
1. **Shared or custom agents.** This is the team angle.
2. **Scheduled or triggered work.** Repeatable work is the heart of the productivity case.
3. **Joins meetings.** It ties directly to the notes example and to P4.
4. **Admin and data controls.** Executives ask about this first.

Move "What it is," "Connectors and plugins" and "Computer use" to an appendix or cut them. Cut the price row.

### APA 7 references (all checked November 20, 2026)
Brynjolfsson, E., Li, D., & Raymond, L. R. (2023). *Generative AI at work* (Working Paper No. 31161). National Bureau of Economic Research. https://www.nber.org/system/files/working_papers/w31161/w31161.pdf

Brynjolfsson, E., Li, D., & Raymond, L. (2025). Generative AI at work. *The Quarterly Journal of Economics, 140*(2), 889–942. https://doi.org/10.1093/qje/qjae044 (journal version; figures above were checked in the working paper)

Dillon, E. W., Jaffe, S., Immorlica, N., & Stanton, C. T. (2025). *Shifting work patterns with generative AI* (Working Paper No. 33795). National Bureau of Economic Research. https://www.nber.org/system/files/working_papers/w33795/w33795.pdf

Noy, S., & Zhang, W. (2023). Experimental evidence on the productivity effects of generative artificial intelligence. *Science, 381*(6654), 187–192. https://doi.org/10.1126/science.adh2586

Olson, K. D., Meeker, D., Troup, M., Barker, T. D., Nguyen, V. H., Manders, J. B., Stults, C. D., Jones, V. G., Shah, S. D., Shah, T., & Schwamm, L. H. (2025). Use of ambient AI scribes to reduce administrative burden and professional burnout. *JAMA Network Open, 8*(10), Article e2534976. https://doi.org/10.1001/jamanetworkopen.2025.34976

Lee, H.-P., Sarkar, A., Tankelevitch, L., Drosos, I., Rintel, S., Banks, R., & Wilson, N. (2025). The impact of generative AI on critical thinking: Self-reported reductions in cognitive effort and confidence effects from a survey of knowledge workers. In *Proceedings of the 2025 CHI Conference on Human Factors in Computing Systems* (pp. 1–22). Association for Computing Machinery. https://doi.org/10.1145/3706598.3713778

Bick, A., Blandin, A., & Deming, D. J. (2025). *The rapid adoption of generative AI* (Working Paper No. 2024-027F). Federal Reserve Bank of St. Louis. https://doi.org/10.20955/wp.2024.027

BetterUp Labs & Stanford Social Media Lab. (2025). *The hidden cost of workslop: What the numbers mean for your organization* [Research summary]. BetterUp. https://www.betterup.com/hubfs/Post-Uplift%20content/BetterUp_Uplift_The%20hidden%20cost%20of%20workslop.pdf

Niederhoffer, K., Kellerman, G. R., Lee, A., Liebscher, A., Rapuano, K., & Hancock, J. T. (2025, September 22). AI-generated "workslop" is destroying productivity. *Harvard Business Review*. https://hbr.org/2025/09/ai-generated-workslop-is-destroying-productivity (paywalled; figures checked in the BetterUp summary above)

Humlum, A., & Vestergaard, E. (2026). *Still waters, rapid currents: Early labor market transformation under generative AI* (Working Paper No. 33777, rev. ed.). National Bureau of Economic Research. https://www.nber.org/system/files/working_papers/w33777/w33777.pdf

### Open questions
- **Meeting notes have no direct office-meeting study.** The best evidence is doctors' visit notes (P4), and the email trial found no change in meeting time (P1). Is Jon OK with framing meeting notes as "less strain and fewer after-hours catch-ups," not "time saved"?
- **Escalations:** the evidence (P2) is customers asking for a manager in a support center, not internal engineering escalations. Should the piece use the support example as is, or say plainly that internal escalations are untested?
- **Vendor ties:** P1 and P5 come from Microsoft Research, P4 has authors tied to the scribe vendor, and workslop comes from BetterUp. None tested Grok Bot. Should the piece say outright that no independent study of Grok Bot exists?
- **The pilot's own measure:** without cost, the stop rule needs a time-and-quality test. A suggestion to adapt, not a finding: time 3 to 5 routine tasks (for example, weekly email triage or drafting status notes) before and during the pilot, and count review rework.

## Addendum 5 (Nov 20): exec pilot case (W47) + W48 notes

**Change (Jon, Direction update 5 in 01-topic.md, commit f76fa55):** the work is split in two. W47 becomes a tool-agnostic case for an executive to sanction a capped, opt-in pilot of AI agents across several use cases. W48 becomes the Grok Bot role-team article. Every new quote below was checked at the original on Fri Nov 20, 2026, and every link opened. Claims reused from earlier in this brief are cited by number and were not re-checked.

### 1. What the evidence supports for a multi-tool, multi-use-case opt-in pilot
**Supported (reuse first):**
- **Several use cases at once is normal in real pilots.** The email trial gave workers a tool "integrated into applications they already used at work for email, meetings, and writing" (Dillon et al., Addendum 4, P1). The UK cross-government and Department for Business and Trade (DBT) pilots covered many everyday uses (claims 8, 10, 11).
- **Gains differ by use case, so judge each use case separately.** Email time fell but meeting time didn't (P1). DBT found "Small time savings were observed across most use cases," but users "completed Excel data analysis more slowly and to a worse quality and accuracy than non-users" (claim 11).
- **Opt-in pilots draw volunteers who aren't typical** (claims 12 and 17; Bick et al. in the final).
- **New, US, fills the "real multi-use-case opt-in pilot" gap:** the Commonwealth of Pennsylvania's yearlong pilot. "The Commonwealth equipped 175 employees to use ChatGPT Enterprise" (p. 8), from "14 state government agencies" (p. 9). "These employees volunteered to explore this new technology" (p. 2). Uses spread across tasks: "Writing assistance, text generation, drafting emails 36%," "Research, idea exploration, learning new topics 27%," "Summarizing 13%" (p. 16). "Users estimated saving 95 minutes per day with ChatGPT" (p. 3). But "Pilot participants were not a representative sample of Commonwealth employees" (p. 12), and "ChatGPT reduced, but did not eliminate, human input into final work products" (p. 34). *Label: US state government; one tool; self-reported time ("Estimates reported by participants in exit survey," p. 33); OpenAI ran some trainings ("OpenAI led trainings," p. 11).*
- **New: self-reported speed-ups can point the wrong way, so time the work.** In a randomized trial with 16 experienced open-source developers, "developers forecast that allowing AI will reduce completion time by 24%. After completing the study, developers estimate that allowing AI reduced completion time by 20%. Surprisingly, we find that allowing AI actually increases completion time by 19%" (abstract, p. 1). The authors "show that both experts and developers drastically overestimate the usefulness of AI on developer productivity, even after they have spent many hours using the tools" (p. 10). They also "caution readers against overgeneralizing on the basis of our results" (p. 12). *Label: Model Evaluation & Threat Research (METR) preprint, not peer-reviewed; small sample; expert coders on code they knew well, not routine office work.*

**Thin or missing (say so plainly in the article):**
- **Multi-tool:** every study in this brief tested one tool (Microsoft 365 Copilot in Dillon, the UK and DBT; ChatGPT in Noy and Zhang and in Pennsylvania; one support-chat AI assistant in Brynjolfsson). I found **no study of a pilot that ran several different AI tools side by side**, and no study comparing tools.
- **Agents that act on their own:** the workplace studies tested assistants that a person prompts and reviews. I found **no workplace study of autonomous agents in an opt-in pilot**. The "start it read-only" line in the final is our judgement, and should stay labeled that way.
- **Teams, not individuals:** Pennsylvania lists this as an open question: "How do best practices and adoption change when teams, not just individuals, add GenAI to their workflows?" (p. 54).
- **Opt-in vs mandate:** still no head-to-head study (open question in the original brief).

### 2. Stop rule (plain words)
**Shape:** before day one, list the use cases, name a tool and an owner for each, and record a baseline (time and errors on 3 to 5 real tasks per use case, done the usual way). Check at week 2 and at the end date (week 4). Judge **each use case on its own**, not the pilot as a whole. *(Structure, check dates and the 3 to 5 tasks are our judgement. The four-week length is the topic's. GOV.UK says "around 4 to 8 weeks is typical" for a discovery phase, claim 9.)*

| Measure | What we count | Bar, and what happens if it isn't met | Backed by a source, or ours? |
|---|---|---|---|
| **Time on the task** | Clock time on the same kinds of real tasks, before vs during. Not people's estimates. | Not faster than baseline by week 4: drop that use case. | **Sourced as a sensible signal:** Dillon (P1) and Noy and Zhang (P3) measured time directly; METR shows estimates can point the wrong way (p. 10); UK and Pennsylvania figures are self-reported (claim 10; Pennsylvania p. 33). **The bar is ours.** |
| **Errors and rework** | Mistakes found, and outputs sent back to be redone, before vs during. | Higher than baseline: drop that use case, even if it's faster. | **Sourced:** Noy and Zhang scored quality (P3); DBT found worse quality on Excel analysis (claim 11); Brynjolfsson et al. found quality fell for the most experienced workers (in the final). **The bar is ours.** |
| **Review burden** | Minutes the reviewer spends checking or fixing AI output, and how often others flag low-quality AI work. | If review time eats the time saved, drop that use case. | **Partly sourced:** workslop survey ("1hr56m lost per incident," vendor research, Addendum 4); Lee et al. on effort moving to "verifying the accuracy of AI outputs" (P5); Pennsylvania's "did not eliminate, human input" (p. 34). **Using it as a stop signal, and the bar, are ours.** |
| **Use falling off** | Share of opted-in people who used the tool for that use case in the last week. | Most participants stop using it by week 2 and it doesn't recover by week 4: drop that use case. The cut-off is for the team to set (blank). | **Sourced as something pilots track:** UK adoption "83%," then "around 80% was maintained" (claim 10); Pennsylvania participants "predicted that they would use ChatGPT for 6 tasks on average but went on to report half as many use cases," and "At the end of the pilot, 4% of participants reported not using ChatGPT at all" (p. 43). **No source says low use means stop. That's ours.** |
| **Security or data incidents** | Any sensitive data put into a tool against the rules, any tool action outside its allowed scope, any access problem. | Any one: pause that tool the same day and review before restarting. | **Context only:** UK Government AI Playbook, "You know how to use AI securely" (claim 19); Pennsylvania participants were "reluctant to use ChatGPT due to uncertainty about how it processes and stores input data" (p. 48). **The rule is ours.** |

**End-date decision (ours):** at week 4, any use case that meets every bar can be proposed for a longer, wider pilot, with its numbers. Use cases that miss a bar end, and access for them is removed. If none pass, the pilot ends. Write this down before day one. *This replaces "if the pilot does not help, stopping is the result."*

### 3. Earlier brief items that no longer apply to W47
- **Grok Bot fit table and "fits when" text.** Addendum 3's comparison table, the "Fits when" section and its caveats, plus the final's "Where Grok Bot fits" section and four-row table. Drop from W47. Parts may feed W48 only if each capability is re-checked against official docs then.
- **Grok-specific price, plan and billing claims.** Claims 1 to 6, the pricing table, the spend-ceiling template, Addendum 4's footnote suggestions for claims 1 to 6, and final Notes 1 to 3. Drop. Keep a tool-agnostic line instead: "set a spending limit in each tool before day one" (our judgement; no source needed beyond each tool's own settings).
- **Claim 7 (team-membership boundary) and the Grok rollout checklist in claim 19.** Grok-specific; move to W48. Keep claim 19's UK Playbook quotes for W47.
- **"Stopping is the result."** Cut, per Jon. Claim 9's GOV.UK quotes ("It's not a failure to stop…", "around 4 to 8 weeks is typical") can stay as support for deciding the test up front, with the stop rule above.
- **Grok-only lines in the final:** "Grok Bot, launched Nov 11, 2026…" in the evidence section, and the Grok routine sentence in "What to test." Reduce to "Grok Bot is one example; none of these studies tested it," or cut.
- **Still applies:** definitions (Puthal et al.), encouragement figures (Bick et al., Pew), Addendum 4 productivity evidence and counterpoints, the volunteers point (claim 12), and the risk line about agents acting on their own (labeled ours).

### 4. W48 notes (light; not a deep dig)
- **Role teams have research precedent, mostly in software and on test tasks.** MetaGPT: "We define five roles in our software company: Product Manager, Architect, Project Manager, Engineer, and QA Engineer" (Hong et al., 2024, p. 4). It works by encoding "Standardized Operating Procedures (SOPs) into prompt sequences," so that agents can "verify intermediate results and reduce errors" (abstract, p. 1). ChatDev has "software agents" with "various social roles (e.g., requirements analysts, professional programmers and test engineers)" (Qian et al., 2024, p. 3). *Label: both are mostly non-US research teams (MetaGPT led by DeepWisdom; ChatDev at Tsinghua University) and tested on software benchmarks, not workplaces.*
- **No source found for a "scrum master" agent role.** MetaGPT's "Project Manager" is the closest, but don't treat them as the same.
- **Counterpoint, US:** across 7 open-source multi-agent frameworks, UC Berkeley researchers report a "41% to 86.7% failure rate" (Cemri et al., 2025, p. 2). They group failures into "(i) system design issues, (ii) inter-agent misalignment, and (iii) task verification" (abstract). *Label: preprint; benchmark tasks, not workplace use.* It supports W48's need for human approval and clear handoffs.
- **lstack as a worked example:** structure only, no results (claim 20).
- **Not done:** no Grok Bot official-doc capability checks for W48 yet. Every capability claim needs that before drafting.

### APA 7 references (new in this addendum; all checked November 20, 2026)
Becker, J., Rush, N., Barnes, B., & Rein, D. (2025). *Measuring the impact of early-2025 AI on experienced open-source developer productivity* (arXiv:2507.09089). arXiv. https://arxiv.org/abs/2507.09089

Cemri, M., Pan, M. Z., Yang, S., Agrawal, L. A., Chopra, B., Tiwari, R., Keutzer, K., Parameswaran, A., Klein, D., Ramchandran, K., Zaharia, M., Gonzalez, J. E., & Stoica, I. (2025). *Why do multi-agent LLM systems fail?* (arXiv:2503.13657). arXiv. https://arxiv.org/abs/2503.13657

Commonwealth of Pennsylvania. (2025). *Lessons from Pennsylvania's generative AI pilot with ChatGPT*. https://www.pa.gov/content/dam/copapwp-pagov/en/oa/documents/programs/information-technology/documents/openai-pilot-report-2025.pdf

Hong, S., Zhuge, M., Chen, J., Zheng, X., Cheng, Y., Zhang, C., Wang, J., Wang, Z., Yau, S. K. S., Lin, Z., Zhou, L., Ran, C., Xiao, L., Wu, C., & Schmidhuber, J. (2024). MetaGPT: Meta programming for a multi-agent collaborative framework. In *The Twelfth International Conference on Learning Representations*. https://arxiv.org/abs/2308.00352

Qian, C., Liu, W., Liu, H., Chen, N., Dang, Y., Li, J., Yang, C., Chen, W., Su, Y., Cong, X., Xu, J., Li, D., Liu, Z., & Sun, M. (2024). *ChatDev: Communicative agents for software development* (arXiv:2307.07924; accepted to the 2024 Annual Meeting of the Association for Computational Linguistics). arXiv. https://arxiv.org/abs/2307.07924

### Doubts
- Pennsylvania is the only US multi-use-case opt-in pilot report I found, and its time figure is self-reported. The article shouldn't lead with "95 minutes."
- No source backs any specific stop-rule threshold. Every bar above is ours and should read that way in the article.
- The final cites Dillon et al. as forthcoming in *American Economic Review: Insights* with p. 8 for the meetings quote. I checked the Working Paper version only (p. 7).

## Addendum 6 (Nov 20): definition of AI agents

**Why:** Wade's W47 rewrite (commit 5164d34) uses a working definition of "AI agents" labeled as ours. Below are two US government definitions that can be cited. Both are vendor-neutral, both were quoted from the original documents on Fri Nov 20, 2026, and both links open.

### Definition A (best fit): Center for AI Standards and Innovation (CAISI), National Institute of Standards and Technology (NIST)
> "AI agent systems are capable of planning and taking autonomous actions that impact real-world systems or environments. AI agent systems consist of at least one generative AI model and scaffolding software that equips the model with tools to take a range of discretionary actions. These systems may be more expansive, containing multiple sub-agents with software that orchestrates their interactions. They can be deployed with little to no human oversight. Other terms used to refer to AI agent systems include AI agents and agentic AI."

**Location:** *Federal Register*, Vol. 91, No. 5, p. 699, Background section. The notice runs pp. 698 to 701.

**Fit with the article:**
- It names the parts the article means: planning, actions, a model *with tools*, and work that changes things outside the chat.
- It covers several agents working together, which also fits W48.
- It says outright that "AI agents" and "agentic AI" are other names for the same thing.
- The same notice limits its scope to agents "capable of taking actions that affect external state, i.e., persistent changes outside of the AI agent system itself" (p. 700). That line draws the boundary between an agent and a chatbot.
- **Caveat:** this is a request for information, not a finished standard. NIST's AI Agent Standards Initiative (announced February 2026) hasn't published a standard definition yet.

### Definition B (plainest for an executive): US Government Accountability Office (GAO)
> "Agentic artificial intelligence (AI) builds upon the capabilities of generative AI to not just create content, but also to make and adjust plans when the actions required to accomplish a goal are not clearly defined by a user. Unlike generative AI, AI agents can interact with their environment to perform tasks for users. For example, while a customer service generative AI system can respond to order status inquiries, an AI agent could interact with other software systems to process a return or exchange, or other complex customer issues."

**Location:** GAO-25-108519, p. 1, "The Technology: What is it?"

**Same page:** "There is no universally agreed upon definition of an AI agent."

**Fit with the article:**
- The customer-service example is the clearest way to show a non-technical executive the difference between a chatbot that answers and an agent that acts.
- The "no universally agreed upon definition" line is a useful honesty note.
- On p. 2, under Challenges, GAO also supports the article's risk line: "AI agents could misinterpret a user's goal or take unethical actions to achieve a goal... Without sufficient oversight, mistakes or unintended consequences could go undetected."
- **Caveat:** GAO says the spotlight "is not an audit product and is subject to revision" (p. 2).

**Which fits best:** use **A (NIST CAISI)** as the cited definition, because it names tools, multi-step planning and actions that change other systems. Optionally, add **B's customer-service example** to make it concrete.

**Suggested plain-words sentence for Wade (sticks to the sources):**
"An AI agent is software built on a generative AI model that can plan and carry out steps toward a goal, using tools to act in other systems (for example, processing a return rather than only answering a question about it), sometimes with little human oversight (Center for AI Standards and Innovation [CAISI], 2026; U.S. Government Accountability Office [GAO], 2025)."

**Considered, not used:**
- Russell and Norvig's textbook is classic, but its definition is broad: any agent that perceives and acts, including robots and thermostats. I couldn't check a page number at the original.
- The NIST AI Agent Standards Initiative announcement describes agents but doesn't define them.

### Dillon et al. page numbers (note for Edie)
- The final cites p. 8 for "We find no similar shifts in the time workers spent in Teams meetings or working in Word." **That is correct as cited.** It refers to the accepted *American Economic Review: Insights* manuscript (AEA file, https://www.aeaweb.org/content/file?id=24562), where the quote is on p. 8 of the PDF. I checked this today.
- **p. 7 refers to the National Bureau of Economic Research Working Paper 33795 (revised November 2025)**, which is the version Addendum 4 used.
- Use one version consistently with its own page numbers. Don't mix p. 7 and p. 8.

### APA 7 references
Center for AI Standards and Innovation. (2026, January 8). Request for information regarding security considerations for artificial intelligence agents. *Federal Register, 91*(5), 698–701. https://www.federalregister.gov/documents/2026/01/08/2026-00206/request-for-information-regarding-security-considerations-for-artificial-intelligence-agents

U.S. Government Accountability Office. (2025). *Science & tech spotlight: AI agents* (GAO-25-108519). https://www.gao.gov/products/gao-25-108519

Dillon, E. W., Jaffe, S., Immorlica, N., & Stanton, C. T. (in press). Shifting work patterns with generative AI. *American Economic Review: Insights*. https://www.aeaweb.org/articles?id=10.1257/aeri.20250275

**Link check:** the Federal Register page, the govinfo PDF (https://www.govinfo.gov/content/pkg/FR-2026-01-08/pdf/2026-00206.pdf) and both AEA links return 200. The GAO site returns 403 to command-line requests but opens through a web fetch (PDF: https://www.gao.gov/assets/gao-25-108519.pdf), so it works for readers.

## Addendum 7 (Nov 21): AI-source recency (Direction update 6)

**Numbering:** Chet's note called this "Addendum 6," but Addendum 6 (definition of AI agents, commit 5d58c1a) already exists, and the topic file sets no number, so this one is Addendum 7.

**Rule (Jon, Direction update 6 in 01-topic.md, commit 0dbcb47):** every AI-specific claim must cite a source whose data is from the last six months, so after May 20, 2026. Where a source falls inside the window but some of its data is older, say which years the data covers. Definitions and non-AI points are exempt, so Puthal et al. (2025), the Center for AI Standards and Innovation (CAISI, 2026), the U.S. Government Accountability Office (GAO, 2025) and GOV.UK's discovery-phase guide (Government Digital Service [GDS], 2021) all stay.

**Method:** I fetched every new figure at its URL on Sat Nov 21, 2026, and quote it word for word below. FRED and the Gallup pages were read as web pages; NBER and arXiv as their PDFs. All quotes in Direction update 6 matched. Nothing had to be cut as unverifiable.

### Swaps (all verified)
| Section of the article | Out | In (verbatim, with location) | Label and data dates |
|---|---|---|---|
| Opening, and "Encouragement goes with use" | Bick et al. (86% vs 13%; 65 points; "not necessarily causal"); Lin and Parker, Pew Research Center ("half say…") | **Gallup, Indicator: Artificial Intelligence**, https://www.gallup.com/699797/indicator-artificial-intelligence.aspx. Section "Do Managers Support Employee Use of AI?": "As of May 2026, nearly four in 10 employees (36%) in AI-integrating organizations strongly agree that their manager supports their team's use of AI." Employees in AI-adopting organizations who strongly agree that their manager actively supports their team's use of AI are "1.7x as likely to use AI a few times a week or more." Section "Do Most Companies Have a Clear AI Strategy?": "As of August 2026, 26% of U.S. employees say their organization has communicated a clear plan for integrating AI into current practices." | US surveys. Data as of May 2026 (manager support) and August 2026 (clear plan). **The 26% measures a clear plan, not encouragement**, so reword: "Only about a quarter of US employees say their organization has communicated a clear AI plan." The "not necessarily causal" caveat now has to be our own words, because Gallup is also a survey: *"This is a survey link, not proof that manager support causes use (our wording)."* |
| "Real pilots already cover several uses" (task mix) | UK trial "20,000 government employees"; DBT "One thousand licences" | **Kemp (2026), Gallup, "Organizational AI Adoption Jumps Six Points," July 20, 2026**, https://www.gallup.com/workplace/712736/organizational-adoption-jumps-six-points.aspx: "Among AI users, the most common uses of AI are writing and editing (51%), search or research (49%), and general assistance or problem-solving (39%)." | US. Survey dates table on the page: "Q2 2026 May 6-20, 2026," sample "22,573." **Note:** the fieldwork ends on the May 20 cutoff itself. |
| "Results differ by use" (average time saved) | Bick et al., "1.4% time savings" | **FRED Blog, Federal Reserve Bank of St. Louis, "Does generative AI save time at work?" (August 27, 2026)**, https://fred.stlouisfed.org/blog/2026/08/does-generative-ai-save-time-at-work/: "the share of work hours saved thanks to AI assistance grew from 1.6% to 2.2%." The same paragraph gives the span: work use grew "from 28.2% in Q3 2024 to 39.2% by Q2 2026," and hours saved grew "over roughly the same stretch." The post also says: "The information is based on how respondents self-report their 'time saved,' so the measurements are inherently approximate." | US, nationally representative (Real-Time Population Survey). **Self-reported.** Data from Q3 2024 to Q2 2026; only the 2.2% endpoint falls in 2026. Use 2.2% as the latest figure, with that label. |
| "Results differ by use": drafting bullet and the uneven-gains point | Noy and Zhang (2023); Brynjolfsson et al. ("most experienced… small declines in quality") | **Autor et al. (2026), "Does AI Assistance Enhance or Erode Expertise? Evidence from a Three-Month Field Experiment in Patent Drafting," National Bureau of Economic Research Working Paper 35720 (September 2026, revised October 2026)**, https://www.nber.org/papers/w35720. Abstract: "we gave 133 practicing patent lawyers at eleven U.S. intellectual property law firms access to a custom AI patent drafting assistant." On quality while using AI, the abstract says "AI access raised the quality of work delivered on benchmark patent drafting tasks at 10 days (0.34 SD, p = 0.03) and 90 days (0.38 SD, p = 0.01), with larger gains among junior lawyers." On the later task done without AI: "Treated lawyers outperformed controls by 0.32 SD (p = 0.04), but this advantage was concentrated entirely among senior lawyers (0.45 SD, p = 0.02). Junior lawyers showed no average gain." On time, PDF p. 4 (printed p. 2): "Treated lawyers spent about 10 fewer minutes on the 10-day drafting task than controls (p = 0.05), whose mean was 110 minutes." | US randomized trial, not yet peer-reviewed. **Data from May 2025 to February 2026**: "the study period of May 2025 through February 2026" (PDF p. 9, printed p. 7). **Google-linked:** "Funding for the direct costs of this experiment was provided by Google"; "The study was conducted by Google"; five of the seven authors disclose Google employment, and one discloses a paid contractor relationship with Google (NBER page disclosures). **Rewrite the bullet, don't swap a number.** While lawyers had AI, juniors gained *more* in quality. On the later judgment task without AI, only seniors kept an edge. This runs in a different direction from Brynjolfsson et al.'s finding (gains mainly for less experienced workers). |
| "Time the work rather than ask people," and the **new teaser hook** | METR (Becker et al., 2025; data from February to June 2025); UK "26 minutes a day" and the DSIT self-report line | **Yu et al. (2026), "Cognitive offloading and the speedup illusion in human-AI interaction"** (Stanford University; arXiv 2605.23177, May 22, 2026), https://arxiv.org/abs/2605.23177. Abstract: "We conducted a preregistered large-scale behavioral study (N = 1237)… While actual completion times between independent completion and AI-assisted completion did not differ, participants predicted AI to be significantly faster." Also in the abstract: "participants reported lower subjective effort with AI despite equivalent completion times." | Preprint; the arXiv comment lists the Proceedings of the 48th Annual Meeting of the Cognitive Science Society. Simple lab tasks ("simple cognitive tasks," abstract), not real jobs. Participants were recruited through Prolific, "comprising a representative sample of the US adult population" (Methods). The AI was GPT-4o. **The paper doesn't state when its data were collected**, so say "published May 2026; collection dates not stated." |
| "What the evidence does not show": trust and checking | Lee et al. (2025); workslop (BetterUp Labs and Stanford Social Media Lab) | **Ma et al. (2026), "Impact of Expertise and Trust on AI-assisted Work"** (Carnegie Mellon University and Microsoft; arXiv 2610.14660, October 10, 2026), https://arxiv.org/abs/2610.14660. Abstract: "participants who delegated more completed more of the task, but were also more likely to produce invalid solutions. Experts more often resisted this tradeoff, sacrificing completion to decompose the task and scrutinize agent outputs." | Preprint. Think-aloud study of "20 professionals" recruited "at a large technology company." The tool was an agent (GitHub Copilot agent mode). Four of the seven authors are at Microsoft. **Collection dates not stated.** **Author-name mismatch:** the arXiv listing reads "Pranav Khape," "Rock Pang" and "Siddarth Suri"; the PDF reads Pranav Khadpe, Rock Yuren Pang and Siddharth Suri. The APA entry below follows the PDF. |
| Agents gap, and the Takeaway | "We found no workplace study of agents that act on their own in an opt-in pilot" | **Wang et al. (2026), "Agentic AI and Human-in-the-Loop Interventions: Field Experimental Evidence from Alibaba's Customer Service Operations"** (arXiv 2605.14830; v1 May 14, 2026, v2 June 1, 2026), https://arxiv.org/abs/2605.14830. Abstract: "Workers in the treatment condition supervised an agentic AI system that resolved AI-eligible chats… The findings show that AI deployment reduces average chat duration and has limited effects on retrial rates, but substantially lowers ratings for AI-eligible chats." | Not US: Taobao, China. Preprint. **Data from August 2024**: "a randomized field experiment conducted on Alibaba's ecommerce platform, Taobao.com, in August 2024, involving 647 customer service workers and 680,676 service chats" (Introduction). **The data predate the window, so the label must say so.** One author is at Alibaba Group, the platform studied. **New gap wording:** "We found one randomized field trial of agents acting on their own at work, outside the US and in customer service only (Wang et al., 2026, data from 2024). We found none of an opt-in pilot, and none that ran several tools." |

### Cuts (per Direction update 6)
- **UK trial numbers.** GDS (2025b): 20,000 employees, "26 minutes a day," "83%" and "around 80%." Also the Department for Science, Innovation and Technology (DSIT) press release, and the UK adoption line in the stop-rule section. Brief claims 8 and 10.
- **Department for Business and Trade (DBT) pilot,** including the Excel finding and the ~70% volunteer line. Brief claims 8, 11 and 12, and the DBT parts of claim 15. The volunteers point now rests on Pennsylvania alone: "Pilot participants were not a representative sample of Commonwealth employees" (p. 12).
- **Escalations** (Brynjolfsson et al.), and with them the "most experienced workers" quote.
- **Humlum and Vestergaard** (Denmark): claims 13, 14, 17 and 18.
- **Bick et al.'s 6-point gender gap.** All Bick et al. figures are out of the article (claim 13a), and Lin and Parker of Pew are out too (claim 13b).
- **Workslop** (BetterUp Labs and Stanford Social Media Lab): the 40% and "1hr56m" figures, and the bullet.
- **UK AI Playbook** (GDS, 2025a), claim 19. "Start each agent read-only, with a named reviewer and an off-limits list" stays, labeled as our judgement.
- **Also out under the same rule** (AI-specific, with data before May 20, 2026; not in the current final, but don't reuse them):
  - Microsoft and LinkedIn (2024) and Gallup (June 2025) in claim 13.
  - The Gallup lines in claims 15 and 16 (work-nearly-doubled article, 2025).
  - Claim 13c (Brookings conference draft, worker survey Jan to Feb 2026).
  - Noy and Zhang (2023), METR (Becker et al., 2025) and Lee et al. (2025).
  - Addendum 4's Bick 1.4%.
  - Addendum 5's MetaGPT, ChatDev and Cemri et al., which are W48 notes. They would need the same recency check before W48 uses them.

### Keep, with "data from" labels
- **Dillon et al. (in press, *American Economic Review: Insights*):** "Between September 2023 and October 2024, Microsoft partnered with 66 large firms to run a cross-industry field experiment" (National Bureau of Economic Research Working Paper 33795, p. 1). Label: **data from 2023 to 2024**.
- **Commonwealth of Pennsylvania (2025):** five cohorts ran "from March 2024 – March 2025" (p. 10). Label: **data from 2024 to 2025**. Its volunteer, self-report and teams quotes stay. It's still the only US opt-in pilot evaluation we have.
- **Olson et al. (2025):** the study ran in 2024 (checked in Addendum 4: February to October 2024). Label: **data from 2024**. I found no verifiable replacement from inside the window, so I'm keeping it with the label, per Jon.

### Knock-on fixes (suggested wording for Wade; his call)
- **Teaser (new hook; 270/280 with ARTICLE_URL counted as 23):** "In a preregistered study of 1,237 US adults, people predicted AI would make simple tasks faster. Completion times did not differ (Yu et al., 2026, preprint). So time the work by the clock. A case for a capped, four-week opt-in pilot of AI agents: ARTICLE_URL"
  - The "US adults" wording rests on the Methods line: "comprising a representative sample of the US adult population."
- **End of "Three terms":** replace the Bick and Pew sentence with: "The Gallup surveys cited below measure manager support and whether a clear AI plan has been communicated. Neither is the same as sanction, and neither measures hidden use (Gallup, n.d.)."
- **Takeaway:** replace "none of it from tests of agents acting on their own" with: "and only one randomized field trial of agents acting on their own, in customer service outside the US, with data from 2024 (Wang et al., 2026)."
- **Stop-rule Sources line:** "Sources: the measures draw on Dillon et al. (in press), Autor et al. (2026), Yu et al. (2026), Ma et al. (2026), Wang et al. (2026), the Federal Reserve Bank of St. Louis (2026) and the Commonwealth of Pennsylvania (2025); see References. Every bar and the stop rule are ours; no source sets a threshold."
  - How the remaining sources map to the measures:
    - Time by the clock: Dillon, Autor and Yu.
    - Errors and rework: Autor (blinded expert scoring) and Ma ("invalid solutions").
    - Checking: Ma, and Pennsylvania p. 34.
    - Use falling off: Pennsylvania p. 43. The UK adoption line is cut.
    - Security: Pennsylvania p. 48.
    - Customer ratings: Wang, as an outcome to watch in customer-facing uses.
- **Stop-rule "Pilots do track use" paragraph:** delete the UK sentence and keep the two Pennsylvania quotes, labeled data from 2024 to 2025.
- **Design section:** delete the DBT volunteer quote, the gender-gap sentence and the Playbook quotes. Keep the Pennsylvania "not a representative sample" quote and the read-only, reviewer and off-limits advice (ours).
- **References:**
  - **Remove:**
    - Becker et al. (2025)
    - BetterUp Labs and Stanford Social Media Lab (2025)
    - Bick et al. (2025)
    - Brynjolfsson et al. (2025)
    - Department for Business and Trade (2025)
    - Department for Science, Innovation and Technology (2025)
    - Government Digital Service (2025a) and (2025b). Keep GDS (2021), and drop its "2021" disambiguation letters if any remain.
    - Humlum and Vestergaard (2026)
    - Lee et al. (2025)
    - Lin and Parker (2025)
    - Noy and Zhang (2023)
  - **Keep:**
    - Center for AI Standards and Innovation (2026)
    - Commonwealth of Pennsylvania (2025)
    - Dillon et al. (in press)
    - Government Digital Service (2021)
    - Olson et al. (2025)
    - Puthal et al. (2025)
    - U.S. Government Accountability Office (2025)
  - **Add:** the seven entries below.

### Counterpoints (still at least two after the cuts)
- **Self-reports mislead.** People predicted AI would be faster when it wasn't (Yu et al.), and the FRED time-saved series is self-reported.
- **Doing more can mean getting it wrong.** Heavier delegation produced more invalid work (Ma et al.).
- **Speed can cost quality.** Agents shortened chats but "substantially lowers ratings" (Wang et al.).
- **Help is uneven and can fade without AI.** Junior lawyers kept no edge on the later task done without AI (Autor et al.).
- **Saved time may not show up in output.** Dillon et al. "do not detect shifts in the quantity or composition of workers' tasks" (abstract; data from 2023 to 2024).

### Open questions
- The recency rule leaves almost no **US** field evidence with data inside the window. Autor et al. ends in February 2026, and the Gallup task mix was fielded May 6 to 20, 2026, ending on the cutoff. Should the article say plainly that AI field evidence lags by a year or more?
- Yu et al. and Ma et al. don't say when they collected their data. Is "published inside the window" enough under Jon's rule, or should each carry "collection dates not stated"? I recommend the label.
- Wang et al. is the only agent field trial, and its data is from August 2024. Jon named it, so it stays, labeled. Confirm he's comfortable with a 2024 data label on the article's only agent trial.

### APA 7 references (new; all checked November 21, 2026)
Autor, D., Rodchenko, T., Martin, J., Iscenko, Z., Strand, S., Pearl, D., & Ferere, M. (2026). *Does AI assistance enhance or erode expertise? Evidence from a three-month field experiment in patent drafting* (Working Paper No. 35720). National Bureau of Economic Research. https://www.nber.org/papers/w35720

Federal Reserve Bank of St. Louis. (2026, August 27). Does generative AI save time at work? *FRED Blog*. https://fred.stlouisfed.org/blog/2026/08/does-generative-ai-save-time-at-work/

Gallup. (n.d.). *Indicator: Artificial intelligence*. Retrieved November 21, 2026, from https://www.gallup.com/699797/indicator-artificial-intelligence.aspx

Kemp, A. (2026, July 20). *Organizational AI adoption jumps six points*. Gallup. https://www.gallup.com/workplace/712736/organizational-adoption-jumps-six-points.aspx

Ma, Q., Khadpe, P., Pang, R. Y., Koedinger, K., Wu, T., Suri, S., & Iqbal, S. (2026). *Impact of expertise and trust on AI-assisted work* (arXiv:2610.14660). arXiv. https://doi.org/10.48550/arXiv.2610.14660

Wang, Y., Zhu, C., Feng, T., Lu, L. X., & Jia, B. (2026). *Agentic AI and human-in-the-loop interventions: Field experimental evidence from Alibaba's customer service operations* (arXiv:2605.14830; Version 2). arXiv. https://doi.org/10.48550/arXiv.2605.14830

Yu, S., Cheng, M., Jabbar, A., Sucholutsky, I., Collins, K. M., Jurafsky, D., & Hawkins, R. D. (2026). *Cognitive offloading and the speedup illusion in human-AI interaction* (arXiv:2605.23177). arXiv. https://doi.org/10.48550/arXiv.2605.23177

**Link check (Nov 21):**
- Return 200: both Gallup pages; the NBER page and PDF for w35720; all three arXiv abstract pages and their DOIs; and the Dillon, Pennsylvania and Olson links.
- The FRED Blog dropped the connection on a command-line request but opened in a web fetch.
- The NBER DOI (https://doi.org/10.3386/w35720) returned a 500 error today, so the reference uses the NBER page URL instead.

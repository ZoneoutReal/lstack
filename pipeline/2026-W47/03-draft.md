# Don't wait for the company rollout: sanction a capped, four-week opt-in pilot of AI agents

Whether an employee uses generative AI at work can look like a personal choice, yet it appears to track whether the employer says yes. In a Federal Reserve Bank of St. Louis working paper, Bick et al. (2025) report from a nationally representative US survey that "86% of respondents whose employer encourages genAI use report adopting it, compared to just 13% among those whose employer does not" (p. 16). Yet in a survey fielded in late 2024, Lin and Parker (2025) of the Pew Research Center found that "half say their employer neither encourages nor discourages the use of AI chatbots at work," while 12% say their employer encourages it (p. 23).

If silence is the norm, and encouragement goes with far more use, what can a cautious leader do while the company-wide rollout is still being planned? The purpose of this article is to make the case for sanctioning a capped, four-week opt-in pilot of AI agents across several uses. Secondly, it shows that results differ by use, why tasks should be timed rather than estimated, what the evidence does not yet cover, and how to write a stop rule in plain words before day one.

## Three terms
Writing in *SN Computer Science*, Puthal et al. (2025) define shadow AI as the "deployment and usage of AI tools, models, or systems by employees of an organization without explicit endorsement, supervision, or management by IT and cyber security departments" (Introduction, para. 1). Here, sanctioned use means AI use the organization has explicitly endorsed and supervises (our wording, built by contrast with Puthal et al., 2025). By AI agents we mean AI tools that do work on a person's behalf, from drafting a reply to taking steps in other apps; this working definition is also ours. The US surveys measure encouragement, which is not the same as sanction, and neither measures hidden use (Bick et al., 2025; Lin & Parker, 2025).

## Encouragement goes with use
Employer encouragement is the strongest predictor in one large US survey: "a worker is 65 percentage points more likely to use genAI for work if their employer encourages them to do so" (Bick et al., 2025, p. 17). The authors "caution that the estimated effect of employer encouragement is not necessarily causal" (p. 17), and no study we found compares opt-in with mandated rollouts. A sanctioned opt-in may therefore serve a team more than waiting does, if the exec sanctions it out loud.

## Real pilots already cover several uses
A pilot need not bet on one task. In a randomized trial across 66 firms, Dillon et al. (in press) gave workers a tool "integrated into applications they already used at work for email, meetings, and writing" (abstract). The UK government ran a Microsoft 365 Copilot trial "involving 20,000 government employees," and the UK Department for Business and Trade (DBT) ran "One thousand licences ... for a 3-month pilot" (DBT, 2025; Government Digital Service [GDS], 2025b).

The closest US example is the Commonwealth of Pennsylvania (2025), where "The Commonwealth equipped 175 employees to use ChatGPT Enterprise" (p. 8) from "14 state government agencies" (p. 9), and "These employees volunteered to explore this new technology" (p. 2). Their uses were spread out: "Writing assistance, text generation, drafting emails 36%," "Research, idea exploration, learning new topics 27%" and "Summarizing 13%" (p. 16). "Users estimated saving 95 minutes per day with ChatGPT" (p. 3), but that figure rests on "Estimates reported by participants in exit survey" (p. 33), and "ChatGPT reduced, but did not eliminate, human input into final work products" (p. 34). *Label: US state government; one tool; self-reported time; "OpenAI led trainings" (p. 11).*

## Results differ by use
The more carefully measured studies suggest that AI helps most on well-defined writing and communication tasks, and most for less experienced workers. Each tested one tool, such as Microsoft 365 Copilot or ChatGPT. Grok Bot is one more example of the tools a pilot could include, and none of these studies tested it.

- **Email fell; meetings did not.** Dillon et al. (in press) found that "In the second half of the 6-month experiment, the 80% of treated workers who used the tool spent two fewer hours on email each week" (abstract), yet "We find no similar shifts in the time workers spent in Teams meetings" (p. 8). *Label: peer-reviewed, forthcoming in American Economic Review: Insights; mostly Microsoft Research authors, testing Microsoft 365 Copilot.*
- **Drafting got faster.** In a randomized experiment published in *Science*, Noy and Zhang (2023) found that "The average time taken decreased by 40% and output quality rose by 18%" (p. 187). *Label: peer-reviewed; short test tasks, not real jobs.*
- **Escalations fell.** In customer support, Brynjolfsson et al. (2025) found "an almost 25% decline in customer requests to speak to a manager," from a baseline of about 6% of chats (p. 933). *Label: one US software firm; most agents outside the US, mainly in the Philippines.*
- **Note-taking strain eased.** Writing in *JAMA Network Open*, Olson et al. (2025) report that after 30 days with an AI note-taker, "burnout among those working in ambulatory clinics decreased significantly from 51.9% to 38.8%" (Key Points). *Label: clinicians' visit notes, not office meetings; volunteers, before-and-after survey; "There was no control group"; authors tied to the vendor.*
- **Spreadsheet work got worse.** DBT found that "Small time savings were observed across most use cases," but users "completed Excel data analysis more slowly and to a worse quality and accuracy than non-users" (DBT, 2025). *Label: not US.*

Across US workers, average gains are modest: Bick et al. (2025) estimate "1.4% time savings across all workers (including non-users)" (p. 2). *Label: self-reported.* For this reason, a pilot should judge each use on its own, not the pilot as a whole.

## Time the work rather than ask people
Self-reported speed-ups can point the wrong way. In a randomized trial with 16 experienced open-source developers run by Model Evaluation & Threat Research (METR), Becker et al. (2025) report: "developers estimate that allowing AI reduced completion time by 20%. Surprisingly, we find that allowing AI actually increases completion time by 19%" (abstract, p. 1). The authors "show that both experts and developers drastically overestimate the usefulness of AI on developer productivity" (p. 10), and they "caution readers against overgeneralizing on the basis of our results" (p. 12). *Label: preprint, not peer-reviewed; small sample; expert coders on code they knew well.* The UK trial likewise reported that "Trial participants saved an average of 26 minutes a day" (GDS, 2025b), yet the Department for Science, Innovation and Technology (2025) notes that "Figures are derived from self-reported daily time savings." A pilot should therefore time real tasks by the clock.

## What the evidence does not show, and where it is thin
- **AI output can create review work.** BetterUp Labs and Stanford Social Media Lab (2025) define workslop as AI-generated work content that "masquerades as good work" and found that "40% of desk workers received workslop in the last month," with "1hr56m lost per incident" (p. 1). *Label: vendor research; BetterUp sells coaching.*
- **Saved time may not show up in output or pay.** Dillon et al. (in press) "do not detect shifts in the quantity or composition of workers' tasks" (abstract), and in Denmark, Humlum and Vestergaard (2026) "estimate precise null effects on earnings and recorded hours" (abstract). *Label: not US.*
- **Gains are uneven.** Brynjolfsson et al. (2025) found that "the most experienced and highest-skilled workers see small gains in speed and small declines in quality" (p. 889).
- **Trusting AI more can mean checking less.** Lee et al. (2025) found that "higher confidence in GenAI is associated with less critical thinking" (abstract). *Label: self-reported; mostly non-US; Microsoft Research authors.*

Some gaps should be said plainly. We found no study of a pilot that ran several AI tools side by side, and none that compares tools. We found no workplace study of agents that act on their own in an opt-in pilot; the studies above tested assistants that a person prompts or reviews. Pennsylvania lists teams as an open question: "How do best practices and adoption change when teams, not just individuals, add GenAI to their workflows?" (Commonwealth of Pennsylvania, 2025, p. 54). The case for a pilot rests on these gaps as much as on the gains: a short, measured test is how a team finds out.

## Design the pilot
Before day one, list the use cases, name a tool and an owner for each, and record a baseline: time and errors on 3 to 5 real tasks per use case, done the usual way. This structure is our judgement. Set a spending limit in each tool before day one, which is also our judgement.

Volunteers are not a random sample. DBT let colleagues "volunteer for a licence, until around ~70% of licences had been allocated," then assigned the rest at random (DBT, 2025), and in Pennsylvania, "Pilot participants were not a representative sample of Commonwealth employees" (Commonwealth of Pennsylvania, 2025, p. 12). In current US work use, "genAI adoption is 6 percentage points higher for men," a raw gap before other factors are accounted for (Bick et al., 2025, p. 10). We suggest mostly volunteers, plus a few who did not volunteer.

A central rollout has real strengths, so the pilot should clear review first. The UK Government AI Playbook asks that "You know how to use AI securely" and "You work with commercial colleagues from the start," and that "humans validate any high-risk decisions influenced by AI" (GDS, 2025a). An agent that acts on its own can also act wrongly, so we suggest starting each one read-only, with a named reviewer and an off-limits list in writing.

## The stop rule, in plain words
Deciding the test up front makes stopping a normal outcome. The GOV.UK Service Manual advises that "It's not a failure to stop at the end of the discovery phase if your research shows that's the best thing to do," and notes that, for the discovery phase of a new service, "around 4 to 8 weeks is typical" (GDS, 2021). We suggest judging each use case on five measures, against the baseline, at week 2 and again at week 4.

| Measure | What to count | Bar (ours) |
|---|---|---|
| **Time by the clock** | Clock time on the same real tasks | Not faster by week 4: drop the use |
| **Errors and rework** | Mistakes found; work sent back | Higher than baseline: drop, even if faster |
| **Minutes checking AI output** | Reviewer time spent checking or fixing | Checking eats the time saved: drop |
| **Use falling off** | Share who used it last week | Most stop by week 2, no recovery by week 4: drop; team sets the cut-off |
| **Security incidents** | Sensitive data shared, actions out of scope, access problems | Any one: pause that tool the same day and review |

Sources: the measures draw on Dillon et al. (in press), Noy and Zhang (2023), Becker et al. (2025), DBT (2025), BetterUp Labs and Stanford Social Media Lab (2025), Lee et al. (2025), GDS (2025a, 2025b) and Commonwealth of Pennsylvania (2025); see References. Every bar and the stop rule are ours; no source sets a threshold.

Pilots do track use over time. The UK trial reported adoption of "83%," then "around 80% was maintained" (GDS, 2025b), while Pennsylvania participants "predicted that they would use ChatGPT for 6 tasks on average but went on to report half as many use cases" (Commonwealth of Pennsylvania, 2025, p. 43). Some also held back over data, being "reluctant to use ChatGPT due to uncertainty about how it processes and stores input data" (p. 48).

At week 4, we suggest that any use case meeting every bar be proposed for a longer, wider pilot, with its numbers. Use cases that miss a bar end, and access for them is removed. If none pass, the pilot ends. Write this down before day one.

## Takeaway
Leaders should be obligated to decide, not to stay silent. Encouragement goes with far more use, and the evidence suggests real but uneven help that differs by task, none of it from tests of agents acting on their own. A cautious exec can sanction one capped, four-week opt-in pilot and ask for five things:

1. Sanction, said out loud.
2. A short list of use cases, each with a tool, an owner and a baseline.
3. A spending limit in each tool.
4. A named reviewer, an off-limits list and read-only access first.
5. The five-measure stop rule, checked at week 2 and week 4, agreed before day one.

## References
Becker, J., Rush, N., Barnes, B., & Rein, D. (2025). *Measuring the impact of early-2025 AI on experienced open-source developer productivity* (arXiv:2507.09089). arXiv. https://arxiv.org/abs/2507.09089

BetterUp Labs & Stanford Social Media Lab. (2025). *The hidden cost of workslop: What the numbers mean for your organization* [Research summary]. BetterUp. https://www.betterup.com/hubfs/Post-Uplift%20content/BetterUp_Uplift_The%20hidden%20cost%20of%20workslop.pdf

Bick, A., Blandin, A., & Deming, D. J. (2025). *The rapid adoption of generative AI* (Working Paper No. 2024-027F). Federal Reserve Bank of St. Louis. https://doi.org/10.20955/wp.2024.027

Brynjolfsson, E., Li, D., & Raymond, L. (2025). Generative AI at work. *The Quarterly Journal of Economics, 140*(2), 889–942. https://doi.org/10.1093/qje/qjae044

Commonwealth of Pennsylvania. (2025). *Lessons from Pennsylvania's generative AI pilot with ChatGPT*. https://www.pa.gov/content/dam/copapwp-pagov/en/oa/documents/programs/information-technology/documents/openai-pilot-report-2025.pdf

Department for Business and Trade. (2025). *The evaluation of the M365 Copilot pilot in the Department for Business and Trade*. GOV.UK. https://assets.publishing.service.gov.uk/media/68adbe409e1cebdd2c96a19d/dbt-microsoft-365-copilot-evaluation.pdf

Department for Science, Innovation and Technology. (2025, June 2). *Landmark government trial shows AI could save civil servants nearly 2 weeks a year* [Press release]. GOV.UK. https://www.gov.uk/government/news/landmark-government-trial-shows-ai-could-save-civil-servants-nearly-2-weeks-a-year

Dillon, E. W., Jaffe, S., Immorlica, N., & Stanton, C. T. (in press). Shifting work patterns with generative AI. *American Economic Review: Insights*. https://www.aeaweb.org/articles?id=10.1257/aeri.20250275

Government Digital Service. (2021). *How the discovery phase works*. GOV.UK Service Manual. https://www.gov.uk/service-manual/agile-delivery/how-the-discovery-phase-works

Government Digital Service. (2025a, February 10). *Artificial intelligence playbook for the UK government*. GOV.UK. https://www.gov.uk/government/publications/ai-playbook-for-the-uk-government/artificial-intelligence-playbook-for-the-uk-government-html

Government Digital Service. (2025b, June 2). *Microsoft 365 Copilot experiment: Cross-government findings report*. GOV.UK. https://www.gov.uk/government/publications/microsoft-365-copilot-experiment-cross-government-findings-report/microsoft-365-copilot-experiment-cross-government-findings-report-html

Humlum, A., & Vestergaard, E. (2026). *Still waters, rapid currents: Early labor market transformation under generative AI* (Working Paper No. 33777). National Bureau of Economic Research. https://www.nber.org/system/files/working_papers/w33777/w33777.pdf

Lee, H.-P., Sarkar, A., Tankelevitch, L., Drosos, I., Rintel, S., Banks, R., & Wilson, N. (2025). The impact of generative AI on critical thinking: Self-reported reductions in cognitive effort and confidence effects from a survey of knowledge workers. In *Proceedings of the 2025 CHI Conference on Human Factors in Computing Systems* (pp. 1–22). Association for Computing Machinery. https://doi.org/10.1145/3706598.3713778

Lin, L., & Parker, K. (2025). *U.S. workers are more worried than hopeful about future AI use in the workplace* [Report]. Pew Research Center. https://www.pewresearch.org/wp-content/uploads/sites/20/2025/02/ST_2025.2.25_AI-Workers_REPORT.pdf

Noy, S., & Zhang, W. (2023). Experimental evidence on the productivity effects of generative artificial intelligence. *Science, 381*(6654), 187–192. https://doi.org/10.1126/science.adh2586

Olson, K. D., Meeker, D., Troup, M., Barker, T. D., Nguyen, V. H., Manders, J. B., Stults, C. D., Jones, V. G., Shah, S. D., Shah, T., & Schwamm, L. H. (2025). Use of ambient AI scribes to reduce administrative burden and professional burnout. *JAMA Network Open, 8*(10), Article e2534976. https://doi.org/10.1001/jamanetworkopen.2025.34976

Puthal, D., Mishra, A. K., Mohanty, S. P., Longo, A., & Yeun, C. Y. (2025). Shadow AI: Cyber security implications, opportunities and challenges in the unseen frontier. *SN Computer Science, 6*(5), Article 405. https://doi.org/10.1007/s42979-025-03962-x

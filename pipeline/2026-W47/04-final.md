# Don't wait for the company rollout: run a capped, four-week opt-in

Whether an employee uses generative AI at work can look like a personal choice. It appears to track closely whether the employer says yes. In a Federal Reserve Bank of St. Louis working paper, Bick, Blandin and Deming (2025) report from a nationally representative US survey that "86% of respondents whose employer encourages genAI use report adopting it, compared to just 13% among those whose employer does not" (p. 16). Yet many employers have taken no side. Lin and Parker (2025) of the Pew Research Center found that "half say their employer neither encourages nor discourages the use of AI chatbots at work," while 12% say their employer encourages it (p. 23).

If silence is the norm, and encouragement goes with far more use, what can a cautious leader do while the company-wide rollout is still being planned? The purpose of this article is to propose a sanctioned, capped, four-week opt-in for Grok team bots. Secondly, it answers the "not worth the cost" objection with official list prices, a spend cap built from settings the product actually has, a stop rule written before day one, an honest way to weigh cost against time saved, and a fair way to choose who joins. The following sections define two terms, make the case, show where Grok Bot fits next to tools a company may already have, and then lay out the plan.

## Two terms: shadow AI and sanctioned use
Writing in *SN Computer Science*, Puthal, Mishra, Mohanty, Longo and Yeun (2025) define shadow AI as the "deployment and usage of AI tools, models, or systems by employees of an organization without explicit endorsement, supervision, or management by IT and cyber security departments" (Introduction, para. 1). No source we found defines sanctioned use on its own. In this article, sanctioned use means AI use the organization has explicitly endorsed and supervises; the wording is ours, built by contrast with Puthal et al. (2025). Both terms describe permission and oversight, not how much people use a tool.

One caution follows. The US survey data measure encouragement, which is not the same as sanction (Bick et al., 2025; Lin & Parker, 2025). An employer can allow a tool without encouraging it, and neither study measures use the employer has forbidden or does not know about. We therefore do not claim that the 13% are shadow AI users. We can suggest only that, without a clear signal from leadership, use is low and left to chance.

## Silence is the default, and encouragement is the lever
Employer encouragement is the strongest pattern in the US evidence. Bick et al. (2025) also found that "a worker is 65 percentage points more likely to use genAI for work if their employer encourages them to do so" (p. 17). In a later Brookings Papers on Economic Activity conference draft, Bick, Blandin, Deming, Fuchs-Schündeln and Jessen (2026) found that the US had the lowest share of workers receiving none of three supports (encouragement, training and tools), yet that share was still 44%, against 69% in France and 70% in Italy (p. 28). Writing for Gallup, Pendell (2025) found that 40% of US workers had used AI at work a few times a year or more, while "only 22% say their organization has communicated a clear plan or strategy." It seems that many organizations are leaving this lever unused.

The evidence has limits. The authors "caution that the estimated effect of employer encouragement is not necessarily causal" (Bick et al., 2025, p. 17). Their 86% and 13% come from 2024 survey waves, and US use has risen since: Kemp (2026), also writing for Gallup, reports that 52% of US workers now use AI in their role. No newer public split by encouragement was found. Nor does any study we found compare opt-in with mandated rollouts head to head. The case here is therefore narrow: a sanctioned, encouraged, bounded opt-in may serve a team more than waiting does. The evidence does not show that it outperforms a mandate.

Clear direction from the top appears to help as well. When employees strongly agree that leadership has communicated a clear plan for AI, Pendell (2025) reports that they are "three times as likely to feel very prepared to work with AI and 2.6 times as likely to feel comfortable using AI in their role." Peers and managers may matter too. In a pilot run by the UK Department for Business and Trade (DBT), "Users were also anecdotally less likely to use M365 Copilot if their colleagues and line managers were hesitant about its use" (DBT, 2025). For this reason, the pilot should not go around leadership. The strongest version asks the exec to sanction it and say so out loud.

## Where Grok Bot fits next to the AI tools a company may already have
A cautious exec may reasonably ask why a team would pilot Grok Bot instead of a tool the company already licenses. The official product pages suggest that the overlap is large. Each of the main workplace AI tools now offers some form of shared agents, scheduled work, connectors and browser automation (Google, n.d.-d; Microsoft, n.d.-c; OpenAI, 2026d; SpaceX Super Intelligence, 2026f). The differences appear to lie mostly in where each tool lives (e.g., Slack, Microsoft Teams or Google Workspace), which meetings it joins, and how it is bought and governed. We therefore frame this section as fit and differences, not as a ranking.

The comparison below draws only on official pages from SpaceX Super Intelligence (the publisher of Grok Bot), OpenAI, Microsoft and Google, as read on Nov 20, 2026. We treat Codex and ChatGPT as one option, since OpenAI now includes Codex in ChatGPT plans; a ChatGPT Business Standard seat includes "access to ChatGPT, ChatGPT Work, and Codex" (OpenAI, 2026a). The appendix covers further rows. These products change often, so re-check every cell before a decision.

| | Grok Bot | ChatGPT Business or Enterprise (includes Codex) | Microsoft 365 Copilot | Gemini for Google Workspace |
|---|---|---|---|---|
| **Shared agents** | Team Bots: "share a Grok Bot with your team ... They can use it in Grok Bot, Slack, Microsoft Teams, or even your calls" (SpaceX Super Intelligence, 2026h) | Workspace agents: "share it with teammates or your workspace, use it in Slack, run it on a schedule, or trigger it through an API" (OpenAI, 2026d) | "Agent creation using Agent Builder and Copilot Studio"; pre-built "Researcher, Analyst, and Facilitator" agents (Microsoft, n.d.-c) | Gems, "customizable versions of Gemini"; "you can share Gems with other users in your organization and beyond" (Google Workspace, 2025) |
| **Scheduled or triggered work** | Routines run "on a schedule, or when something happens, such as a Slack message, a GitHub, Linear, Sentry, or PagerDuty event, an email, or a webhook call" (SpaceX Super Intelligence, 2026f) | Enterprise team tasks "run on a schedule or supported trigger, using approved company tools" (OpenAI, 2026b); Codex scheduled tasks in the ChatGPT desktop app (OpenAI, n.d.-d) | Scheduled prompts "across Microsoft Teams, Office.com chat, and Microsoft Outlook," with "up to 10 active and 50 total schedules per user" (Microsoft, 2026b) | "Up to 10 active schedules at a time" (Google, n.d.-d); in Workspace Studio, "You can choose an event, schedule, or create a trigger manually" (Google, n.d.-c) |
| **Meetings** | Joins "Google Meet, Zoom, or Microsoft Teams calls," "listens, takes notes, answers questions in the meeting chat"; on Team, Enterprise, Ultra and Super plans (SpaceX Super Intelligence, 2026a) | Record transcribes meetings in the macOS desktop app; calendar auto-join "supports Google Meet links only," and Zoom and Teams need a manual start (OpenAI, 2026c) | Facilitator in Teams meetings "Answers open-ended questions in the meeting chat"; it "can only be added to scheduled meetings" (Microsoft, n.d.-a) | Meet note-taking, where "a Google Doc with the notes is emailed to the organizer"; Business Standard and up (Google, 2026) |
| **Public list price (US)** | Team seats at $30 (Premium), $100 (Super) or $200 (Ultra) per seat per month; Enterprise through sales (SpaceX Super Intelligence, n.d., 2026e) | Business Standard seats at $20 per user per month billed annually, or "$25 per user per month when billed monthly"; Enterprise "Contact sales" (OpenAI, n.d.-c, 2026a) | Enterprise add-on "$30.00 user/month, paid yearly," which also requires "a qualifying Microsoft 365 plan" (Microsoft, n.d.-c) | Business Starter $7, Standard $14 and Plus $22 per user per month, each listing a "Gemini AI assistant"; Enterprise "Contact sales" (Google, n.d.-a) |

Where each option fits, from documented capabilities only and with no claim about performance:

- **Grok Bot fits when** a team wants one shared assistant that works in Slack and Microsoft Teams and joins Meet, Zoom and Teams calls (SpaceX Super Intelligence, 2026a, 2026h). It also fits when work should run on triggers from tools such as GitHub, Linear or PagerDuty, or on the bot's own persistent computer for browser tasks (SpaceX Super Intelligence, 2026f, 2026k).
- **ChatGPT Business or Enterprise fits when** a company wants a broad ChatGPT workspace with shared agents, team tasks and the Codex coding agent under one admin console (OpenAI, 2026a, 2026b, 2026d).
- **Microsoft 365 Copilot fits when** the company already runs on Microsoft 365 and Teams and wants AI inside Outlook, Word and Teams meetings, or agents built in Copilot Studio (Microsoft, n.d.-a, n.d.-c, 2026c).
- **Gemini for Google Workspace fits when** the company runs on Gmail, Docs and Meet and wants AI included in the Workspace subscription, with Meet note-taking and shared Gems (Google, n.d.-a, 2026; Google Workspace, 2025).

Gemini is included in Workspace plans (Google, n.d.-a). Microsoft 365 Copilot is an add-on to an existing Microsoft 365 plan (Microsoft, n.d.-c), and a Grok Bot pilot is a separate line item (SpaceX Super Intelligence, 2026e). If the company already pays for Microsoft 365 Copilot or a Workspace edition with Gemini, we suggest the first question is what that tool does not cover for this team. The pilot then tests that difference (e.g., joining Meet, Zoom and Teams calls). It is not a replacement decision.

## What it costs, in official list prices
These are US list prices as of Nov 20, 2026, before tax. The pricing page says "Prices subject to change," so re-check before you sign (SpaceX Super Intelligence, n.d.).

- Grok Bot "is included on Premium, Super, and Ultra. Plus does not include Grok Bot" (SpaceX Super Intelligence, 2026e).
- Team plans: "Premium at $30 per seat, Super at $100 per seat, and Ultra at $200 per seat. Each seat includes the same usage as the matching individual tier." You can mix tiers (e.g., "three Premium seats and one Super seat"). "Plus isn't available for teams" (SpaceX Super Intelligence, 2026e).
- Team Bots, shared bots that everyone on a team can work with, "are available on Team and Enterprise plans" (SpaceX Super Intelligence, 2026d). "Meetings are available on Team, Enterprise, Ultra, and Super plans" (SpaceX Super Intelligence, 2026a).
- Enterprise is sold through sales, with no list price. The pricing page points organizations that "need invoicing, pooled usage, or advanced security" to Enterprise (SpaceX Super Intelligence, n.d.).
- The monthly prices exclude "Third Party model usage in Cursor" (the coding tool in the same subscription), which "must be purchased separately" (SpaceX Super Intelligence, n.d.).

No official page states how much work a seat's usage covers in hours, tasks or dollars. Bot usage "draws from that seat's shared weekly usage pool, not a separate additive pool," and on self-serve team plans "Seats do not share weekly pools" (SpaceX Super Intelligence, 2026e, 2026j). The pilot will have to measure this.

## Make the cap real: two settings, one boundary
"Capped spend" has to mean two settings, because there is no cap just for the bot: "A separate Grok Bot spend cap is not available today. Account-level on-demand controls apply" (SpaceX Super Intelligence, 2026c).

1. **A fixed number of seats at list price.** Seat cost for the pilot is the number of pilot seats times the tier price, for each billing period the pilot touches (SpaceX Super Intelligence, 2026e). Someone who joins mid-period gets "a new seat ... charged a prorated amount for the rest of the billing period" (SpaceX Super Intelligence, 2026i).
2. **A monthly additional usage limit.** This "controls how much paid Additional Usage you can use in a calendar month." Additional Usage is paid usage beyond each seat's included weekly pool, plus the third-party model usage above. Set it before day one. "Alerts do not stop usage. To put a hard stop on paid Additional Usage, set a monthly additional usage limit." Auto Top-up is "off unless you turn it on"; leave it off or bounded (SpaceX Super Intelligence, 2026g, 2026j).

Your maximum pilot spend is the seat cost for each billing period, plus the additional usage limit for each calendar month the pilot touches. Write that number down before you start.

Stopping takes deliberate steps. A removed member "lose[s] access to the team right away," but "Their seat stays on your plan" until an admin selects Reduce seats, and "Removed seats come off at the end of the billing period" (SpaceX Super Intelligence, 2026i). "On Team plans, a canceled seat stays active until the end of the billing period," and the pricing page says to cancel "at least 24 hours prior to renewal to avoid additional charges" (SpaceX Super Intelligence, n.d., 2026b). Put the Reduce seats step on the calendar before the end date.

The boundary is team membership. "On the Teams plan, Grok Bot is enabled by default, and every member has access without any admin action ... There is no switch to turn it off" (SpaceX Super Intelligence, 2026c). "People can belong to more than one workspace," so run the pilot in its own team workspace and add only the people in it (SpaceX Super Intelligence, 2026i). If the seat count and the limit are not set up front, the cost case falls apart.

## Write the stop rule before you start
Time-boxed, capped pilots are normal practice, even in large organizations; the examples here are from the UK government. Its Government Digital Service (GDS) ran a cross-government Microsoft 365 Copilot trial "from 30 September 2024 to 31 December 2024, involving 20,000 government employees," after earlier pilots "limited to 300 licences at most" (GDS, 2025b). DBT ran "One thousand licences ... for a 3-month pilot" (DBT, 2025).

Stopping is a legitimate result if the test is decided in advance. The GOV.UK Service Manual advises weighing "how much it'd cost against how much of an improvement you think you could make," and adds: "It's not a failure to stop at the end of the discovery phase if your research shows that's the best thing to do. In fact, you'll be saving time and money" (GDS, 2021). It also notes that "around 4 to 8 weeks is typical" for a discovery (GDS, 2021), and the UK Copilot pilots ran three months, so four weeks is the short end. We suggest stating that openly. Write these down, and get the exec to agree before day one:

- The end date, four weeks out.
- The cost-versus-improvement test you will apply at the end.
- Kill conditions (e.g., usage below a level you name, spend reaching the cap, or a quality incident you define).
- The off-limits list (see below).

## Weigh cost against time saved without fooling yourself
We found no published hours-saved figure for Grok Bot, so this article does not claim one. The UK cross-government trial reported that "Trial participants saved an average of 26 minutes a day," but a press release from the UK Department for Science, Innovation and Technology notes that "Figures are derived from self-reported daily time savings" (Department for Science, Innovation and Technology, 2025; GDS, 2025b). The DBT evaluation found "Small time savings were observed across most use cases," yet "The evaluation did not find evidence that time savings have led to improved productivity," and users "completed Excel data analysis more slowly and to a worse quality and accuracy than non-users" (DBT, 2025). It seems that self-reported time savings are weak evidence of value, so an exec who distrusts "hours saved" has a point.

The pilot should produce its own evidence instead. We suggest deciding in advance how time saved will be measured beyond self-report (e.g., timing a few repeat tasks before and during the pilot, or comparing samples of work from inside and outside it). That result can then be set against the maximum spend written down on day one.

## Pick who joins: volunteers plus a few who did not raise a hand
Everyone should get a chance to raise a hand, but volunteers are not a random sample. DBT let colleagues "volunteer for a licence, until around ~70% of licences had been allocated," then assigned the remaining ~30% to a random sample "stratified by directorate group and grade to improve representation" (DBT, 2025). In current US use of generative AI for work, "genAI adoption is 6 percentage points higher for men" (Bick et al., 2025, p. 10), and in the authors' statistical model the gap shrinks once occupation and employer encouragement are taken into account (Bick et al., 2025, p. 17, Table 1). We can suggest that pure self-selection may carry such gaps into a pilot, while a deliberate, encouraged pilot may narrow them.

Training and firsthand experience matter as well. DBT found "self-led training [was] more effective than formal departmental training sessions" (DBT, 2025). In the same Gallup article, Pendell (2025) found that 68% of US employees with firsthand experience using AI with customers said it had a positive effect, while only 13% of those without it believed it would. For this reason, mix the group: mostly volunteers, plus a few people who did not volunteer, with hands-on, self-led training.

## Clear review first, and keep some work off the bot
A central rollout has real strengths. Security, network controls, identity, data handling and procurement are easier to get right once than many times. The UK Government AI Playbook, published by GDS, asks that "You know how to use AI securely" and "You work with commercial colleagues from the start" (GDS, 2025a). Grok Bot's own rollout checklist asks admins to review proxy and TLS inspection, sign-in method and inherited policies before rollout, and several controls are "Enterprise only" (e.g., Network Controls, Team Secrets and Auto-review rules; SpaceX Super Intelligence, 2026c). The pilot should therefore invite security and commercial review, not route around it.

Some work should stay off the bot. The UK trial observed limitations "when dealing with complex, nuanced, or data-heavy aspects of work," and "Human oversight was required at all times" (GDS, 2025b). DBT reported hallucinations, and slower, less accurate Excel work (DBT, 2025). The Playbook asks for "meaningful human control at the right stage," including "ensuring that humans validate any high-risk decisions influenced by AI" (GDS, 2025a). Name the off-limits work in writing: high-risk decisions, and nuanced or data-heavy tasks without a human review.

## How it runs day to day: a structural example
lstack, an open template for a small team of content bots, is one example of the structure, not of results. Its working agreements state: "Files are the handoff." "A human approves every publish. No exceptions." "Work goes back to the previous step at most once" (lstack, 2026a). Each bot has a role file with its own OKRs (e.g., the researcher's "KR1: 100% of claims sourced"; lstack, 2026b). A pilot can borrow the shape: a human approves anything that goes out, work hands off in a place everyone can see, and each bot has a goal someone can check.

## Takeaway
Leaders should be obligated to decide, not to stay silent. The US evidence suggests that encouragement goes with far more use, and that few US workers say their employer gives it (Bick et al., 2025; Lin & Parker, 2025). A cautious exec does not need to make a company-wide decision to act on that. They can sanction one bounded pilot and ask for five things:

1. Sanction, said out loud, for one pilot team workspace.
2. A fixed seat count and tier at list price.
3. A monthly additional usage limit, with Auto Top-up off.
4. An end date four weeks out, with Reduce seats on the calendar before it.
5. A stop rule, a way to measure time saved beyond self-report, and an off-limits list, agreed before day one.

Security and commercial review should come first. If the pilot does not pay off, stopping is the result, and the organization will have saved time and money finding out.

## Appendix: further differences
These rows extend the comparison table. Each cell draws on the same official pages, read on Nov 20, 2026.

| | Grok Bot | ChatGPT Business or Enterprise (includes Codex) | Microsoft 365 Copilot | Gemini for Google Workspace |
|---|---|---|---|---|
| **What it is** | An assistant that works from its own persistent cloud computer with a browser, command line and files (SpaceX Super Intelligence, 2026k) | A ChatGPT workspace for teams; Codex is "OpenAI's coding agent that helps you write, review, and ship code"; in Slack, @ChatGPT "can send repository work to a separate Codex Cloud task" (OpenAI, n.d.-e, 2026a, 2026f) | An AI assistant across Microsoft 365 apps, sold as an add-on to a Microsoft 365 plan (Microsoft, n.d.-c) | Gemini built into Workspace apps such as Gmail, Docs and Meet (Google, n.d.-a) |
| **Connectors and plugins** | A "Connect apps" catalog; a Bot "can also add an MCP server that isn't in the catalog," and the team's MCP policy "applies in full" (SpaceX Super Intelligence, 2026c, 2026k) | Plugins "can include skills and MCP servers," in one directory shared by ChatGPT and Codex; Enterprise admins "configure app connections for teams" (OpenAI, n.d.-b, 2026b) | Copilot connectors for external data; Copilot Studio offers "Custom connectors ... to connect to any publicly available API" (Microsoft, n.d.-c, 2026c) | Schedules that use another app need it "connected"; Workspace Studio steps reach "Gmail, Sheets, and Drive, as well as other common apps" (Google, n.d.-c, n.d.-d) |
| **Computer use** | "Files, sign-ins, and browser sessions persist between tasks" (SpaceX Super Intelligence, 2026k) | Codex Cloud "runs coding tasks on OpenAI-managed computers"; Enterprise admin toggles for "Cloud browser use," "Cloud network access" and "Cloud computer use"; desktop Computer Use on macOS and Windows (OpenAI, n.d.-a, 2026e, 2026f) | Copilot Studio computer use "lets your agent interact with and automate tasks on a Windows computer," billed "through the Agent action feature with a billing rate of five Copilot Credits" (Microsoft, 2026a) | Chrome auto browse: "Gemini works in Chrome browser tabs to complete multi-step tasks"; "off by default for managed users" (Google, n.d.-b) |
| **Admin and data controls (examples)** | SCIM; Enterprise-only controls such as Network Controls and Enforce Auto-review; with Privacy Mode, "customer data is not used for training" (SpaceX Super Intelligence, 2026c) | Enterprise: "SCIM, EKM ... RBAC ... Audit logs," plus "Data retention and data residency controls"; on Business, "OpenAI won't train on your workspace's data" (OpenAI, n.d.-c, 2026a) | "Enterprise Data Protection (EDP), management, compliance, and controls"; scheduled-task data "stored within the Microsoft 365 compliance boundary" (Microsoft, n.d.-b, 2026b) | Work accounts: chats "won't be reviewed by human reviewers or otherwise used to improve generative AI models" (Google, n.d.-e) |

Several notes qualify both tables:

- **Promotional pricing.** Microsoft also lists a Copilot Business add-on "starting from $18.00," shown against "Originally starting from $21.00." That is a limited-time promotional price and may have expired by the time this article is read (Microsoft, n.d.-b). The table shows the standard $30 Enterprise add-on instead.
- **Feature changes.** New custom GPT creation is disabled for affected ChatGPT Enterprise workspaces, which are told to "Use Plugin Creator" instead (OpenAI, 2026b). Microsoft's Power Platform scheduled prompts retire on Dec 31, 2026 (Microsoft, 2026b).
- **Metered extras.** Microsoft lists some agent features as metered or usage-based, and OpenAI and Grok Bot both sell usage beyond included limits (Microsoft, n.d.-b, n.d.-c; OpenAI, 2026a; SpaceX Super Intelligence, 2026e). List price is therefore not total cost.
- **Defaults.** Several capabilities are off by default and need an admin, including ChatGPT workspace agents, Gemini auto browse and some Enterprise-only Grok Bot controls (Google, n.d.-b; OpenAI, 2026d; SpaceX Super Intelligence, 2026c). A pilot of any of them needs admin time.

## References
Bick, A., Blandin, A., & Deming, D. J. (2025). *The rapid adoption of generative AI* (Working Paper No. 2024-027F). Federal Reserve Bank of St. Louis. https://doi.org/10.20955/wp.2024.027

Bick, A., Blandin, A., Deming, D. J., Fuchs-Schündeln, N., & Jessen, J. (2026, March 26-27). *Mind the gap: AI adoption in Europe and the US* [Conference draft]. Brookings Papers on Economic Activity, Spring 2026, Washington, DC, United States. https://www.brookings.edu/wp-content/uploads/2026/03/6%5FBick-et-al%5Funembargoed.pdf

Department for Business and Trade. (2025). *The evaluation of the M365 Copilot pilot in the Department for Business and Trade*. GOV.UK. https://assets.publishing.service.gov.uk/media/68adbe409e1cebdd2c96a19d/dbt-microsoft-365-copilot-evaluation.pdf

Department for Science, Innovation and Technology. (2025, June 2). *Landmark government trial shows AI could save civil servants nearly 2 weeks a year* [Press release]. GOV.UK. https://www.gov.uk/government/news/landmark-government-trial-shows-ai-could-save-civil-servants-nearly-2-weeks-a-year

Google. (n.d.-a). *Compare flexible pricing plan options*. Google Workspace. Retrieved November 20, 2026, from https://workspace.google.com/pricing

Google. (n.d.-b). *Gemini in Chrome*. Chrome Enterprise and Education Help. Retrieved November 20, 2026, from https://support.google.com/chrome/a/answer/16291696?hl=en

Google. (n.d.-c). *Get started with Google Workspace Studio*. Workspace Studio Help. Retrieved November 20, 2026, from https://support.google.com/workspace-studio/answer/16444479?hl=en

Google. (n.d.-d). *Schedules in Gemini Apps*. Gemini Apps Help. Retrieved November 20, 2026, from https://support.google.com/gemini/answer/16316416?hl=en

Google. (n.d.-e). *Use Gemini Apps with a work or school Google Account*. Gemini Apps Help. Retrieved November 20, 2026, from https://support.google.com/gemini/answer/14620100?hl=en&co=DASHER._Family%3DBusiness-Enterprise

Google. (2026). *Let Google Meet AI take notes for my users*. Google Workspace Help. Retrieved November 20, 2026, from https://knowledge.workspace.google.com/admin/meet/let-google-meet-ai-take-notes-for-my-users

Google Workspace. (2025, September 18). *Introducing Gems sharing in the Gemini app, including admin controls*. Google Workspace Updates. https://workspaceupdates.googleblog.com/2025/09/gem-sharing-gemini-app-workspace.html

Government Digital Service. (2021). *How the discovery phase works*. GOV.UK Service Manual. https://www.gov.uk/service-manual/agile-delivery/how-the-discovery-phase-works

Government Digital Service. (2025a, February 10). *Artificial intelligence playbook for the UK government*. GOV.UK. https://www.gov.uk/government/publications/ai-playbook-for-the-uk-government/artificial-intelligence-playbook-for-the-uk-government-html

Government Digital Service. (2025b, June 2). *Microsoft 365 Copilot experiment: Cross-government findings report*. GOV.UK. https://www.gov.uk/government/publications/microsoft-365-copilot-experiment-cross-government-findings-report/microsoft-365-copilot-experiment-cross-government-findings-report-html

Kemp, A. (2026, July 20). *Organizational AI adoption jumps six points*. Gallup. https://www.gallup.com/workplace/712736/organizational-adoption-jumps-six-points.aspx

Lin, L., & Parker, K. (2025). *U.S. workers are more worried than hopeful about future AI use in the workplace* [Report]. Pew Research Center. https://www.pewresearch.org/wp-content/uploads/sites/20/2025/02/ST_2025.2.25_AI-Workers_REPORT.pdf

lstack. (2026a). *Working agreements* [AGREEMENTS.md]. GitHub. https://github.com/ZoneoutReal/lstack/blob/main/AGREEMENTS.md

lstack. (2026b). *Rhett, the Researcher* [roles/researcher.md]. GitHub. https://github.com/ZoneoutReal/lstack/blob/main/roles/researcher.md

Microsoft. (n.d.-a). *Facilitator in Microsoft Teams meetings*. Microsoft Support. Retrieved November 20, 2026, from https://support.microsoft.com/en-us/teams/copilot/facilitator-in-microsoft-teams-meetings

Microsoft. (n.d.-b). *Microsoft Copilot plans and pricing: AI for business*. Retrieved November 20, 2026, from https://www.microsoft.com/en-us/copilot/pricing/business

Microsoft. (n.d.-c). *Microsoft Copilot plans and pricing: Enterprise*. Retrieved November 20, 2026, from https://www.microsoft.com/en-us/copilot/pricing/enterprise

Microsoft. (2026a). *Automate web and desktop apps with computer use*. Microsoft Learn. Retrieved November 20, 2026, from https://learn.microsoft.com/en-us/microsoft-copilot-studio/computer-use

Microsoft. (2026b). *Manage scheduled prompts for Microsoft Copilot*. Microsoft Learn. Retrieved November 20, 2026, from https://learn.microsoft.com/en-us/copilot/manage/scheduled-prompts

Microsoft. (2026c). *Use connectors in Copilot Studio agents*. Microsoft Learn. Retrieved November 20, 2026, from https://learn.microsoft.com/en-us/microsoft-copilot-studio/advanced-connectors

OpenAI. (n.d.-a). *Computer Use* [Codex documentation]. Retrieved November 20, 2026, from https://developers.openai.com/codex/computer-use

OpenAI. (n.d.-b). *Plugins* [Codex documentation]. Retrieved November 20, 2026, from https://developers.openai.com/codex/plugins

OpenAI. (n.d.-c). *Pricing* [Codex documentation]. Retrieved November 20, 2026, from https://developers.openai.com/codex/pricing

OpenAI. (n.d.-d). *Scheduled tasks* [Codex documentation]. Retrieved November 20, 2026, from https://developers.openai.com/codex/automations

OpenAI. (n.d.-e). *Use ChatGPT in Slack* [Codex documentation]. Retrieved November 20, 2026, from https://developers.openai.com/codex/third-party/slack

OpenAI. (2026a). *ChatGPT Business overview*. OpenAI Help Center. Retrieved November 20, 2026, from https://help.openai.com/en/articles/8792828-chatgpt-business-overview

OpenAI. (2026b). *ChatGPT Enterprise and Edu release notes*. OpenAI Help Center. Retrieved November 20, 2026, from https://help.openai.com/en/articles/10128477-chatgpt-enterprise-and-edu-release-notes

OpenAI. (2026c). *ChatGPT Record*. OpenAI Help Center. Retrieved November 20, 2026, from https://help.openai.com/en/articles/11487532-chatgpt-record

OpenAI. (2026d). *ChatGPT workspace agents for Enterprise and Business*. OpenAI Help Center. Retrieved November 20, 2026, from https://help.openai.com/en/articles/20001143-chatgpt-workspace-agents-for-enterprise-and-business

OpenAI. (2026e). *Managing dots in ChatGPT workspaces*. OpenAI Help Center. Retrieved November 20, 2026, from https://help.openai.com/en/articles/20001554-managing-dots-in-chatgpt-workspaces

OpenAI. (2026f). *Using Codex with your ChatGPT plan*. OpenAI Help Center. Retrieved November 20, 2026, from https://help.openai.com/en/articles/11369540-using-codex-with-your-chatgpt-plan

Pendell, R. (2025, June 15). *AI use at work has nearly doubled in two years*. Gallup. https://www.gallup.com/workplace/691643/work-nearly-doubled-two-years.aspx

Puthal, D., Mishra, A. K., Mohanty, S. P., Longo, A., & Yeun, C. Y. (2025). Shadow AI: Cyber security implications, opportunities and challenges in the unseen frontier. *SN Computer Science, 6*(5), Article 405. https://doi.org/10.1007/s42979-025-03962-x

SpaceX Super Intelligence. (n.d.). *Pricing: Compare plans*. Retrieved November 20, 2026, from https://x.ai/pricing

SpaceX Super Intelligence. (2026a). *Add a Bot to your meetings*. Retrieved November 20, 2026, from https://docs.x.ai/grok-bot/meetings

SpaceX Super Intelligence. (2026b). *Cancel your subscription*. Retrieved November 20, 2026, from https://docs.x.ai/x-subscription/cancel

SpaceX Super Intelligence. (2026c). *Grok Bot for teams and enterprises*. Retrieved November 20, 2026, from https://docs.x.ai/grok-bot/teams-and-enterprises

SpaceX Super Intelligence. (2026d, November 11). *Introducing Grok Bot 1.0*. https://x.ai/news/grok-bot-1-0

SpaceX Super Intelligence. (2026e). *Pricing*. Retrieved November 20, 2026, from https://docs.x.ai/x-subscription/pricing

SpaceX Super Intelligence. (2026f). *Skills and routines*. Retrieved November 20, 2026, from https://docs.x.ai/grok-bot/skills-routines-and-automations

SpaceX Super Intelligence. (2026g). *Spending caps: Monthly extra-usage caps and alerts*. Retrieved November 20, 2026, from https://docs.x.ai/x-subscription/spending-caps

SpaceX Super Intelligence. (2026h). *Team Bots*. Retrieved November 20, 2026, from https://docs.x.ai/grok-bot/team-bots

SpaceX Super Intelligence. (2026i). *Team plans: Workspaces, seats, and invites*. Retrieved November 20, 2026, from https://docs.x.ai/x-subscription/team-plans

SpaceX Super Intelligence. (2026j). *Usage limits*. Retrieved November 20, 2026, from https://docs.x.ai/x-subscription/usage-limits

SpaceX Super Intelligence. (2026k). *Use the computer and apps*. Retrieved November 20, 2026, from https://docs.x.ai/grok-bot/computer-and-apps

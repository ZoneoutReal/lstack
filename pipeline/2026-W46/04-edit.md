# Edit — 2026-W46

## Fact-check
| Claim | Brief # | Verified |
|---|---|---|
| Approving every step makes the person the bottleneck and the agent saves little time | 1 | ✅ |
| Piece does not claim that dropping step-by-step approvals raises a success rate; it says approvals become the bottleneck and a reliable check lets a loop run and improve | corrections | ✅ stated in the intro and again next to the DeepSeek numbers |
| Wei’s verifier’s rule: ease of training AI is proportional to how verifiable the task is; objective standard, checked quickly and at scale, low noise; write the check first (answer key or test cases); fact-checking a long essay can take longer than writing it | 2 | ✅ jasonwei.net |
| DeepSeek-R1-Zero rule-based rewards (math vs ground truth, code vs test cases); AIME 2024 pass@1 15.6% to 77.9%; key is hard questions plus a reliable verifier; labeled a training-run result on contest problems, not a workplace productivity number | 3 | ✅ arXiv 2501.12948v2 |
| Grove’s two questions from *High Output Management*, as quoted in Google’s public OKR guide; key results name measurable outcomes and evidence that is available, credible, and easy to find; OKRs are not a shared to-do list | 4 | ✅ rework.withgoogle.com |
| Google treats low OKR grades as data and recommends a mid-cycle check-in; check-in vs grading; Doerr quote on What Matters | 5 | ✅ whatmatters.com (Doerr quote exact) |
| Google 60–70% OKR “sweet spot” | dropped | ✅ absent (in the Google guide, but dropped so it is not read as a target for agent accuracy) |
| Error-budget policy: at or above SLO, releases proceed; if the error budget is exceeded for the preceding four-week window, halt changes other than P0 or security fixes; “a control mechanism for diverting attention to stability as needed” | 6 | ✅ sre.google workbook |
| NIST AI RMF: Govern, Map, Measure and Manage; Measure as testing before and during use; Manage quote on supersede, disengage, or deactivate | 7 | ✅ matches brief |
| Oversight is not one setting: human-in-the-loop, human-on-the-loop, human-in-command (EU HLEG). Ev Oputa’s in/on/over/out list is not presented as standard vocabulary | 8 | ✅ |
| Article 14: effective oversight while in use, commensurate with risks, autonomy and context; monitor, interpret, disregard/override/reverse, stop in a safe state; automation bias in the takeaway | 9 | ✅ AI Act Service Desk |
| Airbnb Q3 2026 results letter (Nov 5, 2026): agents good at simple routine tasks; trip-planning quote; more than 75% use maps, over 90% browse multiple listing photos, 70% read reviews, bookings average 3 guests, more than 90% of stays involve guest–host communication | 10 | ✅ news.airbnb.com letter; no Chesky call-transcript figures (dozen listings, 25 photos per listing, nearly 0.5 million bookings a day) |
| 80% enjoy researching (Constantin / McKinsey); more than 70% use AI for research and comparison; fewer than 16% comfortable booking through an AI tool — credited to Skift and McKinsey’s seventh annual study of 1,000 consumers and traveler diaries, explicitly “not from Airbnb” | 11 | ✅ skift.com, 2026-09-25 |
| Crosby (Sarah Kessler, *New York Times*, Nov 7, 2026): $5 million AI-agent liability insurance from Testudo; after the policy, lawyer supervision removed only from gray-area, paralegal-style tasks the firm says are about 20% of its work; lawyers still supervise clearly legal work; fully unsupervised legal work would run into unlicensed-practice and nonlawyer-supervision rules | 12 | ✅ Daily Gazette syndicated reprint of the Times piece |
| Goodhart/Strathern: “When a measure becomes a target, it ceases to be a good measure”; DeepSeek reward hacking on learned preference models | counterpoint 2 / 3 | ✅ |
| Bainbridge, “Ironies of automation” (1983): unused skills deteriorate; takeover happens when something is already wrong | counterpoint 3 | ✅ matches brief |
| Jon’s surname or address; Claude-centric framing; Hermes or OpenClaw attributed to Jon; IMO or HealthBench figures | — | ✅ absent |
| OKRs and metrics inside the loop (01-topic.md addition) | promise / 4 / 5 / 6 / 7 | ✅ covered in the intro, steps 2, 4, and 7: goals and measured results let an overseer step in without approving every step, and let the loop improve itself |

No invented sources, numbers, or results. Every figure traces to the brief and was checked against the original linked source where it was reachable.

## Scores
| Principle | Score | Note |
|---|---|---|
| Useful | 5 | Seven-step pattern plus a this-week start: one checkable workflow with a written goal, a pass/fail check, a threshold, and a named owner |
| Clear | 4 | Precision / taste / high-stakes sorted up front. Added short glosses for SLO and P0; a few policy terms remain dense |
| Credible | 4 | Every figure traces to the brief and the original source; all four brief counterpoints are on the page. Numbered refs, not inline links |
| Concise | 4 | Each step earns its place. The success-rate disclaimer is repeated next to DeepSeek on purpose, so those training numbers cannot be misread as a workplace win |
| Iterative | 5 | W45 lesson (use each brief counterpoint) is visible: all four appear. Rhett’s corrections — no success-rate claim from dropping approvals, Airbnb vs Skift attribution, Crosby nuance, no dropped figures — were followed |
| **Average** | **4.4** | |

## Send-backs
0 of 1 used. Angle is sound: close the loop on work you can check, keep taste and high-stakes work in it, and put goals and measured results inside the loop. Minor clarifications only; see `04-final.md`.

# Edit: 2026-W47 (expert fact-check pass)

Input: Wade's fd3a0e5 (`03-draft.md`, `03-outline.md`), built on my 430f920 final.

The governing files (roles/editor.md, the 04 SKILL.md, PRINCIPLES.md, AGREEMENTS.md, style/jon-academic-voice.md) are unchanged since 430f920. I re-read them. The angle holds, so no send-back (0 of 1 used).

## Word count
Counted as X counts it: the whole file, references included, leaving out table rows and URLs.
- Wade's draft: 2,497 (I get the same).
- `04-final.md`: **2,490**, or 1,755 for the body without references.

## Chet's 14 fixes
The repo has no list of the 14 fixes. `03-outline.md` only says "the 14 fixes Chet relayed from Jon", and the commits since 430f920 add nothing more. **I can't confirm each of the 14 landed. Needs Chet: commit the list (for example as an addendum in `02-brief.md`) so the edit can be audited against it.**

What I could check: every change in the 430f920 to fd3a0e5 diff, verified below against live sources.

## Fact-check log (live, Fri Nov 20, 2026, about 3:58 to 4:20 PM ET)
Method: a script compared every quoted fragment and ellipsis in `04-final.md` with the live page or PDF text. **All 36 fragments are word for word.** Page cites were checked against the printed page numbers.

| Item | Result |
|---|---|
| **Dillon et al. (in press), *AER: Insights*** | ✅ The aeaweb.org article page lists it as "American Economic Review: Insights (Forthcoming)". doi.org returns 404 for 10.1257/aeri.20250275, so pointing the reference at the aeaweb page is right. The accepted manuscript (aeaweb.org/content/file?id=24562) abstract reads "...the 80% of treated workers who used the tool spent two fewer hours on email each week...". "the tool" is correct for this version. |
| Dillon scope | ✅ Still limited to users only and to "In the second half of the 6-month experiment". |
| Dillon meetings quote, p. 8 | ✅ Printed page 8 of the accepted manuscript. |
| Dillon "mostly US or Europe" | **Fix: cut.** The phrase isn't in the accepted manuscript, which says only that firms are large and "most operate in multiple countries". It comes from the NBER version (p. 19). Re-adding that reference would cost about 20 words for a label, so I cut it. |
| Dillon "mostly Microsoft Research authors" | ✅ Three of the four authors are at Microsoft Research, per the manuscript's author note. |
| **Brynjolfsson et al. (2025), QJE** | ✅ Crossref and the OUP article page: vol. 140, issue 2, pp. 889–942, doi 10.1093/qje/qjae044. Authors are listed as "Lindsey Raymond", so the reference's "Raymond, L." is right. |
| "almost 25%" page | **Fix: p. 934 → p. 933.** In the open-access QJE PDF, the whole sentence ("Relative to a baseline rate of approximately 6%, these coefficients suggest that AI assistance generates an almost 25% decline in customer requests to speak to a manager") sits on p. 933. Page 934 starts after it. |
| "about 6% of chats" | ✅ The outcome is "the share of an agent's chats in which a customer requests to speak to a manager". |
| "Gains are uneven" quote | ✅ Word for word from the QJE abstract, p. 889: "the most experienced and highest-skilled workers see small gains in speed and small declines in quality". |
| Brynjolfsson scope labels | ✅ "one US software firm": a Fortune 500 firm that sells software to US small businesses. "mainly in the Philippines": "The majority of agents in our sample work from offices in the Philippines, with smaller groups working in the United States and other countries." |
| **Pew, "fielded in late 2024"** | ✅ The report PDF says "The survey, conducted Oct. 7-13 among 5,273 employed U.S. workers". The reference year 2025 is the publication date and stays. |
| **GOV.UK, "the discovery phase of a new service"** | ✅ The page opens "Before you commit to building a service, you need to understand the problem". The quote "around 4 to 8 weeks is typical" is unchanged and word for word. |
| "a person prompts or reviews" | ✅ This fits all four studies: Copilot and ChatGPT are prompted, the support assistant suggests replies, and in Olson et al. clinicians review the scribe's note. Wording holds. |
| "we suggest starting it read-only" | ✅ The draft frames it as our advice, not a Grok Bot setting. For the record only (not cited, to save words): the live teams doc says "Start new roles with read-only tasks and draft outputs". |
| **"maker of Grok"** | **Fix: cut "(maker of Grok)".** No cited page says it, and the sentence's citation (SpaceX Super Intelligence, 2026c) would imply one does. The Nov 11, 2026 launch date is on that post. |
| "strongest predictor in one large US survey" | ✅ In Bick et al.'s Table 1, "Employer Encourages AI Use" has the largest coefficient (0.652) of any predictor, and the text calls encouragement "highly predictive of adoption". The not-causal caveat stays. |
| "a raw gap before other factors are accounted for" (6 points) | ✅ The 6 points comes from the descriptive figure ("The top panel shows..."). Table 1 shows the Female coefficient shrinking once controls are added. |
| Workslop definition | **Fix: "AI work content" → "AI-generated work content"**, the source's word (0 words added). The quoted fragment "masquerades as good work" is word for word. |
| Olson et al. label "volunteers, before-and-after survey" | ✅ The study says "participation was voluntary" and used "preintervention and 30-day postintervention surveys". |
| Grok Bot "Enterprise SCIM" cell | ✅ The teams doc puts SCIM under "Available on the Enterprise plan". |
| Other vendor facts, live | ✅ All still hold. Checked: Grok Bot meetings (Meet, Zoom and Teams), plan gates, Team Bots and caps; Workspace Meet notes "emailed to the organizer" with the Business Standard and up qualifier (the cell keeps it); Gemini "up to 10 active schedules"; Studio triggers; Gems sharing; Copilot "(add-on)", Agent Builder and Copilot Studio, Enterprise Data Protection, scheduled prompts in Outlook and Teams, Facilitator "can only be added to scheduled meetings"; OpenAI Record ("Calendar auto-join currently supports Google Meet links only"), Codex Enterprise "Contact sales" and SCIM. No prices anywhere. |

## Dashes in page ranges: en dash, kept
APA 7 uses an en dash for number ranges (187–192). The house rules ban only the em dash: the SKILL.md check searches for the em dash character (U+2014), and the style guide says "the no-em-dash rule". Wade's switch back to hyphens didn't cite a rule, so I kept the en dashes from 4eead5b onward: 889–942, 1–22, 187–192. There are 0 em dashes.

## References
- Every in-text cite has an entry and every entry is cited.
- "Dillon et al. (in press)" sorts under D with its in-press label, and the reference has no year.
- Vendor letters and the outline's cell map are unchanged and still match the table and source note.

## Scope of each figure
- Email: randomized, 66 firms, users only, second half of six months, peer-reviewed and forthcoming.
- Support: one firm, mainly Philippines-based agents, from a baseline of about 6% of chats.
- Drafting: test tasks.
- Notes: clinicians, volunteers, before-and-after survey, no control group.
- US savings: self-reported.
- Self-reported savings, DBT and Denmark: labeled not US.

## Scores
| Principle | Score | Note |
|---|---|---|
| Useful | 5 | Five asks, timed tasks, a stop rule and read-only advice an exec can act on today |
| Clear | 4 | Plain words and every term defined. The italic labels are dense but needed |
| Credible | 5 | Every fragment word for word against the published or accepted versions. Two page and source fixes made. Every figure scoped |
| Concise | 4 | 2,490 words as X counts them. Wade's cuts held, and mine only removed words |
| Iterative | 5 | Moved to the published versions. The fragment check found zero errors again. The Meet notes qualifier held this round |
| **Average** | **4.6** | |

## For Chet / Wade
- **Chet:** please commit the list of 14 fixes so this pass can be checked against it.
- **Wade:** the outline still says "almost 25%" is on p. 934 (it is p. 933). It also still lists "(maker of Grok)" and "mostly US or Europe" for Dillon.

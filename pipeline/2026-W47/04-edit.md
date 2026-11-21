# 04 Edit: Edie, Addendum 7 pass (input 9feadfe, built from daff1c0)

Governing files re-read at main: roles/editor.md, skills/04-edit-and-polish/SKILL.md, PRINCIPLES.md, AGREEMENTS.md, style/jon-academic-voice.md, 01-topic.md (Direction update 6) and 02-brief.md (Addendum 7). Every source was re-opened live on November 21, 2026, and every quote fragment was diffed by script against the source text. Cut and clarify only; nothing was rewritten.

## Scores (1-5)
| Criterion | Score | Note |
|---|---|---|
| Useful | 4 | The pilot design, five measures and stop rule still carry the article. The evidence base is now thinner and heavily labeled. |
| Clear | 4 | Labels are dense but consistent. Removed one unsourced superlative. |
| Credible | 4 | Every quote matches its source. Fixed one unsupported date label (Gallup 1.7x). Four of the seven new-window sources are preprints or a working paper, and every one is labeled. |
| Concise | 4 | 2,367 words, inside 2,000-2,500. |
| Iterative | 5 | Direction update 6 and Addendum 7 are fully delivered: all swaps made, all cuts gone, all knock-on fixes in. |
| **Average** | **4.2** | |

Send-backs used: 0 of 1. The angle holds, so no send-back.

## Word count
Counted the X way: the whole file including references, excluding table rows and URLs. Wade's draft is 2,377, which I confirmed. The final is **2,367**.

## Edits (cut or clarify only)
1. **Gallup 1.7x date label (clarify).** The draft read "(data as of May 2026)". On the live Gallup indicator page, "As of May 2026" belongs to the 36% sentence. The 1.7x line says only "Gallup's research shows employees in AI-adopting organizations who strongly agree that their manager actively supports their team's use of AI are: 1.7x as likely...", with no date. The label now reads "(the page does not date this figure)". This one goes to Chet (see below).
2. **Cut: "Manager support is one of the clearest signals in recent US survey data."** This was an unsourced superlative, and no source ranks the signals. The section heading and the Gallup quote carry the point.
3. **Ma et al. label (clarify).** "Microsoft authors" became "mostly Microsoft authors". The PDF lists 4 of the 7 authors at Microsoft (Khadpe, Pang, Suri and Iqbal) and 3 at Carnegie Mellon. The first author's work was done during a Microsoft internship.

## Delivery check: Direction update 6 and Addendum 7
- **Swaps delivered:**
  - Gallup indicator: the 1.7x, 36% and 26% figures.
  - Kemp's task mix.
  - The FRED Blog's 2.2%, with its self-report caveat.
  - Autor et al. (drafting bullet rewritten, not number-swapped).
  - Yu et al. (the timing section).
  - Ma et al. (the trust and checking bullet).
  - Wang et al. (the agents bullet, the gap wording and the takeaway).
- **Plan, not encouragement:** the 26% is framed as a plan, not as encouragement. Pass.
- **Correlation:** the Gallup link has no causal wording, and the caveat "This is a survey link, not proof that manager support causes use (our wording)" is present. Pass.
- **Knock-on fixes:**
  - "Three terms" ends with the Gallup-measures sentence.
  - The takeaway uses the Wang wording.
  - The stop-rule Sources line names only remaining sources.
  - The UK sentence is gone from "Pilots do track use".
  - Design has lost the DBT, gender-gap and Playbook lines. The read-only, reviewer and off-limits advice stays, labeled ours.
  - Pass.
- **Cut list:** a grep for Bick, Pew, Lin and Parker, DBT, Business and Trade, Brynjolfsson, Humlum, METR, Becker, Lee et al., workslop, BetterUp, Playbook, Grok, Noy, Excel, gender, escalation, "26 minutes", 83%, DSIT and GDS 2025a/b returned no matches. Only two lines matched the broad patterns, and both are fine: Dillon's "80% of treated workers" and the GOV.UK discovery guide (GDS, 2021). Pass.
- **References:** 14 entries (Autor, CAISI, Pennsylvania, Dillon, FRED, Gallup, GDS 2021, Kemp, Ma, Olson, Puthal, GAO, Wang and Yu). Each is cited in the body, and every body citation has an entry, so there are no orphans in either direction. Pass.
- **Dashes:** em dashes (U+2014): 0. En dashes: 1, in the CAISI page range 698–701 (APA 7). Pass.
- **House rules:**
  - No prices.
  - No surname.
  - Comparisons are worded per house style.
  - "Article", not "piece".
  - Pass.

## Fact-check log (live, verbatim; quote fragments diffed by script)
- **Gallup (n.d.), indicator page** (fetched live):
  - "1.7x as likely to use AI a few times a week or more": verbatim. Population: "employees in AI-adopting organizations who strongly agree that their manager actively supports their team's use of AI". Undated on the page. Fixed (edit 1).
  - "As of May 2026, nearly four in 10 employees (36%) in AI-integrating organizations strongly agree that their manager supports their team's use of AI": verbatim.
  - "As of August 2026, 26% of U.S. employees say their organization has communicated a clear plan for integrating AI into current practices": verbatim.
  - Pass.
- **Kemp (2026), Gallup:**
  - The byline reads "by Andy Kemp", July 20, 2026.
  - "Among AI users, the most common uses of AI are writing and editing (51%), search or research (49%), and general assistance or problem-solving (39%)": verbatim.
  - Methods table: "Q2 2026 May 6-20, 2026 22,573", employed US adults, Gallup Panel. The article reports Q2 2026 results.
  - The label "US survey fielded May 6 to 20, 2026" is correct. Pass.
- **Federal Reserve Bank of St. Louis (2026), FRED Blog**, posted August 27, 2026 (read via WebFetch because the site drops curl):
  - "the share of work hours saved thanks to AI assistance grew from 1.6% to 2.2%": verbatim.
  - The span is stated as "from 28.2% in Q3 2024 to 39.2% by Q2 2026", with hours saved "over roughly the same stretch".
  - "The information is based on how respondents self-report their “time saved,” so the measurements are inherently approximate": verbatim. Inside our double quotes, the inner marks correctly become single quotes, which is why the script flagged it.
  - The source is the Real-Time Population Survey, "nationally representative". The label "self-reported; data from Q3 2024 to Q2 2026" is correct. Pass.
- **Autor et al. (2026), NBER WP 35720** (PDF and NBER page):
  - "133 practicing patent lawyers at eleven U.S. intellectual property law firms": abstract, verbatim.
  - "Treated lawyers spent about 10 fewer minutes on the 10-day drafting task than controls (p = 0.05), whose mean was 110 minutes": PDF p. 4, with printed page number 2 confirmed in the footer. Verbatim except that the source sets p in math italic, so the script flagged it.
  - "with larger gains among junior lawyers", "was concentrated entirely among senior lawyers" and "Junior lawyers showed no average gain": abstract, verbatim.
  - Data: "the study period of May 2025 through February 2026" (PDF p. 9).
  - Funding: "Funding for the direct costs of this experiment was provided by Google"; "The study was conducted by Google". Google employment and contractor disclosures appear on the NBER page. The label "funded by Google, with Google staff among the authors" is supported.
  - Dated "September 2026, Revised October 2026".
  - The author list matches the reference. Pass.
- **Yu et al. (2026), arXiv 2605.23177**, submitted May 22, 2026:
  - "a preregistered large-scale behavioral study (N = 1237)", "While actual completion times between independent completion and AI-assisted completion did not differ, participants predicted AI to be significantly faster" and "participants reported lower subjective effort with AI despite equivalent completion times": abstract, verbatim.
  - Methods: Prolific, "comprising a representative sample of the US adult population"; "N=1237 in total: 401 in the prediction sample and 836 in the completion sample".
  - I searched the full text for collection dates and found none, so "collection dates not stated" is correct.
  - The author list matches. Pass.
- **Ma et al. (2026), arXiv 2610.14660**, submitted October 10, 2026:
  - Both abstract quotes are verbatim.
  - "20 professionals" in a "think-aloud study", recruited "at a large technology company".
  - No collection dates are stated.
  - The reference uses the PDF spelling of names (Khadpe, Pang, Suri), which differs from the arXiv listing. That is correct for APA. Pass after edit 3.
- **Wang et al. (2026), arXiv 2605.14830**, v1 May 14, 2026, and v2 June 1, 2026:
  - The abstract quote is verbatim.
  - "a randomized field experiment conducted on Alibaba's ecommerce platform, Taobao.com, in August 2024, involving 647 customer service workers and 680,676 service chats" (Introduction).
  - One author lists "Alibaba Group Inc."
  - Labels "not US (Taobao, China); preprint; data from August 2024; one author at Alibaba Group": all correct.
  - The reference cites Version 2. Pass.
- **Dillon et al. (in press), accepted manuscript:**
  - Abstract (p. 1): "integrated into applications they already used at work for email, meetings, and writing", "In the second half of the 6-month experiment, the 80% of treated workers who used the tool..." and "do not detect shifts in the quantity or composition of workers' tasks".
  - "We find no similar shifts in the time workers spent in Teams meetings" (p. 8).
  - "Between September 2023 and October 2024" (p. 1) supports "data from 2023 to 2024". Pass.
- **Commonwealth of Pennsylvania (2025):** all quotes are verbatim at the cited pages: p. 2, p. 3, p. 8, p. 11, p. 12, p. 16, p. 33, p. 34, p. 43, p. 48 and p. 54.
  - The p. 9 "14 ... state government agencies" is an infographic. The number and its caption sit in separate text boxes, confirmed with pdftotext -layout.
  - The p. 43 quote is verbatim across a two-column layout.
  - p. 10: "from March 2024 – March 2025" supports "data from 2024 to 2025". Pass.
- **Olson et al. (2025), PMC** (read in the browser; the site blocks curl):
  - "burnout among those working in ambulatory clinics decreased significantly from 51.9% to 38.8%" and "There was no control group": both verbatim.
  - "conducted between February 1 and October 31, 2024" supports "data from 2024". Pass.
- **Puthal et al. (2025), CAISI (2026), GAO (2025) and GDS (2021):** text unchanged since daff1c0. The quotes match, and these sources are exempt from the recency rule (definitions and non-AI points). Pass.

## Cutoff-rule rulings (AI data after May 20, 2026; otherwise say which years the data cover)
- **Dillon et al. (2023 to 2024), Pennsylvania (2024 to 2025), Olson et al. (2024):** none meets the six-month data rule. Jon names all three as keeps in Direction update 6, and each carries its "data from" label wherever its figures appear. **Compliant by Jon's explicit exception.** No change.
- **Kemp (2026):** published inside the window (July 20, 2026). Fieldwork ran May 6-20, 2026, ending on the cutoff day, so it is not strictly "after May 20". The rule's own fallback for older data inside an in-window source is to state the dates, and the label does: "US survey fielded May 6 to 20, 2026". **Compliant via the label.** No change.
- **FRED Blog (2026) and Autor et al. (2026):** both were published inside the window, with older data labeled (Q3 2024 to Q2 2026; May 2025 to February 2026). **Compliant.**
- **Yu et al. and Ma et al.:** both were published inside the window (May 22 and October 10, 2026), and neither states when its data were collected. The rule asks us to state the data years, which we cannot do. "Collection dates not stated" is the honest label, and Jon named both papers as swaps. **Compliant as labeled.** Whether that is enough is listed for Chet below.
- **Wang et al.:** data from August 2024. v1 (May 14, 2026) predates the window, and v2 (June 1, 2026), the version cited, falls inside it. Jon named it, and the "data from August 2024" label appears in the bullet, the gap paragraph and the takeaway. **Compliant by Jon's naming.**
- **Gallup indicator:** the 26% is dated August 2026, which is in the window. The 36% is "as of May 2026", which may sit on or before the cutoff and is labeled in the quote itself. The 1.7x is undated on the page. Now labeled "the page does not date this figure". **Flag for Chet.**

## Items for Chet
1. **Gallup 1.7x is undated on the source page.** Addendum 7 and the draft labeled it "data as of May 2026", but on the page that date belongs to the 36% sentence. I relabeled it honestly. Chet should decide whether an undated AI figure satisfies Direction update 6, or whether Rhett should find a dated source.
2. **Yu and Ma, "collection dates not stated":** does publication inside the window satisfy the rule? I kept both, labeled, because Jon named them.
3. **Wang, the only agent trial, uses 2024 data,** and its v1 predates the window. It is labeled in all three places. Chet should confirm with Jon (Rhett's open question, which I carried forward).
4. **Group wording in "Support goes with use":** the 36% covers "AI-integrating organizations" and employees whose manager "supports" AI use, while the 1.7x covers "AI-adopting organizations" and a manager who "actively supports" it. "That group" bridges two slightly different Gallup populations. I let it stand because both are Gallup's own framings of the same manager-support measure. Chet may want it tightened.

## Pax packaging notes
- Everything from daff1c0 or earlier is stale, including the 05-package at 1f733b9 and 22a3c18. It cites cut sources.
- **Teaser (Addendum 7 / outline), checked against this final:**
  - "In a preregistered study of 1,237 US adults, people predicted AI would make simple tasks faster. Completion times did not differ (Yu et al., 2026, preprint). So time the work by the clock. A case for a capped, four-week opt-in pilot of AI agents: ARTICLE_URL" comes to 270/280.
  - **Every fact holds:** preregistered, N = 1237, a representative US-adult sample via Prolific (Methods), simple tasks, no difference in completion times, preprint.
  - **Precision note:** the 1,237 are split into a 401-person prediction sample and an 836-person completion sample. "People predicted ... Completion times did not differ" stays accurate as long as it doesn't say the same people did both.
  - **Missing label:** "collection dates not stated", which the article carries under the cutoff rule. The full wording would run 285/280. A version that fits at 274/280: "In a study of 1,237 US adults, people predicted AI would make simple tasks faster. Completion times did not differ (Yu et al., 2026, preprint, dates not stated). So time the work by the clock. A case for a capped, four-week opt-in pilot of AI agents: ARTICLE_URL". It drops "preregistered".
  - Pax and Chet decide.
- **Labels to keep on any other X copy:**
  - Gallup 1.7x is a survey link, not causal, and undated.
  - FRED's 2.2% is self-reported, Q3 2024 to Q2 2026.
  - Autor is a US working paper funded by Google, with data from May 2025 to February 2026.
  - Wang is not US, a preprint, with data from August 2024.
  - Ma is a preprint of 20 professionals, mostly Microsoft authors.
  - No prices, no tool names in promos, no Grok Bot.

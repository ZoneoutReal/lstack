# Edit: 2026-W47 (tool-agnostic exec pilot case)

**Inputs**
- Wade's 5164d34 (`03-draft.md`, `03-outline.md`).
- Governing direction: Direction update 5 (`01-topic.md`, f76fa55), Addendum 5 (`02-brief.md`, c7c604c) and Addendum 6 (`02-brief.md`, 5d58c1a, the AI agent definition).
- The governing files (roles/editor.md, the 04 SKILL.md, PRINCIPLES.md, AGREEMENTS.md, style/jon-academic-voice.md) are unchanged and were re-read.

**Angle: holds.** No send-back (0 of 1 used).

## Word count (X way: whole file, references included, no table rows or URLs)
- Wade's draft: 2,434 (I get the same).
- `04-final.md`: **2,490**, or 2,030 for the body without references.
- The sourced definition and its two references added about 70 words. I offset them with the cuts listed below.

## Does the draft deliver Direction update 5 and Addendum 5?
| Ask | Result |
|---|---|
| Tool-agnostic case for a capped, opt-in pilot of AI agents across uses, not a Grok Bot pitch | ✅ The Grok Bot fit section, table, claims 1 to 6 and Notes 1 to 3 are gone. Claim 7, the rollout checklist and lstack moved to W48. I also cut the last Grok Bot sentence (Addendum 5 §3 allows "or cut"), so the article names no vendor tool except those the studies tested. |
| Keep the productivity evidence, definitions, limits and the risk line | ✅ All kept. The risk line is labeled ours ("we suggest starting each one read-only"). |
| §1 several uses: Dillon, UK, DBT, Pennsylvania (labeled), METR (labeled) | ✅ Present. Pennsylvania doesn't lead with "95 minutes"; it's tied straight to "Estimates reported by participants in exit survey". |
| §1 thin list: multi-tool, agents acting on their own, teams (Pennsylvania p. 54), opt-in vs mandate | ✅ All four are stated plainly. Opt-in vs mandate is in "Encouragement goes with use". |
| §2 stop rule in plain words: what is measured, by when, what happens | ✅ Five measures, week 2 and week 4, judged per use case. The table column is "Bar (ours)" and the source note says "Every bar and the stop rule are ours; no source sets a threshold." The end-date decision is "we suggest". |
| "Stopping is the result" cut | ✅ Gone. GOV.UK quotes kept as support for deciding the test up front. |
| "Article," not "piece"; no em dashes; no surname; no prices | ✅ |

## Checks requested
1. **"AI agents" definition: fixed with Addendum 6.** Wade's labeled working definition wouldn't have blocked the edit, since Jon's rule allows "say the wording is ours". Now a cited one exists, so I swapped in Rhett's sentence. That's a clarification from the brief, not a rewrite. Verified live:
   - **CAISI, Federal Register 91(5), p. 699:** "AI agent systems consist of at least one generative AI model and scaffolding software that equips the model with tools to take a range of discretionary actions" and "They can be deployed with little to no human oversight". The notice's AGENCY line names CAISI at NIST, it is dated Jan 8, 2026, and it runs pp. 698–701 (FR Doc. 2026-00206). The reference is correct.
   - **GAO-25-108519, p. 1** (published Sep 10, 2025): agentic AI makes "and adjust[s] plans" toward a goal, and "an AI agent could interact with other software systems to process a return or exchange". I kept GAO's caveat word for word and briefly: "There is no universally agreed upon definition of an AI agent" (p. 1). The reference carries GAO's release date.
   - **Paraphrase:** faithful on every clause (built on a generative model, plans and acts toward a goal, uses tools in other systems, the returns example, little oversight). It adds nothing the sources don't say.
2. **Dillon et al. meetings quote, p. 8: pass.** It is on printed p. 8 of the accepted manuscript (aeaweb.org/content/file?id=24562). The reference is the in-press *AER: Insights* entry, which matches. The email quote and scope (users of the tool, second half of the 6-month experiment) are word for word from that abstract. "integrated into applications they already used at work for email, meetings, and writing" also matches.
3. **UK figures:**
   - **20,000: pass.** GDS (2025b): a cross-government Microsoft 365 Copilot trial "from 30 September 2024 to 31 December 2024, involving 20,000 government employees". The text names it as UK.
   - **83% and 80%: fixed scope.** The adoption rate is "the ratio between active users and number of users with a M365 Copilot licence", where active means "at least one interaction ... in the previous 30 days", based on data for 14,500 users. The draft set it beside a "used it last week" measure with no definition, so I added "meaning licence holders active in the previous 30 days" (+8 words). Both fragments are word for word.
   - **1,000 licences: pass.** DBT (2025): "One thousand licences were available for a 3-month pilot from October to December 2024 and were allocated to UK-based staff". The ellipsis drops only "were available". The sample was "volunteers (~70%) and randomly selected participants (~30%)". DBT is labeled not US in the spreadsheet bullet, and the 20,000 and 1,000 sentence names the UK.
4. **"Mostly Microsoft Research authors": pass, plus one fix.** Dillon et al.: three of four authors are at Microsoft Research, so it stays. Lee et al.'s label said "Microsoft Research authors", but six of seven are, so it is now "mostly Microsoft Research authors".
5. **Stop rule, thresholds and read-only advice: pass.** Every bar, the check dates, the 3 to 5 baseline tasks, the spending limit, read-only and the end-date decision are labeled ours ("our judgement", "Bar (ours)", "we suggest"). No source is cited for any threshold. The "Pilots do track use" paragraph cites sources only for tracking use, not for any cut-off.
6. **Brynjolfsson et al. at p. 933: pass.** Re-verified live on the QJE article page; the quote is word for word.
7. **"maker of Grok" and "mostly US or Europe": pass.** Both are gone.

## Fact-check log (live, Fri Nov 20, 2026, about 5:45 to 6:15 PM ET)
- **Quote fragments:** a script compared every fragment and ellipsis against the live text. All 54 match.
  - Two Pennsylvania items were checked by page layout because the PDF interleaves its columns: "14 state government agencies" (the p. 9 infographic: "14 / state government agencies represented in the pilot"), and the p. 43 "predicted ... half as many use cases".
  - Olson et al. was checked in the browser, since PMC blocks scripted fetches.
- **Pennsylvania pages:** 2, 3, 8, 9, 11, 12, 16, 33, 34, 43, 48 and 54 all match.
- **METR (Becker et al.):** 16 developers, 246 tasks, randomized. The quotes are on pp. 1, 10 and 12. Labeled preprint, small sample.
- **Other studies:** Bick et al. pp. 2, 10, 16, 17; Pew p. 23 (late 2024); Noy and Zhang p. 187; QJE p. 889 and p. 933; Humlum; Lee; BetterUp p. 1; DSIT; Playbook; Service Manual. All pass.
- **References:** every in-text cite has an entry and every entry is cited, including the new CAISI and GAO entries. Alphabetical order is correct: Center before Commonwealth, and U.S. Government last. Page ranges use the APA en dash (889–942, 1–22, 187–192, 698–701), kept for the reason logged last round. There are 0 em dashes.

## Cuts (to pay for the definition)
- "Grok Bot is one more example of the tools a pilot could include, and none of these studies tested it." (20 words.) Addendum 5 §3 allows cutting it, and the article stays tool-agnostic.
- "For this reason, a pilot should judge each use on its own, not the pilot as a whole." (17 words.) It followed the 1.4% average as if it were the reason, which is a non sequitur, and the stop rule already says to judge each use case.

## Scores
| Principle | Score | Note |
|---|---|---|
| Useful | 5 | Five asks and a stop rule saying what is measured, by when and what happens |
| Clear | 4 | Every term now cited. The labels and the table source note are dense |
| Credible | 5 | Every fragment word for word, each figure scoped (the UK adoption rate now defined), all "ours" items labeled, the thin evidence said plainly |
| Concise | 4 | 2,490 words as X counts them |
| Iterative | 5 | Last round's fixes held (p. 933, Dillon label). The definition gap was closed from the brief within the hour |
| **Average** | **4.6** | |

## For Wade / Rhett
- **Wade:** `03-outline.md` still lists the working definition and the Grok Bot example sentence.
- **Optional, not added (length):** GAO p. 2 also supports the risk line: "Without sufficient oversight, mistakes or unintended consequences could go undetected."

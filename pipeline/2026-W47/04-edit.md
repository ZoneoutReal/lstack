# Edit: 2026-W47 (trim pass)

Piece: "Don't wait for the company rollout: run a capped, four-week opt-in." Jon asked for a trim: shorter table cells, a body of about 2,000 to 2,500 words, and APA "et al." for three or more authors. Wade built it on 4eead5b's `04-final.md` at 83fb869. This file replaces the edit log for 4eead5b. Governing files are unchanged since 4eead5b and were re-read.

## Word count
Counted as X counts it: the whole file, excluding table rows and URLs, references included. That method gives 3,951 for 4eead5b and 2,497 for Wade's draft, matching Wade's figures. `04-final.md`: **2,495**, or 1,830 for the body without references. Every addition below is offset by cuts.

## Fact-check
A script diffed every quoted fragment, split at each ellipsis, against live page text fetched Fri Nov 20, 2026, after 1:30 PM. All 43 checkable fragments are verbatim. Not script-checkable:
- Scare quotes: "not worth the cost", "Capped spend".
- Puthal et al.: Springer blocks scripted fetches. The quote was verified at source in round 1 and is unchanged.
- The two lstack quotes: they matched once the source's markdown bold was ignored.

| Item | Verified |
|---|---|
| Wade's examples: "Small time savings" (DBT), "seat stays on your plan" (team plans, from "Their seat stays on your plan") | ✅ verbatim fragments; meaning intact |
| "a new seat ... charged a prorated amount..." | ✅ the ellipsis drops only "is bought and" |
| "every member has access without any admin action ... There is no switch to turn it off" | ✅ the ellipsis drops a list of what members can do |
| Grok Bot docs (pricing, caps, teams, meetings, team plans, cancel, routines, team bots, computer) | ✅ live. "Last updated" dates unchanged since this morning (latest Nov 17) |
| Microsoft Copilot $30.00 add-on; Business promo "Originally starting from $21.00 now starting from $18.00" | ✅ promo still running. Offer terms: "available between July 1, 2026, and December 31, 2026" |
| Google Workspace $7 / $14 / $22; Meet notes editions; "up to 10 active schedules at a time" | ✅ |
| OpenAI Codex pricing ($20 annual, "$25 per user per month when billed monthly"); Business overview seat quote | ✅ |
| Research quotes (Bick et al. pp. 10, 16, 17; Pew p. 23; Pendell; Kemp; GDS; DSIT; DBT; Service Manual; Playbook) | ✅ |
| All table cells checked against their pages and the outline's cell map | ✅ two cells fixed (see check 1) |
| Em dashes, overclaims, tools Jon doesn't use, Jon's surname or address | ✅ none |

## Wade's checks
1. **Plan qualifiers.**
   - Grok Bot meetings: left as is. A team pilot runs on a Team plan, which Meetings covers, and the cost section quotes the full plan gate. The cell doesn't mislead for this article's reader.
   - Gemini Meet notes: restored "(Business Standard and up)". With the price row listing $7 Starter, the cell implied Starter gets Meet notes.
   - Also fixed: "Up to 10 schedules" is now "Up to 10 active schedules" (the source's limit is on active schedules), and "per user" was added to the ChatGPT and Gemini price cells so every price row has the same unit. Table cells aren't in the X count, so these cost nothing.
2. **Quote fragments.** Every fragment and ellipsis is verbatim and keeps its meaning (see the table). This is the first W47 round with no fragment errors.
3. **Brookings 13c.** Not restored. The US point (few workers get encouragement) is carried by Pew's 12%, and the France and Italy comparison isn't needed for a US reader. The Bick et al. (2026) reference is correctly gone with it.
4. **Live re-check.** Done (see the table). Nothing changed since this morning's pass, and the Copilot promo is still live.

## Other fixes
- **Brief requirement restored:** the brief's corrections say to state that prices exclude tax and that third-party models cost extra. The trim had dropped both. Restored: "before tax" and "Third Party model usage in Cursor" costs extra (vendor wording, about 9 words).
- **Hedges restored:** "some form of" before the shared-features list, and "appear to lie" for the differences. The trim had turned both into flat claims.
- **Gender gap:** the 6-point figure is labeled "current US work use" again, as fixed in round 1.
- **DSIT citation:** the narrative mention plus a duplicate parenthetical is now "Department for Science, Innovation and Technology (2025) notes...". The 26-minute figure is cited to GDS (2025b) directly. This saved about 6 words.
- **References:** "Usage limits" (2026j) no longer supported any sentence; it was only attached to the Auto Top-up line, which the spending caps page covers. Cite and entry removed, and "Use the computer and apps" re-lettered from 2026k to 2026j.
- **Cut:** "simply".

**APA:** "et al." is used from first mention for Bick et al. (three authors) and Puthal et al. (five), and "Lin and Parker" / "Lin & Parker" for two. Organizations are named in full at first use, with GDS and DBT abbreviated after. A script cross-check found every in-text cite matches a reference entry and every entry is cited.

## Scores
| Principle | Score | Note |
|---|---|---|
| Useful | 5 | Five-item ask plus a four-row fit table an exec can use today |
| Clear | 4 | Short cells and one source note per table. Billing terms stay a little dense |
| Credible | 5 | Every quote verbatim and every cell traced to a live page. Hedges and brief-required price caveats restored. Counterpoints named |
| Concise | 4 | 2,495 words as X counts them, inside Jon's range. Each section carries a decision |
| Iterative | 5 | Jon's trim asks met. Last round's lesson applied: every fragment diffed against source, with zero errors this round |
| **Average** | **4.6** | |

## Send-backs
0 of 1 used. The angle is unchanged and sound. Fixes are cuts and clarifications.

**Pre-publish:** re-check x.ai/pricing, the docs.x.ai pricing, caps, team plans, teams and meetings pages, Microsoft's Copilot business page (promo ends Dec 31, 2026), workspace.google.com/pricing, and OpenAI's Codex pricing and Business overview.

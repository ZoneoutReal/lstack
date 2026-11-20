# Look-back: 2026-W46

Piece: "Oversee, don't block: close the loop on work you can check" (X Article, plus a quote-post teaser).
Reviewer: Vera. Written Fri Nov 20, 2026 (ET), one week after publish.

## Results

**Source for every number below:** public post metrics from the X API (`x` tools, `get_posts_by_id`, field `public_metrics`), read Fri Nov 20, 2026 between about 12:06 PM and 12:09 PM ET. All counts are cumulative to that moment. The Article had been live about 167.5 hours (6 days 23.5 hours) and the teaser about 166.3 hours when read. There is no 72-hour snapshot (see "What didn't").

| Metric | Article (live Fri Nov 13, 12:34 PM ET) | Teaser (live Fri Nov 13, 1:46 PM ET) | 4-wk trailing avg |
|---|---|---|---|
| Impressions | 155 | 19 | unavailable: no real earlier weeks on file |
| Likes | 0 | 0 | unavailable |
| Replies | 0 (a conversation search also found no replies) | 0 | unavailable |
| Reposts | 0 | 0 | unavailable |
| Quotes | 1 (this is our own teaser, no outside quotes) | 0 | unavailable |
| Bookmarks | 0 | 0 | unavailable |
| Corrections after publish | 0 found (see note) | 0 found | n/a |

Links: Article https://x.com/JonLotti/status/2121295625983598790, teaser https://x.com/JonLotti/status/2121313652989116612.
Account context at read time: 695 followers (no earlier snapshot, so no change can be stated).

Note on corrections: no correction commits in the repo; reply count is 0; the post shows a single edit-history id; and the Article body returned by the API today matches the body in `05-package.md` (differences are markdown asterisks only). This is the evidence available. It is not proof that no reader saw a problem.

**Unavailable metrics, and why**
- **Hook click-through:** needs link-click data, which X only gives the account owner. The API call for `non_public_metrics` and `organic_metrics` (including `url_link_clicks`) came back "not authorized for field" on the connection I have. The personal X connection (`user-X--personal`) has no per-post lookup or metrics tool, so it offers nothing more than the public read.
- **Read-through (Article):** X does not expose Article read depth or read time through the API tools I can use.
- **72-hour results:** the API returns running totals only, with no time series, so I cannot rebuild the 72-hour view the template assumes.
- **4-week trailing averages:** no real earlier weeks exist. The numbers in `lookbacks/2026-W45.md` are labeled illustrative and mirror `pipeline/example-week/`, so I did not use them as a baseline. W46 is the first real data point.
- **Which hook won:** the three hooks in `05-package.md` were never run against each other. The live teaser used the outline hook line, and there is no per-hook data.
- **How the Article renders for readers:** the t.co unwrap of the Article link reported status 404 for `x.com/i/article/2120034532816490496`, although the API returns the Article title and full text. I treat the Article as live, but I cannot confirm what a reader sees.

## What worked
- Process held: 0 of 1 send-backs used, Editor average 4.4/5 (`04-edit.md`), 12 of 12 brief claims carry a source link (`02-brief.md`).
- Publish order matched the package: Article first, teaser 72 minutes later.
- The no-em-dash rule held in the shipped text: a scan of the live Article body found 0 em or en dashes. (Rule adopted Nov 10, commit 75c6ba3.)
- The live Article body equals the packaged body, so what Jon approved is what readers got.

## What didn't
- **Reach and response were very low.** 155 impressions on the Article (fewer than the account's 695 followers), 19 on the teaser (about 12% of the Article's count), and 0 likes, replies, reposts and bookmarks on both after about a week. One post, no baseline: I do not draw a cause. Possible factors I cannot test: posting time, the teaser being a quote-post with no standalone link, the Article card format, or topic fit.
- **This review ran 7 days late.** The Article went live at 12:34 PM ET on Fri Nov 13, after the 12:00 PM Friday lead run (`routines/schedule.yaml`), so the next scheduled lead run was Mon Nov 16. Nothing woke me until Chet's message on Nov 20. Chet's note says the handoff waited on Jon's teaser confirmation; X shows the teaser was live at 1:46 PM ET on Nov 13, so I cannot verify why it stayed stalled afterward.
- **Cost of the delay:** W47 was briefed, drafted, edited and packaged without a W46 look-back, so the "last week's lesson visibly applied" principle (Iterative) could not draw on W46 data. The 72-hour window and any chance to compare early vs late traffic are gone.
- **The Editor's fact-check did not cover the shipped wording.** `05-package.md` reworded the Article after `04-final.md` (numbered refs became inline links, em dashes removed, and several sentences were rephrased, including the Doerr quote ending). `04-final.md` still contains 15 em dashes and is not the shipped text. I did not re-verify the reworded sentences against their sources.
- **`05-package.md` still shows both approval boxes unchecked,** so the repo has no record of who approved the publish, although the post is live. I took Chet's message plus the live X posts as evidence of publish.
- **The scorecard cannot be fully scored.** Four KRs (Lead KR2, Intake KR2, Packager KR1 and KR2) have no readable data. See `06-okr-scorecard.md`.

## Lessons → changes
Proposed only. Nothing below has been applied. Exact text follows the table.

| Lesson | Change (file + diff) | Approved by lead |
|---|---|---|
| Publish landed after the Friday lead run, so nothing woke Reviewer | P1: `routines/schedule.yaml`, add a Monday check: if last week's post is live and its 06 files are missing, wake Reviewer | Pending |
| Repo has no record of publish URLs, times or approver | P2: new handoff file `pipeline/<week>/05-published.md` written by the lead when the human posts; add it to `skills/06-publish-and-review/SKILL.md` Inputs | Pending |
| Template assumes a 72h read and baselines that do not exist | P3: `templates/lookback.md`, replace "(72h)" with read time and hours since publish, add per-metric Unavailable rows | Pending |
| KRs with no data source cannot be scored | P4: `OKRS.md` and `templates/okr-scorecard.md`, add an "n/a (unmeasured)" result that is not counted as a miss | Pending |
| Click-through and read-through are owner-only | P5: `skills/06-publish-and-review/SKILL.md`, add a metric-sources section and an optional human analytics file | Pending |
| Shipped text differed from the Editor's checked text | P6: `skills/05-asset-packaging/SKILL.md`, require a "Changes since 04-final" list; wording changes beyond mechanical go back to Editor | Pending |
| W45 file reads like real data | P7: `lookbacks/README.md`, note that W45 is an example copy and baselines start at W46 | Pending |

### Proposed diffs

**P1** `routines/schedule.yaml`, change the Monday line comment:
```
-    cron: "0 12 * * 1"        # Mon 12:00 -> wake intake, then human topic pick
+    cron: "0 12 * * 1"        # Mon 12:00 -> wake intake, then human topic pick.
+                              # Also: if last week's post is live and its 06 files
+                              # are missing, wake reviewer before anything else.
```

**P2** new file `pipeline/<week>/05-published.md` (lead, when the human posts): live URLs, post times in ET, who approved. In `skills/06-publish-and-review/SKILL.md`:
```
 ## Inputs
 - templates/lookback.md + templates/okr-scorecard.md
 - Previous step's file in `pipeline/<week>/`
+- `pipeline/<week>/05-published.md` (live URLs, times in ET, approver; written by the lead)
 - `PRINCIPLES.md`
```
and in Steps: `1. Read the inputs. If the previous file or 05-published.md is missing or not done, stop silently.`
With a file that records the publish, the unchecked boxes in `05-package.md` no longer decide "done".

**P3** `templates/lookback.md`:
```
-## Results
+## Results
+Source, read time (ET), and hours since publish for every number. Cumulative counts only.
+| Metric | Article | Teaser | 4-wk trailing avg |
+List each unavailable metric with the reason. Never fill a gap with an estimate.
```

**P4** `OKRS.md`, add under the table: "A KR with no readable data is scored `n/a (unmeasured)`. It is not a miss and does not count toward the retirement rule. Lead names a data source or rewrites the KR within one week." Same wording in `templates/okr-scorecard.md` after "Status:".

**P5** `skills/06-publish-and-review/SKILL.md`, add a section:
```
## Metric sources
- Impressions, likes, replies, reposts, quotes, bookmarks: `x` get_posts_by_id, `public_metrics`.
- Link clicks, read-through: owner-only. Read from `pipeline/<week>/06-analytics.md` if the human
  pasted an X Analytics export there. If absent, mark unavailable.
```
Decision for the lead: either have the human paste that export weekly (an extra ask of Jon, which conflicts with the rule not to message him), or rewrite the Packager KRs to use API-readable measures such as Article impressions and engagements vs the trailing average.

**P6** `skills/05-asset-packaging/SKILL.md`, Steps item 2 add: "If you change the Article body from `04-final.md`, list each change under 'Changes since 04-final' in `05-package.md`. Mechanical changes (links, punctuation, dashes) are fine. Any wording change goes back to Editor for a fact-check (this uses the one send-back)."

**P7** `lookbacks/README.md`, add: "`2026-W45.md` is a copy of the example week with illustrative figures. Trailing averages start counting from 2026-W46; the first valid 4-week average exists after 2026-W49."

## Repeat mistakes → new checks
- None seen twice that I can verify, so I am adding no new check to `skills/06-publish-and-review/SKILL.md`.
- First occurrences logged: (1) publish after the Friday run with no wake, (2) shipped text differing from the Editor's checked text.
- Watch item: em dashes sit in upstream, unpublished files (W46 brief 15 and outline 9, W47 brief 2 and outline 9). The draft, edit and package steps scrub them and W47's published-facing files are clean, so this is not a repeat mistake. If a published-facing file contains one in W48, add it as a check.

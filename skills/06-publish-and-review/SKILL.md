---
name: 06-publish-and-review
owner: Reviewer
day: Fri PM
---
# 06 Publish & Review

**Owner:** Reviewer · **Runs:** Fri PM

## Job
Published results, a look-back, and proposed skill changes.

## Inputs
- templates/lookback.md + templates/okr-scorecard.md
- Previous step's file in `pipeline/<week>/`
- `pipeline/<week>/05-published.md` (live URLs, times in ET, approver; written by the lead)
- `PRINCIPLES.md`

## Output
- `pipeline/<week>/06-lookback.md, 06-okr-scorecard.md`

## Steps
1. Read the inputs. If the previous file or 05-published.md is missing or not done, stop silently.
2. Fill the template completely. No placeholders left.
3. Check against the definition of done below.
4. Write the file. That is the handoff.

## Metric sources
- Impressions, likes, replies, reposts, quotes, bookmarks: `x` get_posts_by_id, `public_metrics`.
- Follower change: `x` get_users_by_username, `public_metrics.followers_count`, compared with the last recorded count.
- Link clicks and read-through are owner-only and not readable. Mark them unavailable and say why.

## Definition of done
Results pulled; look-back written; each lesson is a proposed diff to a skill or checklist.

## Checks (added after repeat mistakes)
- _None yet. The Reviewer adds checks here when a mistake happens twice._

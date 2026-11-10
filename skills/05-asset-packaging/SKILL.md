---
name: 05-asset-packaging
owner: Packager
day: Fri AM
---
# 05 Asset Packaging

**Owner:** Packager · **Runs:** Fri AM

## Job
Title, hooks, thread version, images, alt text, an X version (launch channel).

## Inputs
- templates/package.md
- Previous step's file in `pipeline/<week>/`
- `PRINCIPLES.md`

## Output
- `pipeline/<week>/05-package.md`

## Steps
1. Read the inputs. If the previous file is missing or not done, stop silently.
2. Fill the template completely. No placeholders left.
3. Check against the definition of done below.
4. Write the file. That is the handoff.

## Definition of done
X version is ready; every image has alt text; lead approval requested.

## Checks (added after repeat mistakes)
- No em dashes (—) in post copy, captions, titles, hooks, thread text or channel versions. Use a comma, period, colon or parentheses instead.

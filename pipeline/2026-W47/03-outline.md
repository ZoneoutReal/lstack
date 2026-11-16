# Outline — Put the boring checks in before you scale agent volume

- **Hook:** Lauren Tan's team reports 10,926 merged PRs in October 2026 from about 227 contributors, with 0.47% of commits reverted. DORA's 2024 numbers say more AI adoption usually means less stable delivery. The difference is not the volume. It is what was in place before the volume. (claims #11, #12, #13, #16)
- **Promise:** Five boring, deterministic checks that apply to every pull request no matter who or what wrote it, plus a four-question test for whether they are in place before you let volume rise.

## Sections
1. Why volume is not proof: Tan's thesis and DORA's amplifier finding — claims: #1, #11, #12, #13, #16, #17; counterpoint 5 (used)
2. Where to spend effort: the inverse pyramid, review at the bottom — claims: #2, #3, #6
3. Check 1. Make the wrong thing impossible (architecture) — claims: #5, #7
4. Check 2. Lint rules that point at the root cause, not comments — claims: #8
5. Check 3. Types, compilers and tests — claims: #2, #6
6. Check 4. Let the agent run the code and show evidence — claims: #10; counterpoint 4 (used: formal methods not a silver bullet)
7. Check 5. Turn every repeated correction into a check, then clean up the old cases — claims: #4, #9
8. The plain test: four questions before you let volume rise — claims: #4, #6, #12, #13, #14, #18
9. What the numbers do not prove — claims: #12, #14, #15, #18; counterpoint 1 (used: low reverts are not good code), counterpoint 2 (used: PR count is not quality), counterpoint 3 (used: one team, self-reported, coincided not caused), counterpoint 4 (used: checks do not replace judgment)

All five counterpoints used; none dropped.

## Close / call to action
Tan's order of operations: fix the codebase and the verification story before you automate, because "if your inner coding loop produces slop, then automating that loop just produces more slop" (claim #15). This week: take the last review comment you wrote twice and turn it into a check, and start tracking reverts and hotfixes next to PR volume (claims #4, #18).
